# Profile README — Setup Guide

## 📁 Repo structure

```
Ayanzadeh93/Ayanzadeh93/         ← your special-name profile repo
├── README.md                     ← this profile
├── assets/
│   ├── research-pipeline.svg    ← custom hand-designed pipeline diagram
│   └── terminal-card.svg        ← custom terminal-style intro card
└── .github/workflows/
    ├── snake.yml                ← daily snake animation
    └── 3d-contrib.yml           ← daily 3D contribution skyline
```

## 🚀 First-time setup

1. **Push everything** to your `Ayanzadeh93/Ayanzadeh93` repo (the one named after your username).
2. **Run both workflows once** from the Actions tab:
   - "Generate Snake Animation" → produces the `output` branch with snake SVGs
   - "Generate 3D Contribution Skyline" → produces `profile-3d-contrib/profile-night-rainbow.svg`
3. Both will re-run daily on their cron schedules.

## ✏️ Things to replace before pushing

| Placeholder | Replace with |
|---|---|
| `https://scholar.google.com/` | Your real Scholar URL with `?user=YOUR_ID` |
| Project descriptions | Add real arXiv / repo links once public |
| Publication entries | Add DOIs or arXiv IDs |

## 🎨 Editing the custom widgets

The pipeline diagram and terminal card are plain SVGs in `assets/`. You can edit them in any text editor — the colors follow the Tokyo Night palette:

- `#1a1b27` background
- `#7aa2f7` blue (Perception)
- `#bb9af7` purple (Representation)
- `#f7768e` red (Reasoning)
- `#9ece6a` green (Output / accept)
- `#c0caf5` foreground text
- `#565f89` dim text

## 🩺 Troubleshooting

- **Typing SVG not rendering** → already URL-encoded for safety; if you change the text, encode `·` → `%E2%80%A2`, `|` → `%7C`, `&` → `%26`.
- **Stats card shows error** → transient Vercel rate limit on `github-readme-stats`. Refresh in 1–2 min.
- **Snake / 3D-contrib not appearing** → make sure the workflow ran at least once in the Actions tab.
