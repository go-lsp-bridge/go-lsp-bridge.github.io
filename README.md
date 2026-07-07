<p align="center"><img src="https://raw.githubusercontent.com/go-lsp-bridge/brand/main/social/go-lsp-bridge.png" alt="go-lsp-bridge/go-lsp-bridge.github.io" width="720"></p>

# go-lsp-bridge.github.io

The organization's institutional landing page, served at
<https://go-lsp-bridge.github.io> and built with [Hugo](https://gohugo.io). It
is a single page (custom `layouts/index.html`, capability cards driven by
`[[params.phases]]` in `hugo.toml`), with a light/dark/system theme toggle
(default = system).

Documentation lives in a separate repository,
[go-lsp-bridge/docs](https://github.com/go-lsp-bridge/docs), served at
<https://go-lsp-bridge.github.io/docs/>. This page links there.

`.github/workflows/deploy-pages.yml` builds the landing with Hugo and deploys it
to GitHub Pages on every push to `main`.

## Local preview

```bash
hugo server      # http://localhost:1313
```
