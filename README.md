# CCA LaTeX Template (Combinatorial Commutative Algebra)

This repository contains the LaTeX style file and a sample manuscript for preparing articles for the journal **Combinatorial Commutative Algebra (CCA)**.

## What’s in this repo

- `cca.sty` — the CCA style file
- `cca-sample.tex` — a sample file showing how to format a manuscript
- `cca-sample.pdf` — the expected output from the sample file
- `CCAlogo.png` — the CCA logo
- `refs.bib` — sample bibliography file (optional)

For a versioned download, use the Latest Release.

## Option 1: Local LaTeX (compile on your computer)

1. Download this repository (green **Code** button → **Download ZIP**) and unzip it.
2. Start by copying `cca-sample.tex` and editing it.
3. Make sure `cca.sty` stays in the same folder as your manuscript `.tex` file.

## Option 2: Overleaf

**Overleaf template (view-only):** https://www.overleaf.com/read/qnpqhkbsjrwk#c6d1f4

Please open the link and create your own editable copy (e.g. “Copy Project”), then write in your copy.

## Using the CCA style file

CCA papers should begin with:
```tex
\documentclass[12pt]{article}
\usepackage[amsmath]{cca}
```

Omit `[amsmath]` if you do not want to use the `amsmath` package.

### Notes / common pitfalls

- The style file sets page size and margins. Please do not load packages or add commands that change them (e.g. `geometry`, `fullpage`, etc.).
- `geometry`, `amssymb`, `amsthm`, `hyperref`, and `microtype` are already loaded. Please do not reload them or set their options.
- Forbidden packages: `fullpage`, `authblk`, `babel`.
- If you want `cleveref`, do not load it directly. Instead use:
  - `\usepackage[amsmath,cleveref]{cca}`
  - (Optional) set options via `\def\cleverefoptions{...}` as shown in `cca-sample.tex`.

## Questions / problems

If you run into a compilation issue or think something in the template should be improved, please open a GitHub Issue (or contact the CCA editorial team).

