# YAMLPreview

**Preview YAML files in macOS Finder with Quick Look — just press Space.**

YAMLPreview is a lightweight macOS Quick Look extension. Select a `.yml` or
`.yaml` file in Finder, hit the spacebar, and see it rendered with clean syntax
highlighting and line numbers instead of plain, unstyled text.

It fills a real gap: macOS has **no built-in Quick Look previewer for YAML**.
The `.yml` / `.yaml` types resolve to the `public.yaml` UTI, which Apple's
built-in text previewer doesn't claim — so without this extension, YAML files
have no preview at all.

## Features

- **Instant previews** for `.yml` and `.yaml` files
- **Syntax highlighting** powered by highlight.js
- **Line-number gutter** for easy reference
- **Light & dark mode** — follows your system appearance automatically
- **Sandboxed, offline, and fast** — nothing leaves your Mac
- **Automatic updates** — built-in updater keeps you on the latest version

## Requirements

- macOS 26 (Tahoe) or later

## Installation

1. Download the latest **`YAMLPreview-x.x.zip`** from the
   [**Releases page**](https://github.com/jjnicolas/YAMLPreview-releases/releases/latest).
2. Unzip it and drag **`YAMLPreview.app`** into your **Applications** folder.
3. **Launch the app once.** This registers the Quick Look extension with the
   system. You can quit it afterward — the preview keeps working.
4. Select any YAML file in Finder and press **Space**.

The app is signed with a Developer ID and notarized by Apple, so it runs without
Gatekeeper warnings.

### Not seeing previews?

Quick Look sometimes needs a nudge after first install:

```sh
qlmanage -r          # reset the Quick Look cache
```

You can also confirm the extension is enabled under
**System Settings → General → Login Items & Extensions → Quick Look**.

## Updating

YAMLPreview checks for updates automatically and will prompt you when a new
version is available. You can also check manually from the app's menu.

## More apps

Part of [Julien Nicolas's macOS apps & utilities](https://apps.tnfnet.org).

## License

MIT © Julien Nicolas

---

<sub>This repository hosts the public release builds and the Sparkle update feed
(`appcast.xml`) for YAMLPreview.</sub>
