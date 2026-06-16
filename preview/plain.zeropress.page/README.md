# plain.zeropress.page

Preview site for `zeropress.plain`, the minimal document theme bundled with `@zeropress/build-pages`.

This site is maintained inside the `zeropress.page` repository so individual theme previews can be deployed from subdirectories.

## Build

Use `build.sh` for the full preview build:

```bash
bash ./build.sh
```

The script runs Build Pages and formats the generated HTML. The generated deployable site is written to `_site/`.

## Static Hosting

When deploying this preview from a repository that contains multiple sites, set the hosting provider's project root or root directory to this folder:

```txt
preview/plain.zeropress.page
```

Then use `bash ./build.sh` as the build command and `_site` as the output directory.

## Core Build Only

For a minimal Build Pages run without the preview site's postbuild steps:

```bash
npx --yes @zeropress/build-pages --source ./documents --destination ./_site --public-dir ./public --theme plain
```
