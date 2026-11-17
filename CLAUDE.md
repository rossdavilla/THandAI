# From Prompt to App (`THandAI`)

A walkthrough for instructors: describe a class activity in plain language, have AI write the
app, and publish it. Live at <https://rossdavilla.github.io/THandAI/>.

## ⚠️ `index.html` is a bundle, and this repo has no source for it

```
index.html   ~1.35 MB, titled "Bundled Page" — one self-contained file with every
             image, style, script and font inlined as data URIs
LICENSE
```

The page is a **build artifact**: it was produced by inlining a multi-file page into a single
HTML file (the same kind of output the `build-standalone` skill produces). The 197 lines are
mostly enormous data URIs, so it is not meaningfully hand-editable, and the original source files
are not in this repository.

**So, before changing anything here:** ask Ross where the source lives. Editing the bundle
directly is only reasonable for a one-line text fix that can be located exactly; anything larger
means rebuilding from source. Do not reconstruct a source tree by extracting the data URIs and
then commit that as if it were the original.

## Publishing

GitHub Pages serves `main` from the repository root, so a push to `main` is the deploy. Because
everything is inlined, the page needs no network at all once loaded.

Already listed in `data/sites.json` in the
[`rossdavilla.github.io`](https://github.com/rossdavilla/rossdavilla.github.io) repo under the
`tools` tag.
