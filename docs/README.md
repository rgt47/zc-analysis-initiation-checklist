# zzcollab Analysis Checklist: Companion Compendium

*2026-04-29 07:24 PDT*

This directory is a zzcollab research compendium that
accompanies the blog post 'A 55-Item Initiation Checklist
for zzcollab Data Analyses'. It serves two purposes:

1. **Host the deliverable artefact.** The standalone
   generic checklist lives at
   [`docs/analysis-checklist.qmd`](analysis-checklist.qmd).
   It can be copied into any zzcollab project and
   rendered to HTML or PDF without modification.
2. **Demonstrate the workspace layout the checklist
   refers to.** Every item in the checklist references a
   specific path inside this directory tree (for example,
   Item 5 names `analysis/data/raw_data/`, Item 18 names
   `analysis/scripts/01-clean-data.R`, Item 41 names
   `analysis/data/derived_data/`).

## Files of Interest

- [`docs/analysis-checklist.qmd`](analysis-checklist.qmd):
  the 55-item checklist (the deliverable artefact).
- [`../analysis/report/index.qmd`](../analysis/report/index.qmd):
  the blog post body. The root-level `index.qmd` is a
  symlink to this file.
- [`docs/DATA_WORKFLOW_GUIDE.md`](DATA_WORKFLOW_GUIDE.md):
  generic zzcollab data workflow notes carried over from
  the post-47 template.
- [`docs/ZZCOLLAB_BLOG_SETUP.md`](ZZCOLLAB_BLOG_SETUP.md):
  generic zzcollab blog-setup notes carried over from
  the post-47 template.
- [`docs/ZZCOLLAB_USER_GUIDE.md`](ZZCOLLAB_USER_GUIDE.md):
  reference for the broader zzcollab framework.

## Rendering the Checklist Standalone

```sh
quarto render docs/analysis-checklist.qmd
```

Produces `docs/analysis-checklist.html` and (if a TeX
engine is available) `docs/analysis-checklist.pdf`.

## Rendering the Blog Post

```sh
quarto render index.qmd
```

The root-level `index.qmd` symlinks to
`analysis/report/index.qmd`. Renders to `index.html`.

## Reproducing the Computational Environment

```sh
make docker-build      # one-time, builds the image
make r                 # interactive R session in container
make test              # run tinytest and testthat suites
make check-renv        # validate package dependencies
```

## Directory Structure

```
zzcollab-analysis-checklist/
|-- index.qmd                      (symlink -> analysis/report/index.qmd)
|-- figures/                       (symlink -> analysis/figures/)
|-- data/                          (symlink -> analysis/data/)
|-- analysis/
|   |-- data/
|   |   |-- raw_data/              (Item 5)
|   |   `-- derived_data/          (Items 22, 41)
|   |-- scripts/                   (Items 18, 23, 39)
|   |-- report/
|   |   `-- index.qmd              (the blog post body)
|   |-- figures/                   (Items 26, 31)
|   |-- media/images/              (hero, ambiance images)
|   `-- configs/
|-- docs/
|   |-- README.md                  (this file)
|   `-- analysis-checklist.qmd     (the deliverable artefact)
|-- R/                             (Items 9, 32-34)
|-- inst/tinytest/                 (Items 10-17, 35-38)
|-- tests/                         (testthat suites)
|-- DESCRIPTION                    (Items 46-48)
|-- Dockerfile                     (Item 1)
|-- renv.lock                      (Item 2)
|-- .Rprofile                      (Item 3)
|-- Makefile
`-- zzcollab.yaml
```

Each numbered annotation maps to a checklist item; reading
the directory structure alongside `analysis-checklist.qmd`
shows how the items relate to artefacts on disk.

## License

GPL-3, consistent with the parent zzcollab framework.
