# Plain Theme Preview

This site previews `zeropress.plain`, the minimal document theme bundled with `@zeropress/build-pages`.

Plain intentionally avoids headers, footers, menus, sidebars, search UI, and collection pagers. Each Markdown file is rendered as the document itself.

## Pages

Because this theme does not render navigation, this index page provides the site entry points as ordinary Markdown links:

- [Markdown Examples](markdown-examples/index.md): typography, code blocks, tables, alerts, Mermaid, iframe, video, and audio rendering.
- [Privacy Policy](legal/privacy.md): placeholder privacy page.
- [Terms of Use](legal/terms.md): placeholder terms page.

## What This Preview Shows

- standalone document rendering
- source Markdown links
- optional GitHub edit links
- updated dates
- progressive heading anchors
- code block copy buttons
- Mermaid lazy loading
- native media rendering

> [!NOTE]
> This preview asks crawlers not to index it and is maintained as a theme preview.

Use `zeropress.docs1` or `zeropress.docs2` when a site needs theme-rendered navigation.
