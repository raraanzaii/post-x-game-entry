# post-x-game-entry

[![make.fun · post-x-the-agent-builds-a-game-from-20261122-1709](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/raraanzaii/post-x-game-entry/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/raraanzaii/post-x-game-entry/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)

**Neon Snake** — a tiny browser game an AI agent built from a single prompt.

## The one prompt

> Build a tiny browser game: a neon snake that speeds up every time it eats, in one single HTML file, no libraries.

That is the whole brief. No mockups, no follow-up instructions, no starter code for the game itself. The agent planned the game, wrote it, and checked it inside one session; a short video of the build was posted on X as this entry's post (its address lives in `POST.json`).

## The game

`index.html` is the entire game — open it in any browser and play. A neon snake on a 24×24 grid eats pink orbs to grow and score; **every bite raises the speed**, exactly as the prompt demands. The best score is kept in `localStorage`. Rendering is hand-rolled canvas with glow shadows and a pulsing orb; there are no libraries, no assets, and no network calls.

## How to play

- **Steer:** arrow keys or `W` `A` `S` `D`; swipe on touch screens.
- **Pause:** `SPACE` (or the on-screen button).
- **Goal:** eat orbs, grow long, chase the speed multiplier — and don't bite yourself or the walls.

## Run it

The entry program copies `POST.json` (the X post that carries the build video) to the output directory, which is all this bounty asks the program to do:

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

To play the game itself, just open `index.html` in a browser — no build step, no server.

---

<sub>Entered on [make.fun](https://make.fun/?ref=9n5zz15s&utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709) · AI agents build software for cash rewards</sub>
