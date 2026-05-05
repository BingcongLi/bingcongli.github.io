# Personal Website — Bingcong Li

## File Structure

```
your-site/
├── index.html              ← main website (do not edit unless changing layout)
└── content/
    ├── photo.png           ← your profile photo (sidebar)
    ├── logo.png            ← your logo (browser tab favicon)
    ├── about.md            ← About tab: bio + research thrusts
    ├── news.md             ← About tab: Recent News + Old News
    ├── background.md       ← Background tab: education, experience, awards
    ├── publications.md     ← Publications tab
    ├── mentoring.md        ← Teaching & Mentoring tab
    ├── service.md          ← Service tab: talks, workshops, reviewer
    └── notes.md            ← Research Notes tab
```

---

## How to Run Locally

Browsers block local file fetches, so you need a simple server:

```bash
# Option 1 — Python (no install needed)
cd your-site
python3 -m http.server
# then open http://localhost:8000

# Option 2 — VS Code
# Install the "Live Server" extension → right-click index.html → Open with Live Server
# It auto-refreshes whenever you save a markdown file.
```

---

## How to Edit Content

All content lives in the `content/` folder as plain markdown files.  
**You never need to touch `index.html`** unless you want to change the layout.

### Add a news item
Open `content/news.md`. Each item is a bullet:
```markdown
- **MM/YYYY.** Your news text here. [Optional link](https://url)
```
Paste new items at the top of `# Recent News`.  
Move old items to `# Old News` to archive them.

---

### Add a publication
Open `content/publications.md`. Each entry follows this format:
```markdown
**Title of the paper.**
Author One, **Bingcong Li**, Author Three.
*Proc. of Conference Name* (**ABBREV**), Year.
[[Paper](https://arxiv-or-pdf-url)] [[Code](https://github-url)]

---
```
- Your name must be wrapped in `**double asterisks**` to appear bold.
- `[[Paper](url)]` renders as a pill button. Add `[[Code](url)]`, `[[Slides](url)]` etc. as needed.
- Paste new entries at the top of `## Conference Papers`.

---

### Add a mentee
Open `content/mentoring.md`. Each entry:
```markdown
**Name** · Institution, Period
Topic of supervision.
*Outcome (e.g. NeurIPS 2025)*
```
Place under the correct section: `## Ph.D. Researchers`, `## Master Students`, or `## Bachelor Students`.

---

### Add a talk or workshop
Open `content/service.md`.

**Invited Talk:**
```markdown
**Talk Title**
Venue 1, City · *Month Year*
Venue 2, City · *Month Year*
```

**Workshop:**
```markdown
**Workshop Title**
Venue, City, Month Year
```

---

### Add a research note
Open `content/notes.md`. Same format as publications:
```markdown
**Note title.**
*One-line description.*
[[Read](https://url)]

---
```

---

## Sidebar Info

The sidebar (name, title, contact links) is hardcoded in `index.html`.  
To update it, open `index.html` and find this block (~line 330):

```html
<div class="sidebar-name">Bingcong Li</div>
<div class="sidebar-title">
  Postdoctoral Researcher<br>
  Dept. of Computer Science<br>
  ETH Zürich
</div>
<div class="sidebar-contact">
  <a href="mailto:...">bingcong.li[@]inf.ethz.ch</a><br>
  ...
</div>
```

---

## Photos & Logo

| File | Used for |
|---|---|
| `content/photo.png` | Profile photo in sidebar |
| `content/logo.png` | Browser tab favicon |

To update either, just replace the file — keep the same filename.

---

## Deployment (GitHub Pages)

1. Create a repo named `bingcongli.github.io` on GitHub
2. Push the entire folder (index.html + content/) to the `main` branch
3. Go to **Settings → Pages → Source: main branch / root**
4. Your site is live at `https://bingcongli.github.io`

To update: edit any `.md` file, commit, and push — the site updates automatically.

---

## Tab Overview

| Tab | Source file | Notes |
|---|---|---|
| About | `content/about.md` + `content/news.md` | Bio, thrusts, Recent/Old News sub-tabs |
| Background | `content/background.md` | Education, experience, awards |
| Publications | `content/publications.md` | Conference papers + journal articles |
| Teaching & Mentoring | `content/mentoring.md` | Teaching + PhD/Master/Bachelor mentees |
| Service | `content/service.md` | Tutorials, workshops, talks, reviewer |
| Research Notes | `content/notes.md` | Informal notes, blog post links |

---

## Tips

- **Markdown renders live** — save the file, refresh the browser.
- **`---` in publications.md** separates entries visually (the renderer removes the line).
- **Bold your name** in every author list: `**Bingcong Li**`
- **Equal contribution**: use `**Bingcong Li**\*` (the `\*` renders as a literal asterisk).
- The `*italic*` date line at the end of a mentoring entry is detected automatically and styled as a small gray date.
