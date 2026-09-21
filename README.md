# Selvakumar KS — Product Engineering Portfolio (GitHub Pages)

## Folder structure — keep this exact layout
```
portfolio-site/
├── index.html
├── README.md
└── assets/
    ├── headshot.jpg
    ├── case-studies/   (7 pairs of -thumb.jpg / -full.jpg, all watermarked)
    └── achievements/   (tech-talk.jpg, magazine.jpg, connected-manager.jpg)
```

## Publishing on GitHub Pages — folder-safe method
1. Repo page → **Add file → Upload files**.
2. Drag `index.html` and `README.md` in as individual files.
3. Drag the **`assets` folder itself** onto the same drop zone (preserves subfolders).
4. Confirm GitHub lists all nested files, then **Commit changes**.

Fallback: GitHub Desktop — clone, copy folder contents on disk, commit + push.

## Enable Pages
**Settings → Pages → Deploy from a branch → main → / (root) → Save.**
Live at: `https://selvakumar-ks.github.io/`

## What's new — CS-07 added
A 7th case study: "Engineering Calculation Automation — Python Tools", featuring the two custom
Python/Tkinter desktop calculators (Shelf Deflection, Cabinet Stability & Tip-Over). The hero
stat and section heading were updated from six to seven case studies.

## Image protection & redactions
- All 7 case-study images carry a bold repeating diagonal "SELVAKUMAR KS" watermark plus a
  corner credit mark.
- CS-01: coworker name + project date redacted; Tolerance Chain and Calculation Table diagrams
  blanked out with a "confidential" placeholder.
- CS-02: the three Creo 3D Model renders converted to black-line wireframe drawings.
- CS-06: client name + coworker names redacted across chart labels and the delivery table.
- Connected Manager certificate (achievements folder): two senior leaders' names redacted.
- Right-click-save and drag-out disabled site-wide (casual deterrent only).

## Editing later
Sections have clear `id`s — search `index.html` by heading text to find and edit any section.
