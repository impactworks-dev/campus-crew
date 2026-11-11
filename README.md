# Campus Crew

Landing pages for four student text agents, built for the UNCW pilot (fall 2026 to summer 2027). Static sites, no build step, no ClickUp dependency.

| Folder | Agent | Launch window | Live path |
|---|---|---|---|
| `escape-room/` | Syllabus Escape Room | Nov 30 to Dec 10, 2026 (finals) | `/escape-room/` |
| `side-quest/` | Side Quest | Jan 8, 2027 (welcome back) | `/side-quest/` |
| `forgotten-refund/` | The Forgotten Refund | Jan 11 to Feb 5, 2027 (trial purge) | `/forgotten-refund/` |
| `move-out-flip/` | UNCW Move-Out Flip | Sellers Mar 8, pickups Apr 30 to May 7, 2027 | `/move-out-flip/` |

The root `index.html` is a simple hub linking to all four.

## Structure

```
campus-crew/
├── index.html            hub page
├── .nojekyll             tells GitHub Pages to serve files as-is
├── escape-room/
│   ├── index.html        the page (single-file build)
│   └── assets/           floater.webp, still.webp, grain.png
├── side-quest/           same layout
├── forgotten-refund/     same layout
├── move-out-flip/        same layout
└── docs/
    └── launch-plan.md    Campus Crew ambassador plan summary
```

## Turn on GitHub Pages

1. Settings, Pages.
2. Source: Deploy from a branch. Branch: `main`, folder `/ (root)`. Save.
3. Live at `https://impactworks-dev.github.io/campus-crew/` within a minute or two.
4. Custom domain later: add it under Settings, Pages, and point a CNAME record at `impactworks-dev.github.io`.

## Updating a page

Pages are designed and edited in ClickUp, then exported. To ship a change: export the new build, replace that folder's `index.html` (and `assets/` if images changed), commit.

## Before launch

- Signup buttons currently open a pre-filled email to dante@impactworks.com. Swap to the real signup form once it exists.
- All chats, prices and stats on the pages are sample content.
- Move-Out Flip is not affiliated with UNCW. Keep that line in the footer.
