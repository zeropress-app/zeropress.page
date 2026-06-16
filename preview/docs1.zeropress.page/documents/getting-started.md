# Getting Started

Docs1 is a small-site theme. It keeps navigation compact and lets each page focus on document content.

## Source Tree

A compact Build Pages source tree can mix ordinary Markdown files with directory index pages:

```txt
documents/
  index.md
  getting-started.md
  guides/
    markdown.md
    configuration.md
  markdown-examples/
    index.md
  .zeropress/
    config.json
public/
  favicon.png
```

The ordinary file `guides/markdown.md` is published as a page route under `/guides/markdown`. The directory index file `markdown-examples/index.md` is published as `/markdown-examples/`.

## Build Command

Use the bundled `docs1` theme:

```bash
npx --yes @zeropress/build-pages --source ./documents --destination ./_site --public-dir ./public --theme docs1
```

The generated site is static HTML and can be deployed to static hosting providers.

## Navigation Model

Docs1 works best when the primary menu can describe the whole site:

```json
{
  "menus": {
    "primary": {
      "name": "Primary Menu",
      "items": [
        { "title": "Overview", "url": "/" },
        { "title": "Getting Started", "url": "/getting-started" },
        { "title": "Markdown", "url": "/guides/markdown" },
        { "title": "Markdown Examples", "url": "/markdown-examples/" },
        { "title": "Reference", "url": "/guides/configuration" }
      ]
    }
  }
}
```

For deeper content sets, choose a sidebar theme such as `docs2`.
