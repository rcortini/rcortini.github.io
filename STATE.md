# Site Restructure — State Summary
_Last updated: 2026-04-23_

## What was done

### Files modified
| File | Change |
|------|--------|
| `_quarto.yml` | New navbar (Home, About, Projects, Personal dropdown, CV); removed `brand` theme layer |
| `index.qmd` | Rewritten as professional landing page with CTA buttons and "What I do" section |
| `about.qmd` | Structured bio with placeholder tables for education, skills |
| `styles.css` | Added minimal CSS: navbar padding, gallery spacing, map caption styling |

### Files created
| File | Purpose |
|------|---------|
| `cv.qmd` | Styled HTML CV with "Download PDF" button; placeholder sections |
| `projects/index.qmd` | Quarto listing page — auto-generates cards from `projects/*.qmd` |
| `projects/oa_time.qmd` | Moved from root; added YAML front matter (title, date, description, categories) |
| `personal/photography/index.qmd` | Lightbox gallery template (placeholder, commented-out example) |
| `personal/maps/index.qmd` | Large captioned images template (placeholder, commented-out example) |
| `personal/coc/index.qmd` | Text + PDF download button (placeholder content) |

---

## What's pending (content you need to provide)

### High priority (visible to recruiters)
- [ ] **CV content** — fill in Experience and Education sections in `cv.qmd`
- [ ] **CV PDF** — export your CV as PDF, save to `assets/cv.pdf`
- [ ] **About narrative** — replace placeholder text in `about.qmd` with your own bio
- [ ] **Home tagline** — review and personalise the one-liner in `index.qmd`
- [ ] **`oa_time.qmd` content** — the project card renders but the page body is mostly placeholder; add the actual analysis

### Medium priority
- [ ] **Projects** — add more `*.qmd` files to `projects/` (each needs `title`, `date`, `description`, `categories` in its YAML front matter to show as a card)
- [ ] **Photography** — add images to `assets/photography/`, then uncomment and populate the gallery template in `personal/photography/index.qmd`
- [ ] **Fantasy maps** — add images to `assets/maps/`, then uncomment and populate `personal/maps/index.qmd`
- [ ] **Call of Cthulhu** — write campaign text in `personal/coc/index.qmd`; add PDF to `assets/coc/campaign.pdf`

### Housekeeping
- [ ] Delete root-level `oa_time.qmd` once you confirm `projects/oa_time.qmd` renders correctly (the root file is superseded but not yet deleted)
- [ ] Verify `quarto render` completes without errors after the restructure
- [ ] Push `docs/` to GitHub Pages

---

## Decisions made (for future reference)

- **Theme:** `cosmo` — clean, Bootstrap 5 base, recruiter-readable; `brand` layer removed (no `_brand.yml` existed)
- **Projects listing:** auto-generated via Quarto `listing`, grid layout sorted by date; add front matter to any `.qmd` in `projects/` to get a card
- **Photography:** uses Quarto's built-in `lightbox: true` — no extension required
- **CV:** styled HTML page at `cv.qmd` + download button pointing to `assets/cv.pdf`
- **Personal pages:** one dropdown click deeper from nav — visible but not leading
