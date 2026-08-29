# mrulis.github.io

Source for <https://mrulis.github.io>, the academic website of Mina Rulis.

Built with [al-folio](https://github.com/alshedivat/al-folio), a Jekyll theme
for academic sites. Every push to `main` starts a GitHub Actions build that
publishes to the `gh-pages` branch; the live site follows a few minutes later.

## Where things live

| To change this           | Edit this                                    |
| ------------------------ | -------------------------------------------- |
| Homepage bio             | `_pages/about.md`                             |
| Research page            | `_pages/research.md`                          |
| Teaching page            | `_pages/teaching.md`                          |
| CV                       | `assets/pdf/rulis_cv.pdf` (replace in place)  |
| Email and profile links  | `_data/socials.yml`                           |
| Headshot                 | `assets/img/headshot.jpg`                     |
| Site title and settings  | `_config.yml`                                 |

Publications, presentations, and courses are written directly into those pages
as HTML. They are not generated from `_bibliography/papers.bib`.

Unused theme pages — blog, projects, repositories, and others — remain in
`_pages/` marked `nav: false`, which keeps them out of the navigation bar.
