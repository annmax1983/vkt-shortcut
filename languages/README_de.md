# vkt-shortcut — Tastenkürzel-Verwaltung
[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | Deutsch | [日本語](README_ja.md) | [Français](README_fr.md)

Eine schlanke Browser-Erweiterung zum Blockieren und Umbelegen von Tastenkürzeln. Vermeiden Sie ungewollte Auslösungen, passen Sie das Tastenverhalten an und übernehmen Sie die volle Kontrolle über Ihre Tastatur.

> Chrome / Edge / Firefox · Manifest V3 · Kein Tracking · Regeln zu 100 % lokal gespeichert

---

## Kernunterscheidungsmerkmale

| Problem bei Konkurrenten | vkt-shortcut Lösung |
|---|---|
| ❌ Nur Blockieren, kein Umbelegen | ✅ Tasten blockieren; Umbelegen als Pro-Funktion |
| ❌ Zersplitterte Regeln ohne zentrale Steuerung | ✅ Standardmäßig überall wirksam, optional auf eine Website beschränkbar, mit globalem Schalter |
| ❌ Komplizierte manuelle Tastensyntax | ✅ Einfach die Taste drücken – sie wird automatisch erkannt |
| ❌ Datenübertragung und Datenschutzrisiken | ✅ Gesamte Konfiguration bleibt lokal im Browser |
| ❌ Stark eingeschränkte Gratisversion | ✅ Blockieren, Presets und Import/Export sind kostenlos, ohne Regelbegrenzung |

---

## Funktionen

### 🆓 Kostenlos

| Funktion | Beschreibung |
|---|---|
| Tasten blockieren | Tastenkürzel innerhalb von Webseiten abfangen und deaktivieren |
| Tastenerkennung | Gewünschte Kombination einfach drücken – wird automatisch erfasst |
| Geltungsbereich | Standardmäßig auf allen Websites; optional auf eine Website beschränkbar (Subdomains inklusive) |
| Website-Voreinstellungen | Ein-Klick-Blockregeln für bekannte Konflikte auf beliebten Websites — YouTube (K/J/L/M/F/C/I/T), X (N/L/R/T/B/M, /), Reddit (A/Z-Stimmen, J/K/C/S), Facebook (J/K/L/C/S, /), GitHub (S/T/W/B/X), Doubaos Ctrl+J, Notions Ctrl+P/J, VS Code Webs Ctrl+P/J. Alle unterstützten Websites stehen direkt im Panel, ohne dass Sie sie erst besuchen müssen. Jede Preset-Taste wird eine eigene Regel; lässt sich einzeln bearbeiten oder löschen |
| Alle Kürzel blockieren | Ein Schalter pro Website, der jedes Seiten-Kürzel außer Kraft setzt, plus ein globaler Schalter oben im Side Panel für alle Websites auf einmal (Eingabe, Tastaturnavigation, Zwischenablage und Neu laden funktionieren weiterhin; die Website-Pause hat Vorrang) |
| Globaler Schalter | Alle Regeln mit einem Klick aktivieren/deaktivieren |
| Regeln | Bis zu 10 in der Gratis-Version (die Lizenz hebt das Limit auf); aktiv oder inaktiv |

### ⭐ Pro (per Lizenz freigeschaltet)

| Funktion | Beschreibung |
|---|---|
| **Tasten umbelegen** | Taste A wirken lassen wie Taste B |
| **Geräteübergreifender Sync** | Regeln über das angemeldete Browser-Konto abgleichen (ohne unsere Server) |

---

## Anwendungsfälle

- **Web-Apps** — F1-Hilfe in Google Docs oder Office 365 blockieren
- **Browserspiele** — Seiteneigene Spielkürzel deaktivieren, die das Gameplay stören (Hinweis: Browser-eigene Kürzel wie Strg+W oder F11 kommen nie auf der Seite an, daher kann sie die Seiten-Interceptor nicht blockieren; Erweiterungen mit `chrome.commands` können nur einige wenige per Leerbefehl neutralisieren)
- **Entwicklertools** — DevTools-Kürzel umbelegen, um Konflikte mit der IDE zu vermeiden
- **Barrierefreiheit** — Komplexe Kombinationen auf einfache Tasten mappen
- **Präsentationsmodus** — Während der Präsentation alle Kürzel auf der Seite außer der Navigation blockieren

---

## Unterstützte Browser

| Browser | Status |
|--------|--------|
| Google Chrome | ✅ Vollständig unterstützt |
| Microsoft Edge | ✅ Vollständig unterstützt |
| Mozilla Firefox | ✅ Vollständig unterstützt |
| Andere Chromium-basierte Browser | ✅ Sollte funktionieren |

> **Firefox-Hinweis:** Die Oberfläche öffnet sich in der Firefox-Seitenleiste (Ansicht → Seitenleiste → vkt-shortcut); die Berechtigung `sidePanel` wird in der Firefox-Version daher nicht angefordert. Die geräteübergreifende Synchronisierung läuft über Firefox Sync (Mozilla-Konto). Die übrigen Funktionen verhalten sich wie unter Chrome / Edge.

---

## Installation

| Store | Link |
|---|---|
| Chrome Web Store | [In Chrome installieren](https://chromewebstore.google.com/detail/afpgmhahakgmmjomkkocecnbcdjndial) |
| Microsoft Edge Add-ons | [In Edge installieren](https://microsoftedge.microsoft.com/addons/detail/odbcgmpmlcobfpahpcpcikhbfhajmila) |
| Firefox-Add-ons (AMO) | [Für Firefox installieren](https://addons.mozilla.org/firefox/addon/shortcut/) |

> Installieren Sie nur über die offiziellen Stores oben – meiden Sie Download-Seiten Dritter.

---

## Datenschutz

- ✅ Regeln verlassen niemals den Browser — Blockieren und Umbelegen geschieht vollständig lokal
- ✅ Keine Analyse, kein Tracking, keine Cookies
- ✅ Regeln werden ausschließlich in `storage.local` gespeichert
- ✅ Nur die Berechtigungen `storage` + `sidePanel` (`sidePanel` nur unter Chrome / Edge; Firefox nutzt die eigene Seitenleiste)
- ℹ️ Die einzigen Netzwerkanfragen sind die optionale Lizenzaktivierung und -prüfung (es werden Lizenzschlüssel, eine zufällige Installations-Kennung und Browser-Metadaten an unseren Lizenzserver `api.annmax1983.com` gesendet)

---

## Support

Fragen, Feedback oder Funktionswünsche: **support@annmax1983.com**

---

## Hinweis zum Quellcode

> ⚠️ **Dieses Repository dient ausschließlich der Projektpräsentation — der vollständige Quellcode wird hier nicht veröffentlicht.** Es enthält nur die Nutzungsdokumentation, die Release-Notizen und Support-Informationen zur Erweiterung.

> 📥 **Installation ausschließlich über die offiziellen Browser-Stores:** Chrome Web Store · Microsoft Edge Add-ons · Firefox-Add-ons (AMO). Von hier werden keine Offline-Installer verteilt.

---

## Lizenz

Diese Software ist proprietär und quellgeschlossen. Ohne vorherige schriftliche Genehmigung des Autors ist das Dekompilieren, Reverse-Engineering, Knacken, Verändern, Neuverpacken, Weiterverbreiten oder Weiterverkaufen der Software (ganz oder teilweise) streng untersagt.

Proprietäre Software. Alle Rechte vorbehalten.

---

## Links

- **Offizielle Website:** https://annmax1983.com/
- **Diese Erweiterung:** https://annmax1983.com/extensions/vkt-shortcut
- **Datenschutz:** https://annmax1983.com/privacy
- **Kontakt:** support@annmax1983.com
- **☕ Projekt unterstützen (Ko-fi):** https://ko-fi.com/annmax?ref=vkt-shortcut
