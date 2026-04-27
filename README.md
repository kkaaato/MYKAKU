# MYKAKU — Memory Match Lobby

**Repository for Programming 2 Finals Project**

**Programmer:** Kavin Karl C. Molos & Kurt Michael D. Yalung
**Course:** BSIT-GD 1st Year

---

## Game Title & Description

**Memory Match Lobby** is a browser-based game hub featuring two distinct memory challenge games:

### 🟠 Game 01 — Shuffling Memory Match
A 2-player turn-based card matching game played on a 6×4 grid of face-down cards. Players take turns flipping pairs of cards to find matching symbols. The twist: every time a player fails to find a match, the 4 cards from the last 2 guesses **shuffle positions**, making the board increasingly tricky to navigate. Matched pairs disappear from the board. The player with the most matched pairs wins.

### 🔵 Game 02 — Qinetika Memory Match
A solo, level-based memory challenge. Numbered squares bounce around the screen during a 5-second memorize phase — then their numbers vanish. The player must click the squares in the correct numerical order from memory. Colors shuffle every round so players can't rely on patterns. Higher levels introduce **Blitz** (random speed bursts) and **Warp** (squares swapping positions). Completing even-numbered levels rewards the player with a skill to use during the recall phase.

---

## Setup Instructions (How to Run)

This project runs entirely in the browser — no installation or build step required.

1. **Clone or download** the repository to your local machine.
2. Open `index.html` (the lobby file) in any modern web browser (Chrome, Firefox, Edge, Safari).
3. The lobby will load, displaying both game cards. Click **▶ PLAY NOW** on either card to launch that game.

> **Note:** An internet connection is required on first load for Google Fonts (`Space Mono` and `Syne`) to render correctly. The games themselves run fully offline once fonts are cached.

---

## List of Controls

### General / Lobby
| Action | Control |
|---|---|
| Launch a game | Click the game card or the **▶ PLAY NOW** button |
| Return to lobby | Click the **← LOBBY** button in the top bar |
| Adjust volume | Drag the volume slider in the top bar |
| Mute / Unmute | Click the speaker icon 🔊 in the top bar |

### Game 01 — Shuffling Memory Match
| Action | Control |
|---|---|
| Flip a card | Left-click on a face-down card |
| Pause / Resume | Click the **Pause** button |
| Return to menu | Click the **Back to Menu** button |
| View instructions | Click **How to Play** on the main menu |

### Game 02 — Qinetika
| Action | Control |
|---|---|
| Click a square (recall phase) | Left-click on the target square |
| Use a skill (recall phase only) | Press keys **1–6** or click an inventory slot |
| Pause / Resume | Click the **Pause** button |
| Return to menu | Click the **Menu** button |

#### Qinetika Skill Keybinds
| Key | Skill |
|---|---|
| `1` | ♥ Extra Heart — Restores 1 life |
| `2` | 🐌 Slug — Slows all squares by 70% for 5 seconds |
| `3` | ❄️ Freeze — Stops all movement for 3 seconds |
| `4` | 💡 Lightbulb — Reveals all numbers for 3 seconds |
| `5` | 💥 Broken Bulb — Flickering number reveal for 5 seconds |
| `6` | ✕2 Double Points — 2× points for the round (cancelled on a wrong click) |

---

## Screenshots

### Memory Match Lobby
![Memory Match Lobby](Screenshot_2026-04-27_083516.png)


### Shuffling Memory Match — Gameplay
![Shuffling Memory Match Gameplay](Screenshot_2026-04-27_083535.png)


### Qinetika — Memorize Phase
![Qinetika Memorize Phase](Screenshot_2026-04-27_083543.png)


---

## Project Notes

- Both games share the same ambient music system built with the Web Audio API — no external audio files are needed.
- All game logic, rendering, and audio are written in vanilla HTML, CSS, and JavaScript with no frameworks or dependencies.
- The lobby embeds both games as Base64-encoded HTML, loaded into iframes on demand.