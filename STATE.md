# Site State
_Last updated: 2026-04-23_

## What's complete

| Page | Status |
|------|--------|
| `index.qmd` | Done — professional landing page |
| `about.qmd` | Done — real bio, education, skills |
| `cv.qmd` | Done — fully populated from real CV |
| `projects/index.qmd` | Done — auto-listing, 4 cards |
| `projects/oa_time.qmd` | Done — content + analysis written by you |
| `projects/barcelona_edificacions.qmd` | Done — content + analysis written by you |
| `projects/aigues_catalunya.qmd` | Done — content written |
| `projects/eua_observatory.qmd` | Done — case study page |
| `personal/photography/index.qmd` | Done — 4 photos with lightbox captions |
| `personal/maps/index.qmd` | Done — 3 maps with captions |
| `personal/coc/index.qmd` | Done — fully written, links to DriveThruRPG |
| `README.md` | Done |

---

## To-do next session

### Must-do before publishing
- [ ] **Add `assets/cv.pdf`** — the Download PDF button on the CV page is live but the file doesn't exist yet. Export your CV as a PDF and drop it there.
- [ ] **Commit and push to GitHub** — nothing has been committed since the restructure. Run `quarto render` first to rebuild `docs/`, then commit and push.

### Quick fixes
- [ ] **Remove stale comment block** from `personal/photography/index.qmd` lines 23–30 (the old placeholder template inside `<!-- -->`; the gallery is live and those lines are dead weight).
- [ ] **Add fourth map** — `assets/maps/State_of_Kazam.jpg` is in the repo but not shown in `personal/maps/index.qmd`. Add a `.map-entry` block for it.
- [x] **Update `index.qmd` Selected Projects** — all four projects now listed.

### Content to add when ready
- [ ] **More photography** — gallery structure is proven; just add images to `assets/photography/` and append new entries to the layout block (remember: blank line between each, `.lightbox` class, unique `#fig-` id).
- [ ] **Project dates** — `barcelona_edificacions` (2026-01-01) and `eua_observatory` (2025-02-01) use placeholder dates. Correct them to reflect when you actually built them; this affects sort order in the listing.
- [ ] **New projects** — any future project gets a `.qmd` in `projects/` with `title`, `date`, `description`, and `categories` front matter; it appears in the listing automatically.
