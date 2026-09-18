# Development workflow

Typst: https://typst.app
Ninja: https://ninja-build.org/

## Commands

```sh
ninja           # compile document.pdf (default)
ninja doc       # compile documetn.pdf
ninja dev       # start watching (auto-rebuild on save)
```

## Project structure

```
├── build.ninja                  # Ninja build file
├── src/
│   ├── main.typ                 # Entry point — document setup + chapter includes
│   ├── presentation.typ         # Entry point for presentation slides
│   ├── chapters/
│   │   ├── 010-introduction.typ
│   │   ├── 020-main-content.typ
│   │   ├── 030-conclusion.typ
│   │   └── 040-appendices.typ
│   ├── figures/                 # Image sources
│   ├── tables/                  # Large tables
│   └── refs/
│       └── references.bib       # Bibliography
├── document.pdf                 # Rendered article document
├── docs/                        # Some useful info about repository
│   └── dev.md
└── README.md
```

## VS Code Setup

In VS Code plugin Tinymist can be used for integrated PDF preview and
PDF-to-sources navigation.

## Agentic development

The project contains `.agents` directory with Typst skill and GOST-specific
knowledge which can be used while markup creation.
