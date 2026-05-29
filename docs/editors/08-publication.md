# Adding a Publication

Publications appear on the **Publications** page (`/publication/`). Each publication has its own folder containing a BibTeX file and an `index.md`.

---

## Where the files live

```
content/publication/
└── firstauthor-shorttitle-year/
    ├── index.md
    └── cite.bib
```

Use a descriptive slug for the folder name — the convention in this repo is `firstauthor-keyword-year` (e.g. `mcbride-resource-competition-2021`). Keep it lowercase and hyphenated.

---

## Step-by-step

1. Create a new folder inside `content/publication/`.
2. Add `cite.bib` with the BibTeX entry.
3. Add `index.md` with the front matter below.

---

## Template

**`cite.bib`**
```bibtex
@article{yourkeyhere,
  title={Full paper title},
  author={Last, First and Second, Author},
  journal={Journal Name},
  volume={10},
  number={4},
  pages={1234--1250},
  year={2026},
  publisher={Publisher Name},
  doi={10.xxxx/xxxxxxx}
}
```

**`index.md`**
```markdown
---
title: "Full paper title"
date: "2026-06-01T00:00:00Z"
authors:
  - First Last
  - Second Author
publication: "*Journal Name*, vol. 10, no. 4"
publication_types:
  - "2"             # see publication types below
abstract: "Paste the abstract here."
featured: false
url_pdf: ""         # direct link to PDF if openly available
doi: "10.xxxx/xxxxxxx"
---
```

---

## Real example

`content/publication/appleton-interactive-2014/`

`cite.bib`:
```bibtex
@article{appleton2014interactive,
  title={Interactive assembly algorithms for molecular cloning},
  author={Appleton, Evan and Tao, Jenhan and Haddock, Traci and Densmore, Douglas},
  journal={Nature Methods},
  volume={11},
  number={6},
  pages={657--662},
  year={2014},
  publisher={Nature Publishing Group}
}
```

`index.md`:
```markdown
---
title: "Interactive assembly algorithms for molecular cloning"
date: "2014-06-01T00:00:00Z"
authors:
  - Evan Appleton
  - Jenhan Tao
  - Traci Haddock
  - Douglas Densmore
publication: "*Nature Methods*, vol. 11, no. 6"
publication_types:
  - "2"
abstract: ""
featured: false
doi: ""
---
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Full paper title |
| `date` | Yes | Publication date in ISO 8601 format |
| `authors` | Yes | List of author full names as plain strings |
| `publication` | Yes | Journal name in italics using `*asterisks*`, plus volume/issue if known |
| `publication_types` | Yes | List with a single type code (see below) |
| `abstract` | No | Paper abstract. Can be left blank |
| `featured` | No | Set to `true` to feature the paper prominently |
| `url_pdf` | No | Direct link to a PDF. Leave blank if not openly available |
| `doi` | No | DOI string only, without `https://doi.org/` |

### Publication type codes

| Code | Meaning |
|---|---|
| `"1"` | Conference paper |
| `"2"` | Journal article |
| `"3"` | Preprint |
| `"4"` | Report |
| `"5"` | Book |
| `"6"` | Book chapter |
| `"7"` | Thesis |

---

## Common mistakes

- **Missing `cite.bib`** — both files are required. The BibTeX file is used by the "Cite" button on the publication page.
- **Authors as slugs** — unlike blog posts, publication `authors` are plain name strings, not slugs from `content/authors/`. Write the full name as it should appear.
- **Wrong date format** — use the full ISO 8601 format including time: `"2026-06-01T00:00:00Z"`.
