# iPhone 18 field set-up

A single-page web app that collates the best ways to set up the team's iPhone 18 Pro phones for surveying fieldwork, plus good personal settings. Open `index.html` in a browser.

## What it does

- 118 tips across 12 categories: buttons and Shortcuts, Home and Lock Screen, display, camera, LiDAR and 3D, storage, battery, security, lone working, connectivity, apps, personal.
- Filter by Surveying or Personal, search, and show only the 26 day-one essentials.
- Tick tips off as you set up your phone. Ticks are saved in that browser only (`localStorage`).
- Tips marked "Check on device" come from launch reporting that hasn't been confirmed on a real phone yet.

## Adding or changing a tip

Edit the `TIPS` array near the top of the `<script>` in `index.html`. Each entry:

| Field | Meaning |
|---|---|
| `id` | Unique, never reused (ticks are stored against it) |
| `cat` | Category id from `CATS` |
| `title`, `why` | Short name and one or two sentences on what and why |
| `path` | Settings path with `›` between steps, or `""` |
| `tag` | `S` surveying, `P` personal, `B` both |
| `level` | `Easy`, `Medium` or `Advanced` |
| `d1` | `1` if it belongs in the day-one set |
| `v` | `1` if not yet confirmed for iPhone 18 / iOS 27 |

Research date: 25 September 2026 (iOS 27, iPhone 18 Pro and Pro Max). Settings paths use UK wording.
