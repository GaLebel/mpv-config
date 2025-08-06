# MPV Configuration Bindings & Scripts

## Key Bindings

| Keys           | Command                        | Description                                       |
|----------------|--------------------------------|---------------------------------------------------|
| `a` / `d`      | `sub-seek -1` / `sub-seek 1`   | Seek forward (a) / backward (d) to closest subtitle         |
| `UP`           | `add volume 2`                 | Increase volume by 2 units                        |
| `DOWN`         | `add volume -2`                | Decrease volume by 2 units                        |
| `Alt + UP`     | `no-osd add sub-pos -1`        | Move subtitles up one row (without OSD)           |
| `Alt + DOWN`   | `no-osd add sub-pos +1`        | Move subtitles down one row (without OSD)         |
| `RIGHT`        | `seek 1 exact`                 | Seek forward 1 second (exact)                     |
| `LEFT`         | `seek -1 exact`                | Seek backward 1 second (exact)                    |
| `Ctrl + RIGHT` | `seek +5`                      | Seek forward 5 seconds                            |
| `Ctrl + LEFT`  | `seek -5`                      | Seek backward 5 seconds                           |
| `y`            | `cycle audio`                  | Cycle through audio tracks                        |
| `SHIFT + q`    |  SimpleHistory command         | Save current video position                       |
| `h`            |  SimpleHistory command         | Show interactive recently played files menu       |
| `SHIFT + ?`    |  SmartSkip command             | Skip intro by detecting silence                   |

---

## Scripts Included

### SmartSkip  
Automatically or manually skip intros/outros/previews based on silence detection or chapters. Includes:
- **Smart Next / Prev** handlers  
- Skip silences when no chapters exist  
- Auto‑skip after configurable countdown  
- Chapter editing and baking tools with OSD feedback  
- Customizable via `script-opts/smartskip.conf`

📦 Source: [github.com/Eisa01/mpv-scripts](https://github.com/Eisa01/mpv-scripts)

---

### SimpleHistory  
Logs every media file you open along with the last playback position. Features:
- Automatically resume where you left off  
- View/search history  
- Works seamlessly in background

📦 Source: [brontosaurusrex.github.io](https://brontosaurusrex.github.io/2021/03/19/mpv-history-log/)

---

## Installation Instructions

1. Place your `input.conf` in:
   ```
   ~/.config/mpv/input.conf
   ```
2. Download the scripts:
   - `smartskip.lua` and `simplehistory.lua` → `~/.config/mpv/scripts/`
   - Optional `.conf` files → `~/.config/mpv/script-opts/`

3. Restart mpv and enjoy enhanced controls!
```




