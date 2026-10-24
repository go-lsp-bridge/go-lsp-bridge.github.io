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

## The design is not here

It comes from the shared Hugo module
[`go-fleettools/landingkit`](https://github.com/go-fleettools/landingkit),
pinned in `go.mod` (Renovate bumps it); `kit.go` keeps `go mod tidy` from
deleting that requirement. `[params.brand]` in `hugo.toml` is read from the logo by
`landingkit brand`. A file under `layouts/partials/` with the name of one of the
kit's would silently override it.
