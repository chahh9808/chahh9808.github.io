# Website Editing Guide (Non-Technical)

This document explains where to edit content, how those edits appear on the site, and how to update safely without affecting production.

---

## 1) Most Frequently Edited Files

### Homepage layout and section content
- File: `content/_index.md`
- Purpose: controls homepage section order, titles, and text blocks
- Major visible sections include Bio, News, Projects, Publications, Professional Experiences, Leadership Experiences, Honors, and Skills

### Top navigation menu
- File: `config/_default/menus.yaml`
- Purpose: controls menu labels, order, and anchor links

### Main profile information
- File: `content/authors/admin/_index.md`
- Purpose: name, role, affiliation, social links, and long bio text

### Project cards on homepage
- Folder: `content/post/*/index.md`
- Purpose: each folder is one project card/page

### Publication cards on homepage
- Folder: `content/publication/*/index.md`
- Purpose: each folder is one publication card/page

### CV download file
- Path: `static/uploads/resume.pdf`
- Purpose: used by the homepage CV download button

---

## 2) Edit-to-UI Mapping

- `content/_index.md` with `id: news`
  - Updates the News section on homepage

- `content/_index.md` with `id: projects`
  - Updates the homepage Projects block
  - This block reads from `content/post`

- `content/_index.md` with `id: papers`
  - Updates the homepage Publications block
  - This block reads from `content/publication`

- `content/_index.md` with `id: professional-experience`
  - Updates Professional Experiences on homepage

- `content/_index.md` with `id: honors`
  - Updates Honors on homepage

- `config/_default/menus.yaml`
  - Updates top navigation text and anchor targets such as `/#projects`

---

## 3) Project Structure (Core)

```text
config/
  _default/
    hugo.yaml               # core Hugo config
    menus.yaml              # top navigation
    params.yaml             # theme and UI options

content/
  _index.md                 # homepage sections
  authors/admin/_index.md   # profile content
  post/*/index.md           # project pages/cards
  publication/*/index.md    # publication pages/cards

static/
  uploads/                  # static files (e.g., resume PDF)

assets/
  media/                    # site media assets

archive/
  unused-content/           # intentionally archived inactive content
```

---

## 4) Safe Update Workflow (No Production Impact)

### Principles
- Do not edit directly on `main`
- Work in a separate branch and verify locally first

### Recommended steps
1. Create a branch: `git switch -c chore/content-edit-YYYYMMDD`
2. Edit files
3. Run local preview
4. Commit changes
5. Optionally push the branch for preview checks
6. Merge into `main` only after final review

Production remains unchanged until merge/deploy.

---

## 5) Local Preview

Use project-compatible Hugo Extended for this repository.

### Run
```bash
cd /Users/hyeongheon/Documents/projects/chahh9808.github.io
.tools/hugo-0.126.1/hugo server -D --disableFastRender --bind 127.0.0.1 --port 1313
```

### Open in browser
- `http://127.0.0.1:1313/`

### Stop server
- Press `Ctrl + C` in the terminal

---

## 6) Common Mistakes to Avoid

- Use valid dates only
  - Example: avoid invalid dates like `2025-02-29`

- Keep YAML indentation with spaces
  - Do not use tabs

- Do not remove front matter separators (`---`)

- Keep full URL prefixes such as `https://`

- For large cleanup, archive first before permanent removal

---

## 7) Archived Inactive Content

The following files were moved to reduce confusion in active content folders:

- `archive/unused-content/content/projects.md`
- `archive/unused-content/content/experience.md`
- `archive/unused-content/content/event/example/index.md`
- `archive/unused-content/content/teaching/_index.md`
- `archive/unused-content/content/teaching/js/index.md`
- `archive/unused-content/content/teaching/python/index.md`
- `archive/unused-content/content/project/pandas/index.md`
- `archive/unused-content/content/project/pytorch/index.md`
- `archive/unused-content/content/project/scikit/index.md`

To restore, move files back under `content/` and re-enable build rendering if needed.

---

## 8) Quick Editing Recipes

### Add one News item
1. Open `content/_index.md`
2. Find the `id: news` block
3. Add one `<li>...</li>` entry
4. Save and refresh local preview

### Add a Project page/card
1. Create `content/post/<slug>/index.md`
2. Copy an existing project file as a template
3. Update title, summary, authors, tags, body
4. Add `featured.jpg` or `featured.png` in the same folder for thumbnail

### Add a Publication page/card
1. Create `content/publication/<slug>/index.md`
2. Copy an existing publication file as a template
3. Update title, authors, date, venue, abstract, tags, links
4. Add a featured image file in the same folder if needed

---

## 9) Content Style Recommendations

- Keep project and publication pages cross-linked when useful
- Match author order with the source paper metadata
- Prefer paper main figure for thumbnails when available
- Keep `Position` text up to date with your latest affiliation
- Keep homepage highlights (News and Honors) in sync with newly added pages

---

## 10) Current Notable Entries (Examples)

- SNAP project page: `content/post/snap/index.md`
- Beyond Hearing project page: `content/post/beyond-hearing/index.md`
- Beyond Hearing publication page: `content/publication/beyond-hearing/index.md`

Use these as up-to-date templates when creating new items.
