# Selvakumar KS — Product Engineering Portfolio (GitHub Pages)

## Folder structure — keep this exact layout
```
portfolio-site/
├── index.html
├── README.md
└── assets/
    ├── headshot.jpg
    ├── case-studies/
    │   ├── cs01-thumb.jpg   cs01-full.jpg
    │   ├── cs02-thumb.jpg   cs02-full.jpg
    │   ├── cs03-thumb.jpg   cs03-full.jpg
    │   ├── cs04-thumb.jpg   cs04-full.jpg
    │   ├── cs05-thumb.jpg   cs05-full.jpg
    │   └── cs06-thumb.jpg   cs06-full.jpg
    └── achievements/
        ├── tech-talk.jpg
        ├── magazine.jpg
        └── connected-manager.jpg
```
`index.html` references images via these exact relative paths (e.g. `assets/case-studies/cs01-thumb.jpg`),
so the folders must be uploaded to GitHub with this structure intact — not flattened.

## Publishing on GitHub Pages — folder-safe method

GitHub's "Choose your files" button only lets you pick individual files, which is why folders
got flattened last time. To upload real folders, you must **drag the folder icon itself** from
your computer's file explorer into the browser — do not click into the folder and select files
from inside it.

1. On your repo page, click **Add file → Upload files**.
2. Open the unzipped `portfolio-site` folder in a separate File Explorer / Finder window, arranged
   so you can see both it and the browser at once.
3. Drag `index.html` and `README.md` into the browser's drop zone — these are single files, so a
   normal drag works.
4. Now drag the **`assets` folder itself** (the folder icon, not its contents) from File Explorer /
   Finder directly onto the same drop zone. Modern Chrome/Edge/Firefox read the whole folder tree
   when you drop a folder this way, including the `case-studies` and `achievements` subfolders
   inside it.
5. Wait a few seconds — GitHub will list out every nested file it found before you commit. Scroll
   through and confirm you see all of: `headshot.jpg`, `case-studies/cs01-thumb.jpg` ... `cs06-full.jpg`,
   `achievements/tech-talk.jpg`, `magazine.jpg`, `connected-manager.jpg` (12 + 3 + 1 = 16 image files
   total, nested under `assets/`).
6. Scroll down, click **Commit changes**.

If dragging the folder doesn't work in your browser, the reliable fallback is **GitHub Desktop**:
install it, clone the empty repo to your computer, copy the `portfolio-site` folder's contents
directly into the cloned folder on disk (via File Explorer, so the nested structure is preserved
automatically), then use GitHub Desktop to commit and push. No drag-and-drop finickiness that way.

## Enable Pages

**Settings → Pages → Build and deployment → Source → Deploy from a branch → main → / (root) → Save.**
(If you deleted and recreated the repo, this setting resets and needs to be done again.)

Live at: `https://selvakumar-ks.github.io/`
