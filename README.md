# zeropress.page

Theme preview and usage example repository for ZeroPress-maintained sites.

This repository contains small, deployable preview sites that demonstrate bundled ZeroPress themes and ordinary Build Pages project structure. The previews are intended to help theme users and site authors inspect real source files before creating their own documentation site.

## Repository Structure

```txt
preview/
  zeropress.page/
  docs1.zeropress.page/
  plain.zeropress.page/
```

Each directory under `preview/` is an independent Build Pages site with its own:

- `documents/` Markdown source tree
- `public/` public asset directory
- `documents/.zeropress/config.json` site configuration
- `build.sh` deploy build script
- `README.md` site-specific notes

The repository root is only a container for these preview sites. Build and hosting commands should be run from an individual preview directory, or the hosting provider's project root should be set to that directory.

## Preview Sites

| Site | Purpose |
| --- | --- |
| `preview/zeropress.page` | Index site for ZeroPress-maintained theme previews. |
| `preview/docs1.zeropress.page` | Preview for the compact `zeropress.docs1` documentation theme. |
| `preview/plain.zeropress.page` | Preview for the minimal `zeropress.plain` document theme. |

## Usage

Use these projects as reference material when starting a new Build Pages site:

- copy the source directory shape that matches your project
- compare how `documents/`, `public/`, and `.zeropress/config.json` work together
- inspect Markdown examples for links, images, media, tables, code blocks, and front matter
- review theme preview output before choosing a bundled theme

For a specific preview, open that preview directory and read its local `README.md`.

## Links

- [ZeroPress](https://zeropress.app)
- [Build Pages documentation](https://build-pages.zeropress.dev)
- [Theme authoring documentation](https://zeropress.dev/theme-authoring/)
