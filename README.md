# Selvakumar KS — Product Engineering Portfolio (GitHub Pages)

## Folder structure — keep this exact layout
```
portfolio-site/
├── index.html
├── README.md
└── assets/
    ├── headshot.jpg
    ├── case-studies/   (6 pairs of -thumb.jpg / -full.jpg, all watermarked)
    └── achievements/   (tech-talk.jpg, magazine.jpg, connected-manager.jpg)
```
`index.html` references images via exact relative paths — upload with this structure intact.

## Publishing on GitHub Pages — folder-safe method
1. Repo page → **Add file → Upload files**.
2. Drag `index.html` and `README.md` in as individual files.
3. Drag the **`assets` folder itself** (the folder icon, not its contents) onto the same drop zone —
   this is what preserves the `case-studies/` and `achievements/` subfolders.
4. Confirm GitHub lists all nested files before committing.
5. **Commit changes.**

Fallback if folder-drag doesn't work in your browser: use **GitHub Desktop**, clone the repo, copy
the folder contents directly on disk, then commit + push from the app.

## Enable Pages
**Settings → Pages → Deploy from a branch → main → / (root) → Save.**
Live at: `https://selvakumar-ks.github.io/`

## Image protection
- All 6 case-study images (thumb + full) carry a repeating diagonal "SELVAKUMAR KS" watermark plus
  a corner credit mark — sized to stay visible even at the smaller in-page display size, not just
  at full resolution.
- Known-sensitive content already redacted: coworker name + date in CS-01; client name + coworker
  names across several chart labels and the delivery table in CS-06.
- Right-click-save and drag-out are disabled on all images site-wide (casual deterrent only).

## Editing later
Sections have clear `id`s (`#profile`, `#competencies`, `#experience`, `#case-studies`,
`#achievements`, `#contact`) — search `index.html` by heading text to find and edit any section.
Colors/type live in the `:root` CSS variables near the top of the file.
