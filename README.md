# canva-latex-engine

Static files for a TeX engine that runs in the browser, served through GitHub Pages and downloaded at run time by a Canva app.

This repository holds no application code. It is an unmodified subset of the [mp-tikz-wasm](https://github.com/jmckalex/mp-tikz-wasm) 0.5.0 release by J. McKenzie Alexander: the WebAssembly engines and the TeX Live files they read. Ghostscript and the OpenType bundles are left out, along with the JavaScript, source maps and macOS metadata files.

Some files have been added to the release, all unmodified from TeX Live 2025 and listed in `bundles/latex-extra/manifest.json`:

- `colortbl.sty` (v1.0k, by David Carlisle, LPPL 1.3c).
- From `sansmathfonts` (by Ariel Barton, LPPL 1.3c): `omlcmssm.fd` and the fonts `cmssmi5`–`cmssmi10` and `cmssmib5`–`cmssmib10` (TFM and Type 1), a sans-serif maths italic with Greek. Their lines from `sansmathfonts.map` are appended to the font maps in `bundles/core/files/fonts/map/`.

## Licences

The files keep their original licences. See `LICENSE`, `NOTICE.md` and `licenses/`. The engines are GPL.

Corresponding source for the engines is at the upstream [v0.5.0 tag](https://github.com/jmckalex/mp-tikz-wasm/tree/v0.5.0) and [release](https://github.com/jmckalex/mp-tikz-wasm/releases/tag/v0.5.0).
