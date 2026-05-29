# Adding an Image to the Visual Gallery

The Visual Gallery (`/visual-gallery/`) showcases SBOL Visual diagrams from published manuscripts. Each image has its own folder containing the image file, a short `index.md`, and optionally a `cite.bib` file for automatic citation parsing.

---

## Where the files live

```
content/visual-gallery/
└── your-image-slug/
    ├── index.md
    ├── image.png      ← the diagram (also .jpg, .jpeg, .gif, .webp, .svg)
    └── cite.bib       ← optional but recommended
```

The folder name becomes the URL slug — use a short identifier from the paper (e.g. the DOI suffix or first author + year).

---

## Step-by-step

### With a BibTeX file (recommended)

1. Create a new folder inside `content/visual-gallery/`.
2. Add the diagram image (any common image format).
3. Add `cite.bib` with the BibTeX entry for the paper.
4. Add `index.md` with just the title, DOI, and publication URL — everything else is read from the `.bib` file automatically.

### Without a BibTeX file

Provide all fields directly in the `index.md` front matter instead.

---

## Template (with cite.bib — recommended)

**`index.md`**
```markdown
---
title: "Full title of the paper this image is from"
doi: "10.1021/acssynbio.1c00281"
publication_url: "https://pubs.acs.org/doi/10.1021/acssynbio.1c00281"
---
```

**`cite.bib`**
```bibtex
@article{yourkeyhere,
  title={Full paper title},
  author={Last, First and Second, Author},
  journal={Journal Name},
  volume={10},
  number={12},
  pages={3330--3342},
  year={2021},
  publisher={Publisher Name}
}
```

The site automatically extracts `author`, `year`, `journal`, and `doi` from the `.bib` file. The `doi` in `index.md` takes priority over the `.bib` if both are present.

---

## Template (without cite.bib)

```markdown
---
title: "Full title of the paper"
credit: "Last Name, First Name and Second Author"
year: 2021
publication: "ACS Synthetic Biology"
doi: "10.1021/acssynbio.1c00281"
publication_url: "https://pubs.acs.org/doi/10.1021/acssynbio.1c00281"
---

Optional caption describing what the diagram shows.
```

---

## Real example

`content/visual-gallery/sb1c00281/`

```
sb1c00281/
├── index.md
├── image.jpeg
└── cite.bib
```

`index.md`:
```markdown
---
title: "Predicting composition of genetic circuits with resource competition: demand and sensitivity"
doi: "10.1021/acssynbio.1c00281"
publication_url: "https://pubs.acs.org/doi/10.1021/acssynbio.1c00281"
---
```

`cite.bib`:
```bibtex
@article{mcbride2021predicting,
  title={Predicting composition of genetic circuits with resource competition: demand and sensitivity},
  author={McBride, Cameron D and Del Vecchio, Domitilla},
  journal={ACS Synthetic Biology},
  volume={10},
  number={12},
  pages={3330--3342},
  year={2021},
  publisher={ACS Publications}
}
```

---

## Field reference (index.md)

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Full paper title. Shown in the card and lightbox |
| `doi` | Recommended | DOI string only, without `https://doi.org/`. Shown as a link in the lightbox |
| `publication_url` | Recommended | Full URL to the paper. Used for the "View Publication" button |
| `credit` | No | Override for author attribution if not using `cite.bib` |
| `year` | No | Override for year if not using `cite.bib` |
| `publication` | No | Override for journal name if not using `cite.bib` |

The body of `index.md` (below the closing `---`) is used as a caption in the lightbox.

---

## Common mistakes

- **Image not found** — the image must be in the same folder as `index.md`. The gallery picks up the first image file it finds (`*.jpg`, `*.jpeg`, `*.png`, `*.gif`, `*.webp`, `*.svg`).
- **`.bib` file not parsed** — the parser reads the `.bib` file line by line. Make sure each field (`author`, `year`, `journal`, `doi`) is on its own line in standard BibTeX format.
- **`authors` as a field name** — do not use `authors` in the front matter. Wowchemy reserves that field and expects a list; using it as a string causes a build error. Use `credit` instead.
