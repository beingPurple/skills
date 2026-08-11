# Media Literacy Game

> You edit a newspaper in a fantasy nation coming apart at the seams — and every day brings more
> to read than you have time for. The stories you skim are the ones that decide who rules. A
> heightened, operatic thriller about drowning in the news cycle until complicity feels like just
> hitting your deadline.

A game about **information warfare in the modern news cycle** — how the Internet and bots let a
handful of well-timed stories reshape a whole nation. You play a news **editor** with more to read
than time to read it, forced to decide what runs off the headlines alone and what you know about
your country and the wider fantasy world. Several parties fight to bend politics and everyday life,
each with real pros and cons — so there are many routes and endings, including a state-controlled-media
route in both an **obvious** and a **hidden** form.

This repo is where the game is being **designed**, not yet built. Design happens as a
[`/wayfinder`](./skills/engineering/wayfinder/SKILL.md) map: a big, foggy idea charted into
decision tickets that get resolved one at a time until the way to a finished design doc is clear.

## Where things live

| Path | What it is |
| --- | --- |
| [`.scratch/info-warfare-game/map.md`](./.scratch/info-warfare-game/map.md) | **The map** — destination, locked decisions, the fog ahead, and what's out of scope |
| [`.scratch/info-warfare-game/issues/`](./.scratch/info-warfare-game/issues/) | **Decision tickets** — one file per open question, with blocking edges |
| [`.scratch/info-warfare-game/research/`](./.scratch/info-warfare-game/research/) | Research briefs (genre teardown + real-world info-war concepts) |
| [`skills/`](./skills/) | The Matt Pocock skills that drive the design process |

## Locked so far

- **Destination:** a game design doc (GDD) — decisions locked, build-ready.
- **Player seat:** an **editor** who can escalate into an information-**operator** by route; the
  **state-media route (obvious + hidden)** is the dark mirror of the newsroom.
- **Tone:** an operatic political thriller with satirical bite — vivid and heightened, sharp and
  comic, but never cheap. Default feeling is *overwhelmed → complicit*; **bad endings are earned by
  not reading critically.** A clever/powerful power-fantasy feeling is reserved for the deliberate-
  influence routes.
- **Guiding design principle** (from the research): make **framing** — not accept/reject — the core
  verb, decoupled from delayed/partial-truth outcomes so the player is *sometimes wrong*; let the
  hidden state-media route emerge from **convenience**, not an order.

The [map](./.scratch/info-warfare-game/map.md) always holds the current, authoritative state.

## Continuing the design

The skills in this repo are what you use to keep charting. To resolve the next decision, open the
frontier ticket you want and run wayfinder against the map — e.g. **"wayfinder 01"** (the setting
bible) or **"wayfinder 03"** (the core loop). Wayfinder resolves **one decision per session** so
each big call gets real focus.

If you're setting this repo up in a fresh environment, run `/setup-matt-pocock-skills` once and
`scripts/link-skills.sh` to link the skills into your harness.

## Built on

The design workflow is powered by **[Matt Pocock's skills](./README.md)**, included here under the
**MIT License** — see [`LICENSE`](./LICENSE) (© 2026 Matt Pocock). The original skills documentation
is preserved unchanged in [`README.md`](./README.md).
