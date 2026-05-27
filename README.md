# Transferable RL — ICML 2026 Project Page

Project webpage for *"Transferable Reinforcement Learning via Probabilistic Latent Embeddings and Dynamic Policy Adaptation for Sim-to-Real Deployment"*.

- **Repo**: <https://github.com/HGY-SEU/Transfer-RL-web>
- **Live site** (after Pages is enabled): <https://hgy-seu.github.io/Transfer-RL-web/>

## Local preview

Just double-click `index.html` — it opens in your default browser. No server needed. Local preview deliberately skips all external analytics calls (counter + visitor globe) so loading stays instant.

## File layout

```text
webpage/
├── index.html              ← all content lives here
├── README.md
└── static/
    ├── css/custom.css      ← all styling
    ├── js/index.js         ← animations, theme toggle, BibTeX copy, analytics injection
    ├── videos/demo.mp4     ← demo video for PointGoal2
    └── images/
        ├── teaser.png      (Figure 1 — Sim2Real gap illustration)
        ├── method.png      (Figure 2 — framework overview)
        ├── f5_exp.png      (PointGoal2 task scene)
        ├── f6_platoon.png  (Autonomous Driving platoon)
        ├── f3a_cost.png    (left analysis card)
        ├── f4a_cost_bar.png, f4b_reward_bar.png  (right analysis card)
        ├── purdue_logo.svg, icml_logo.svg
        └── (other unused: cost.png, platoon.png, results.png, f3b_reward.png)
```

## Places to update later

Search `index.html` for `UPDATE:` — three spots:

| What | Find | Replace with |
|---|---|---|
| Paper PDF button | `<!-- UPDATE: arXiv PDF link ...` | `https://arxiv.org/pdf/XXXX.XXXXX` (then change `<button data-modal="paperModal">` to `<a href="...">`) |
| arXiv button    | `<!-- UPDATE: arXiv abstract page ...` | `https://arxiv.org/abs/XXXX.XXXXX` |
| Code button     | `<!-- UPDATE: code repo link ...` | `https://github.com/<you>/<paper-code-repo>` (and change `<button data-modal="codeModal">` to `<a href="...">`) |

Also update the BibTeX inside `<pre id="bibtexCode">` once you have an official PMLR page/pages range.

## Analytics (already configured)

Both run **only** after page load AND only on `http(s)` — local previews stay 100% offline.

- **Page-view counter** (hits.seeyoufarm) — counts the deployed URL automatically, no setup.
- **Visitor globe** (ClustrMaps 3D globe) — keyed to your site via `CLUSTRMAPS_KEY` in `static/js/index.js`. Already wired with:
  `dZsiTLFFKTSJFfI7pO9rqarYVwaLYDc_iv3vs9aXpgo`

## Deploy to GitHub Pages

Your repo `HGY-SEU/Transfer-RL-web` is already created. To go live:

1. Upload the contents of this `webpage/` folder (drag `index.html`, `README.md`, and the entire `static/` folder) into the repo via the GitHub web UI's **Add file → Upload files** → commit.
2. Repo → **Settings** → **Pages** → Source: `Deploy from a branch`, Branch: `main` / `(root)` → **Save**.
3. Wait ~1 min → site live at <https://hgy-seu.github.io/Transfer-RL-web/>.
