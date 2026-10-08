# Mark's Shadow Grid

A 2–3 minute hidden-unit strategy game on a 7×8 hex battlefield, with a 5-chapter story mode. Rock-paper-scissors combat
(Armor > Infantry > Anti-Tank > Armor), a Commander, a Spy, and a President to capture.

## Layout
- `docs/index.html` — the whole game. Edit this one.
- `docs/lib/` — three.js r128 and OrbitControls, bundled so the APK works offline (also copied to `app/src/main/assets/lib/`).
- `app/` — Android WebView wrapper. The build copies `docs/index.html` into the APK automatically.
- `.github/workflows/build.yml` — builds the debug APK on every push to `main`.

## Get the APK
1. Push this repo to GitHub (GitHub Desktop works).
2. Open the repo's **Actions** tab and wait for **Build Android app** to finish (about 3–5 minutes).
3. Open the finished run and download **shadow-grid-debug-apk** under Artifacts.
4. Unzip it and install `app-debug.apk` on your phone (allow installs from unknown sources when asked).

## Play in a browser
Enable GitHub Pages (Settings → Pages → `main` branch, `/docs` folder).

## Version 0.1 scope
v0.3: renamed to Mark's Shadow Grid; 3D board (drag to rotate, pinch to zoom, 2D toggle); Relaxed pace with no timers (60 turns).
v0.2: renamed to Mark Dave's Night Division; story mode (5 chapters with dialogue), lore codex, in-world text.
v0.1: single player vs AI, five maps, full v0.3 rules, coin toss for first move.
Not yet built: WiFi PvP and the "Eyes Only" camera mode (both only matter once there's a human opponent).
