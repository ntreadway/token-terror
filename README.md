# TOKEN TERROR

**Builder Network Challenge #1: Teach Me Something Scary**

Running out of tokens in Claude Code is scary. Having to finish the job with a fallback model is scarier. TOKEN TERROR is a Halloween survival game that turns that fear into something you understand and can manage.

## Play

Unzip, then double-click `index.html`. No install, no internet needed (Three.js is bundled). Best in Chrome or Safari, desktop with mouse and keyboard.

**Controls:** WASD / arrows move, mouse aims, hold click or Space to fire, P pauses, M mutes.

## The game

You are a little orange mascot in a haunted terminal, which is a neon maze in the spirit of Pac-Man. Walls block you, the ghosts and your bullets, and the ghosts path through the corridors to hunt you. Your token bar drains every second and every shot. Eat the dots along the corridors (small tokens) and grab orange orbs (big tokens) to refill it. Clear every dot for a +500 bonus.

At zero tokens you drop into **Muse-lite mode**: slow, dark, bullets go anywhere, and some tokens are hallucinated. Collect real tokens (25 is enough) to wake Claude back up.

## What it teaches

Every concept shows up as a game mechanic first, then a short lesson card explains the real thing:

| In the game | The real concept |
|---|---|
| Orange orbs and the token ticker | Tokens are chunks of text (~¾ of a word), not whole words |
| Every shot costs tokens | Every request costs tokens; vague prompts cause retries |
| Drain speeds up each wave | Each turn re-reads the whole conversation, so long chats cost more |
| Purple Context Overflow ghost | `/compact`, `/clear`, `/context` |
| Red 429 ghosts | Rate limits (HTTP 429): slow down, back off, retry |
| Out of tokens, Muse mode | Usage limits reset on a rolling window; fallback models need checking |
| Flickering fake tokens | Hallucination: confident is not correct, so verify |
| Blue clock pickup | Plan big tasks around the limit reset |
| Clearing every dot on the board | `/clear`: start the next task with a clean context |

Die once and a quiz question appears. Answer correctly for a free 5-hour reset. Either way you see the explanation. The game-over screen ends with a six-line token cheat sheet.

## Built with

Plain HTML, JavaScript and Three.js (r128, MIT licensed). One file, no build step. Vibe coded with Claude Code.
