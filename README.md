# From Prompt to App

A walkthrough for instructors: describe a class activity in plain language, have AI write the app,
and publish it where students can use it.

**Live:** https://rossdavilla.github.io/THandAI/

## What's in here

```
index.html   the whole walkthrough — one file, ~1.35 MB
LICENSE
```

`index.html` is a **bundle**: every image, stylesheet, script and font is inlined into the file as
a data URI, so the page makes no network requests at all and can be opened straight from disk or
a USB stick. That also means it is not meaningfully hand-editable — the file is a few hundred
lines of very large data URIs — and the multi-file source it was built from is not in this
repository.

## Running it

Open `index.html` in a browser. Nothing to install, nothing to serve, no connection needed.
