# Bullet Variants

> **This plugin is now part of [Vault Management](https://github.com/VeryRandomness/obsidian-vault-management)**, which combines bullet variants, color swatches, bulk property editing and theme updates in one plugin. This repo is archived and no longer updated.

An [Obsidian](https://obsidian.md) plugin with extra bullet styles for lists. It only changes how bullets look; your notes keep exactly what you type.

| You type | Bullet shown |
| --- | --- |
| `- text` | The normal dot |
| `+ text` | A `+` sign |
| `- \|-> text` | An arrow: down, then right |
| `- => text` | A right arrow, for "moved" |
| `- ? text` | A question mark |

A space must follow the symbol. Tasks (`- [ ]`), numbered lists, `*` bullets and code blocks are left alone.

- **Live Preview:** the typed `|->`, `=>` or `?` is hidden until your cursor is on that line.
- **Reading view and phone:** the same shapes appear. They are drawn as small images, so fonts can't change them.
- **Colours** come from your theme's bullet colours.
- **Shift+Alt+8** (command: **Cycle bullet style**) changes the bullet on the current line, or on every bullet in a selection: normal, `+`, `|->`, `=>`, `?`, then back to normal.

## Install

Copy `main.js`, `manifest.json` and `styles.css` into `<vault>/.obsidian/plugins/cb-bullet-variants/` (the folder name must match the plugin ID), then enable **Bullet Variants** under Settings → Community plugins.

## Updates

The plugin updates itself. On startup it compares the version in this repo's `manifest.json` with the installed one and, if the repo's is newer, installs the new files and reloads. The command **Check for update now** does the same on demand. To ship a change, raise `version` in `manifest.json` and push.

The ID `cb-bullet-variants` is deliberately unique, so Obsidian's "Check for updates" can't replace it with a different plugin.
