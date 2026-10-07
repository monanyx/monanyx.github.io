# monanyx.github.io

My first portfolio site: a small pixel-art platformer where each biome is a section of my CV.

**Live:** https://monanyx.github.io

| Zone | Section |
| --- | --- |
| 🌙 Spawn | Home |
| 🌿 Overworld | About me |
| ⛏ Deep Cave | Experience |
| 🔥 The Nether | Projects |
| 💎 Deep Ocean | Skills (you can swim here) |
| 👁 The End | Certifications |
| 📚 Stronghold | Education |
| 📡 Beacon | Contact |

Walking into a zone opens its info panel. There are 16 XP orbs hidden on platforms across the world. Collect them all for an achievement.

## Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Move | `A` / `D` or `←` / `→` | ◀ ▶ |
| Jump / swim up | `W`, `↑` or `Space` | ▲ |
| Drop through a platform | `S` or `↓` | ▼ |
| Fast travel | `1` – `8` or click the hotbar | tap the hotbar |
| Open zone info | `E` | tap the yellow prompt |
| Close info | `Esc` | ✕ CLOSE |
| Music on/off | `M` | menu button |

## Run it locally

Everything is in `index.html`, with no build step. Open it in a browser, or serve the folder:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

Every push to `main` runs `.github/workflows/static.yml`, which publishes the repo to GitHub Pages.

## Editing the content

The text for every panel is in the `PANEL_CONTENT` object near the bottom of `index.html`. The level layout (decorations, platforms and orbs, per zone) is in `buildLevel()`.
