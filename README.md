# NCS — Standalone Timeline Demo

A fully self-contained demo of the NCS project timeline ("Wayfinder — Trail Companion App").
No build step, no server required: open `ncs-timeline-standalone.html` directly in a browser,
or serve the folder with any static server.

```bash
python3 -m http.server 8000
# then open http://localhost:8000/ncs-timeline-standalone.html
```

## What's in the demo

- The project timeline: iterations with images, changes notes, inspired-by citations
- **Share modal (two tiers, Figma-style)** — via the **+ pill → Collab**:
  - *Invite to collaborate* — private `#invite-<token>` link with expiry (1h / 24h / 7d / 30d / none), full edit access
  - *View-only link* — react and comment, never edit
- **Share update** — the frozen, numbered update-note flow (preview is the picker; Publish vs quiet Copy link)
- Unified **Respond** button, Media / Text / Collab add menu, discussion rail, appreciation marks

Everything (fonts, styles, logic) is inlined in the single HTML file; the only external
assets are the demo images in `demo-pics/` (referenced relatively) and dicebear.com avatars.

## Provenance

Snapshot of `public/ncs-timeline-standalone.html` from the NCS-REAL working tree as of
2026-07-21 — includes the two-tier share modal work that post-dates
[cocreateteam/NCS-REAL PR #39](https://github.com/cocreateteam/NCS-REAL/pull/39).
