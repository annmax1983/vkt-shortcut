# vkt-shortcut — Keyboard Shortcut Manager

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A lightweight browser extension that blocks and remaps keyboard shortcuts. Stop unwanted hotkeys, redirect keys to custom actions, and take full control of your keyboard.

> Chromium-based · Manifest V3 · No tracking · Fully Local Processing

---

## Why vkt-shortcut?

Most shortcut blockers only block keys — they can't remap them. vkt-shortcut is different: **block for free, remap with Premium**, with one rule set that applies everywhere by default — plus per-site scoping when you need it.

| Advantage | Detail |
|-----------|--------|
| 🚫 **Block Keys** | Intercept and disable page-level shortcuts on any website (web apps, games) |
| 🔁 **Remap Keys** | Redirect one key combo to another inside the page (Premium) |
| 🌐 **Global + Per-Site Rules** | Rules apply on every website by default; optionally scope a rule to one site (subdomains included) |
| ⚡ **Site Presets** | One-click block rules for well-known shortcut conflicts on popular sites — YouTube (K/J/L/M/F/C/I/T), X (N/L/R/T/B/M, /), Reddit (A/Z votes, J/K/C/S), Facebook (J/K/L/C/S, /), GitHub (S/T/W/B/X), Doubao's Ctrl+J, Notion's Ctrl+P/J, VS Code Web's Ctrl+P/J. Every supported site is listed in the panel, so you don't have to visit it first. Each preset key becomes one rule, so the free 20-rule cap applies |
| 🔇 **Block All Shortcuts** | A per-site toggle that neutralizes every page shortcut, plus a global switch on the panel for all sites at once (typing, arrow-key navigation, clipboard and refresh still work; per-site pause takes priority) |
| ⌨️ **Key Recording** | Press the key combo directly — captured automatically |
| 📤 **Import / Export** | Backup and restore rules as JSON (Premium) |

---

## Free vs Premium

| Plan | Features |
|------|----------|
| **Free** | Block shortcuts, key recording, global toggle, up to 20 enabled rules |
| **⭐ Premium** | Unlimited rules, key remapping, import/export JSON, priority support |

All core features (block, record) are free forever. **Key Remapping** and **Import/Export** require a VKT Premium license.

- ⚙ Activate it: open the vkt-shortcut side panel → click the **⚙** button → enter your license key.

> License activation is **optional**. The free tier works fully without it — no account, no sign-up, no license key required.

---

## Preview

<p align="center">
  <img src="screenshot/promo.png" alt="vkt-shortcut Preview" width="640">
</p>

---

## Supported Browsers

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Fully supported |
| Microsoft Edge | ✅ Fully supported |
| Other Chromium-based browsers | ✅ Should work |

---

## Installation

1. Visit the Chrome Web Store page for vkt-shortcut
2. Click **Add to Chrome** and confirm
3. Click the ⌨️ vkt-shortcut icon in your toolbar to open the side panel

---

## Usage

1. **Click the ⌨️ icon** in your browser toolbar to open the side panel
2. **Click "➕ New Rule"** to create a shortcut rule
3. **Choose rule type** — Block (disable key) or Remap (redirect key A → key B)
4. **Set the source key** — click the input field and press the key combo you want to intercept
5. **For remap: set the target key** — click the target input and press the combo to redirect to
6. **(Optional) Scope to a website** — enter a domain like `youtube.com` (subdomains included), or leave blank to apply everywhere
7. **Save the rule** — it takes effect immediately, no page refresh needed
8. **Toggle rules** — use the global switch to pause without deleting
9. **(Shortcut) Panel bars** — a collapsible **Site Presets** list shows every supported site up front with its known conflicts and a one-click **Block** (✓ once all its keys are covered); the bar above it blocks all page shortcuts on every site at once, and the current-site bar adds a per-site block-all toggle plus a site pause switch

---

## Use Cases

- **Web apps** — Block F1 from opening help in Google Docs, Office 365, or any web editor
- **Online games** — Disable page-defined shortcuts that interfere with gameplay (note: browser-reserved keys like Ctrl+W or F11 never reach the page, so page-level interception cannot block them; extensions using `chrome.commands` can only neutralize a few by binding them to empty commands)
- **Developer tools** — Remap DevTools shortcuts to avoid conflicts with IDE keybindings
- **Accessibility** — Remap complex combos to simpler keys for easier access
- **Presentation mode** — Block all page-level shortcuts except navigation during presentations

---

## Privacy

- ✅ Rules never leave your browser — blocking/remapping happens entirely locally
- ✅ No analytics, no tracking, no cookies
- ✅ Rules stored in `chrome.storage.local` only
- ✅ Only `storage` + `sidePanel` permissions
- ℹ️ The only network requests are optional license activation/validation, which sends your license key, a random install identifier and browser metadata to our license server (`api.annmax1983.com`)

---

## Copyright Disclaimer

This extension intercepts keyboard events on web pages at the browser level for the user's convenience. All content, functionality and intellectual property of the original websites remain unchanged. Blocking or remapping shortcuts does not modify any website content — it only prevents or redirects keyboard input before it reaches the page.

---

## Source Code Notice

> ⚠️ **This repository does not publish source code.** It contains only usage documentation, release notes, and support resources. The extension is distributed exclusively through the Chrome Web Store. No offline installation packages or end-user source code are provided.

---

## License

Copyright © 2026 vkt-shortcut. All rights reserved.

---

## ❤️ Support

If you find vkt-shortcut helpful, consider buying me a coffee!

**[👉 Click here to support](https://ko-fi.com/annmax?ref=vkt-shortcut)**
