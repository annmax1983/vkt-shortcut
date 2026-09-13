# vkt-shortcut — Gestionnaire de raccourcis clavier

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | Français

Une extension légère qui bloque et redéfinit les raccourcis clavier. Bloquez les raccourcis indésirables, redirigez les touches vers des actions personnalisées et prenez le contrôle total de votre clavier.

> Chromium · Manifest V3 · Aucun suivi · Traitement 100 % local

---

## Pourquoi vkt-shortcut ?

La plupart des bloqueurs de raccourcis ne font que bloquer — ils ne peuvent pas les redéfinir. vkt-shortcut est différent : **bloquez gratuitement, redéfinissez avec le Premium**, avec un jeu de règles qui s'applique partout par défaut — plus un ciblage par site quand vous en avez besoin.

| Avantage | Détail |
|-----------|--------|
| 🚫 **Bloquer des touches** | Interceptez et désactivez n'importe quel raccourci clavier sur n'importe quel site |
| 🔁 **Redéfinir des touches** | Redirigez une combinaison vers une autre — rare dans les outils similaires (Premium) |
| 🌐 **Règles globales + par site** | Les règles s'appliquent sur chaque site par défaut ; limitez optionnellement une règle à un seul site (sous-domaines inclus) |
| ⌨️ **Enregistrement de touches** | Appuyez directement sur la combinaison — capturée automatiquement |
| 📤 **Import / Export** | Sauvegardez et restaurez les règles en JSON (Premium) |

---

## Gratuit vs Premium

| Plan | Fonctionnalités |
|------|----------|
| **Gratuit** | Blocage de raccourcis, enregistrement de touches, activation globale, jusqu'à 3 règles |
| **⭐ Premium** | Règles illimitées, redéfinition de touches, import/export JSON, support prioritaire |

Toutes les fonctionnalités de base (blocage, enregistrement) sont gratuites à vie. La **Redéfinition de touches** et l'**Import/Export** nécessitent une licence VKT Premium.

- ⚙ L'activer : ouvrez le panneau latéral vkt-shortcut → cliquez sur le bouton **⚙** → saisissez votre clé de licence.

> L'activation de la licence est **optionnelle**. Le niveau gratuit fonctionne entièrement sans elle — pas de compte, pas d'inscription, pas de clé de licence requise.

---

## Aperçu

<p align="center">
  <img src="screenshot/promo.png" alt="Aperçu vkt-shortcut" width="640">
</p>

---

## Navigateurs compatibles

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |
| Autres navigateurs basés sur Chromium | ✅ Devrait fonctionner |

---

## Installation

1. Rendez-vous sur la page Chrome Web Store de vkt-shortcut
2. Cliquez sur **Ajouter à Chrome** et confirmez
3. Cliquez sur l'icône ⌨️ vkt-shortcut dans votre barre d'outils pour ouvrir le panneau latéral

---

## Utilisation

1. **Cliquez sur l'icône ⌨️** dans la barre d'outils pour ouvrir le panneau latéral
2. **Cliquez sur « ➕ Nouvelle règle »** pour créer une règle de raccourci
3. **Choisissez le type de règle** — Bloquer (désactiver la touche) ou Redéfinir (rediriger la touche A → touche B)
4. **Définissez la touche source** — cliquez sur le champ de saisie et appuyez sur la combinaison à intercepter
5. **Pour une redéfinition : définissez la touche cible** — cliquez sur le champ cible et appuyez sur la combinaison de redirection
6. **(Optionnel) Limitez à un site** — saisissez un domaine comme `youtube.com` (sous-domaines inclus), ou laissez vide pour une application globale
7. **Enregistrez la règle** — elle prend effet immédiatement, aucun rechargement de page nécessaire
8. **Basculez les règles** — utilisez l'interrupteur global pour mettre en pause sans supprimer

---

## Cas d'utilisation

- **Applications web** — Bloquez F1 pour empêcher l'ouverture de l'aide dans Google Docs, Office 365 ou tout éditeur web
- **Jeux en ligne** — Désactivez les raccourcis définis par la page qui interfèrent avec le jeu (note : les touches réservées par le navigateur comme Ctrl+W ou F11 ne peuvent pas être interceptées par une extension)
- **Outils de développement** — Redéfinissez les raccourcis DevTools pour éviter les conflits avec les raccourcis de votre IDE
- **Accessibilité** — Redéfinissez des combinaisons complexes vers des touches plus simples pour un accès facilité
- **Mode présentation** — Bloquez tous les raccourcis sauf la navigation pendant les présentations

---

## Confidentialité

- ✅ Les règles ne quittent jamais votre navigateur — le blocage/redéfinition se fait entièrement en local
- ✅ Pas d'analytics, pas de suivi, pas de cookies
- ✅ Les règles sont stockées uniquement dans `chrome.storage.local`
- ✅ Permissions `storage` + `sidePanel` uniquement
- ℹ️ Les seules requêtes réseau sont l'activation/validation optionnelle de la licence, qui envoie des métadonnées de l'appareil à notre serveur de licences (`api.annmax1983.com`)

---

## Avertissement relatif au droit d'auteur

Cette extension intercepte les événements clavier sur les pages web au niveau du navigateur pour la commodité de l'utilisateur. Tout le contenu, les fonctionnalités et la propriété intellectuelle des sites web originaux restent inchangés. Le blocage ou la redéfinition de raccourcis ne modifie aucun contenu de site — cela empêche ou redirige simplement la saisie clavier avant qu'elle n'atteigne la page.

---

## Avis sur le code source

> ⚠️ **Ce dépôt ne publie pas le code source.** Il contient uniquement la documentation d'utilisation, les notes de version et les ressources d'assistance. L'extension est distribuée exclusivement via le Chrome Web Store. Aucun package d'installation hors ligne ni code source destiné aux utilisateurs finaux n'est fourni.

---

## Licence

Copyright © 2026 vkt-shortcut. Tous droits réservés.

---

## ❤️ Soutenir

Si vkt-shortcut vous est utile, offrez-moi un café !

**[👉 Cliquez ici pour soutenir](https://ko-fi.com/annmax?ref=vkt-shortcut)**
