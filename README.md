# Peppermint Academy

Product documentation, service guides, and training video hub for Peppermint Robotics platforms.

Live site: `https://anishsambhus-sudo.github.io/peppermint-academy/` (enable in repo **Settings → Pages** if not live yet)

## Structure

Each product has its own folder with three subfolders:

```
<product>/
├── index.html   (product landing page)
├── user/        (operating & setup guides)
├── service/     (maintenance & repair guides)
└── videos/      (training videos, or links to hosted video)
```

## Adding a new product

1. Copy `_template.html` into a new folder as `<slug>/index.html`
2. Replace `__NAME__`, `__TAGLINE__`, and `__SLUG__` in that file
3. Create `<slug>/user/`, `<slug>/service/`, `<slug>/videos/` subfolders
4. Add a card for it on the homepage (`index.html`)
5. Commit and push — the live site updates automatically

## Adding docs/videos to an existing product

Just drop files into the relevant `user/`, `service/`, or `videos/` folder, then:

```bash
git add .
git commit -m "Add <product> <doc type>"
git push
```

Large video files are better linked from Google Drive/YouTube than stored directly in the repo — GitHub has a 100MB per-file limit.
