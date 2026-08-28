# mrulis.github.io

Academic website of Mina Rulis — https://mrulis.github.io

Built with [al-folio](https://github.com/alshedivat/al-folio), a Jekyll
theme for academic sites. Published automatically by GitHub Actions: every
push to `main` rebuilds the site and updates the live page within a few
minutes.

## Where things live

| To change this            | Edit this                        |
| ------------------------- | -------------------------------- |
| Homepage bio and photo    | `_pages/about.md`                |
| Publications              | `_bibliography/papers.bib`       |
| CV                        | `_data/cv.yml`                   |
| Teaching                  | `_teachings/` (one file per course) |
| Name, site title, address | `_config.yml`                    |
| Email and profile links   | `_data/socials.yml`              |
| Profile photo             | `assets/img/prof_pic.jpg`        |

Publications are generated from the BibTeX file — paste entries exported
from Google Scholar or Zotero into `_bibliography/papers.bib` and the
publications page updates itself. Mark an entry `selected={true}` to also
feature it on the homepage.

## Sections currently switched off

The blog, projects, repositories, people, and submenu pages still exist in
`_pages/` but are hidden from the navigation bar (`nav: false` in each
file's header). Set `nav: true` to bring one back.

## Reference

The theme's own documentation is kept in `docs/` — `docs/CUSTOMIZE.md` is
the most useful one.
