# vkt-shortcut — Tastenkürzel-Verwaltung
[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | Deutsch | [日本語](README_ja.md) | [Français](README_fr.md)

Eine schlanke Browser-Erweiterung zum Blockieren und Umbelegen von Tastenkürzeln. Vermeiden Sie ungewollte Auslösungen, passen Sie das Tastenverhalten an und übernehmen Sie die volle Kontrolle über Ihre Tastatur.

> Chromium-basiert · Manifest V3 · Kein Tracking · Regeln zu 100 % lokal gespeichert

---

## Kernunterscheidungsmerkmale

| Problem bei Konkurrenten | vkt-shortcut Lösung |
|---|---|
| ❌ Nur Blockieren, kein Umbelegen | ✅ Tasten blockieren; Umbelegen als Premium-Funktion |
| ❌ Zersplitterte Regeln ohne zentrale Steuerung | ✅ Standardmäßig überall wirksam, optional auf eine Website beschränkbar, mit globalem Schalter |
| ❌ Komplizierte manuelle Tastensyntax | ✅ Einfach die Taste drücken – sie wird automatisch erkannt |
| ❌ Datenübertragung und Datenschutzrisiken | ✅ Gesamte Konfiguration bleibt lokal im Browser |
| ❌ Stark eingeschränkte Gratisversion | ✅ 3 kostenlose Regeln für den Grundbedarf |

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
| Regeln | Unbegrenzt, aktiv oder inaktiv |

### ⭐ Premium (per Lizenz freigeschaltet)

| Funktion | Beschreibung |
|---|---|
| **Tasten umbelegen** | Taste A wirken lassen wie Taste B |
| **Geräteübergreifender Sync** | Regeln über das angemeldete Browser-Konto abgleichen (ohne unsere Server) |
| **Prioritäts-Support** | Bevorzugte Unterstützung |
---

## Anwendungsfälle

- **Web-Apps** — F1-Hilfe in Google Docs oder Office 365 blockieren
- **Browserspiele** — Seiteneigene Spielkürzel deaktivieren, die das Gameplay stören (Hinweis: Browser-eigene Kürzel wie Strg+W oder F11 kommen nie auf der Seite an, daher kann sie die Seiten-Interceptor nicht blockieren; Erweiterungen mit `chrome.commands` können nur einige wenige per Leerbefehl neutralisieren)
- **Entwicklertools** — DevTools-Kürzel umbelegen, um Konflikte mit der IDE zu vermeiden
- **Barrierefreiheit** — Komplexe Kombinationen auf einfache Tasten mappen
- **Präsentationsmodus** — Während der Präsentation alle Kürzel auf der Seite außer der Navigation blockieren

---

## Installation

1. vkt-shortcut im Chrome Web Store aufrufen
2. Auf **Zu Chrome hinzufügen** klicken und bestätigen
3. In der Symbolleiste auf das ⌨️-Symbol klicken, um das Side Panel zu öffnen

---

## Datenschutz

- ✅ Regeln verlassen niemals den Browser — Blockieren und Umbelegen geschieht vollständig lokal
- ✅ Keine Analyse, kein Tracking, keine Cookies
- ✅ Regeln werden ausschließlich in `chrome.storage.local` gespeichert
- ✅ Nur die Berechtigungen `storage` + `sidePanel`
- ℹ️ Die einzigen Netzwerkanfragen sind die optionale Lizenzaktivierung und -prüfung (es werden Lizenzschlüssel, eine zufällige Installations-Kennung und Browser-Metadaten an unseren Lizenzserver `api.annmax1983.com` gesendet)

---

## Quellcode-Hinweis

> ⚠️ **In diesem Repository wird kein Quellcode veröffentlicht.** Es enthält ausschließlich Nutzungsdokumentation, Versionshinweise und Support-Angebote. Die Erweiterung wird nur über den Chrome Web Store vertrieben; Offline-Installationspakete oder Quellcode für Endnutzer werden nicht bereitgestellt.

---

## Support

Fragen, Feedback oder Funktionswünsche: **support@annmax1983.com**

---

## Lizenz

Proprietäre Software. Alle Rechte vorbehalten.
