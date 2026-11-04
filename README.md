# 15 Years: Zombie World

**15 Years: Zombie World** is a self-contained, browser-based survival game inspired by an owner-provided cinematic zombie timeline. The player guides one survivor from the first day of the collapse to a functioning community fifteen years later.

## Features

- Seven chronological stages: **Day 1, Day 3, Week 1, Month 6, Year 5, Year 10, and Year 15**.
- Three strategic choices at each playable stage.
- Five tracked resources: **water, food, shelter, morale, and community**.
- Three possible endings based on the final state of the settlement.
- Cinematic stills extracted from the supplied reference video, plus the original local video reference.
- Browser-native speech synthesis for the current scene.
- Responsive UI with no external runtime dependencies or remote services.
- Completed stages are locked after a decision, preventing resource accumulation by replaying earlier stages in the same run.

## Technology

- Semantic HTML5
- CSS3 with responsive layout and cinematic styling
- Vanilla JavaScript using a deterministic state machine
- HTML5 video
- Web Speech API (`speechSynthesis`)
- Windows batch launcher

## Run locally

No build step is required. Either:

1. Open `index.html` in a modern browser; or
2. Double-click `ABRIR_JUEGO.bat` on Windows.

All assets are local. The game does not call an API, upload files, or require a package manager. If a browser blocks local video playback from a `file://` URL, serve this folder with any static file server and open the resulting local URL.

## Project structure

```text
index.html                 Game shell and accessible UI structure
game.js                    Stages, choices, state transitions, endings
style.css                  Responsive visual design
ABRIR_JUEGO.bat            Windows launcher
assets/intro.mp4           Local reference video
assets/stage_0.jpg ...     Seven local stage images
```

## Scope

This is a polished playable prototype / portfolio demo. It demonstrates interactive narrative design, stateful decision logic, resource balancing, and a complete local delivery package. It does not claim paid game employment, commercial release, or production-scale multiplayer functionality.
