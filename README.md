# NCS — Standalone Timeline Demo

A fully self-contained demo of the NCS project timeline ("Wayfinder — Trail Companion App").
No build step, no server required.

**Live:** <https://ncs-timeline-demo.vercel.app> · featured-designer flow at
[/?flow=featured](https://ncs-timeline-demo.vercel.app/?flow=featured)

To run locally, serve the folder with any static server:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/ncs-timeline-standalone.html
```

(Prefer a served URL over double-clicking the file — some browsers give `file://` pages
ephemeral storage, so demo state may not survive a refresh.)

## What's in the demo

- The project timeline: iterations with images, changes notes, inspired-by citations
- **Share modal (two tiers, Figma-style)** — via the **+ pill → Collab**:
  - *Invite to collaborate* — private `#invite-<token>` link with expiry (1h / 24h / 7d / 30d / none), full edit access
  - *View-only link* — react and comment, never edit
- **Featured-designer flow** (`?flow=featured`) — NCS collected the designer's final; the
  **ready-to-feature onboarding guide** walks the claim: numbered self-ticking steps pinned
  above the beats (confirm it's yours → add process, with inline examples → say what
  changed → publish No. 001), foldable to a slim bar, aggregate-progress flag in the toolbar
- **Share update** — the frozen, numbered update-note flow (preview is the picker; Publish vs quiet Copy link)
- Unified **Respond** button, Media / Text / Collab add menu, discussion rail, appreciation marks

Everything (fonts, styles, logic) is inlined in the single HTML file; the only external
assets are the demo images in `demo-pics/` (referenced relatively) and dicebear.com avatars.

## Provenance

Snapshot of `public/ncs-timeline-standalone.html` from the NCS-REAL working tree as of
2026-07-24 (`feat/collab-invites @ 940b711`, local) — includes the two-tier share modal
work that post-dates
[cocreateteam/NCS-REAL PR #39](https://github.com/cocreateteam/NCS-REAL/pull/39), plus the
featured-flow onboarding guide from the 2026-07-24 feedback round.
