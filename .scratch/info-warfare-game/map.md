<!-- wayfinder:map -->
# Wayfinder map: Information-warfare news-cycle game

## Destination

A **game design doc (GDD)** for the information-warfare game — locked decisions across the
core loop, factions, routes/endings, setting bible, and scoring — complete enough to hand to
a developer (or future-you) and start building. Prose deliverable, not code. Produced by the
final assembly ticket (`15-gdd-assembly`).

## Notes

- **Domain:** game design. Setting is a fantasy nation running a modern media ecosystem
  (the Internet, bots). Consult `CONTEXT.md` and `docs/agents/domain.md` each session.
- **Premise locked while charting:** the player is a news **Editor** who can **escalate into
  an information-operator** by route. The **state-controlled-media route — obvious *and*
  hidden — is the dark mirror** of the newsroom origin.
- **Core tension (given by the user, not up for debate):** there is always more to read than
  there is time to read it; publish decisions are made off **headlines + the player's
  knowledge of the nation and the greater fantasy world**.
- **This is PLANNING.** Produce decisions, not build. Resolve **one ticket per session**
  (research tickets excepted). The single execution step is `15-gdd-assembly`, which compiles
  the resolved decisions into the destination artifact.
- **Skills to invoke per ticket:** `/grilling` + `/domain-modeling` for decision tickets;
  `/prototype` for "how should it behave/look" tickets; `/research` for external knowledge.

## Decisions so far

<!-- index only — one line per resolved ticket, gist + link; detail lives in the ticket -->

- [05 — Genre & info-war research](issues/05-genre-and-infowar-research.md) — Republia Times is the skeleton (press clock + too-small front page + Loyalty/Readership meters); make **framing/reframe** the core verb, decouple it from **probabilistic/delayed/partial-truth** outcomes so the player is sometimes wrong; hidden state-media route should emerge from **convenience** (free official sources + sponsor-safe framings), not an order. Avoid Headliner's telegraphed binary choices.
- [04 — Tone & pitch](issues/04-tone-and-pitch.md) — **Operatic political thriller with satirical bite** (heightened, not straight satire). Default feeling **overwhelmed → complicit**; bad endings are **earned by not reading critically** — that's a hard design constraint on the loop (03) & knowledge (09). **Power-fantasy** feeling is a *reward reserved for the deliberate-influence routes* (operator / overt state-media). Touchstones: Papers Please, Republia Times, Disco Elysium, Network.

## Not yet specified

<!-- in-scope fog: real but not yet sharp enough to ticket; graduates as the frontier advances -->

- **Difficulty & balance tuning** of the consequence model (needs the model's shape first — ticket 07).
- **Content volume & authoring format** for the headline/story corpus (needs the story object — ticket 06 — and structure — ticket 14).
- **Tutorial / onboarding** flow (needs the core loop — ticket 03).
- **Detailed UI screen layouts** (needs the loop + the verb set — tickets 03, 06).

## Out of scope

<!-- ruled beyond the destination; never graduates. Redrawing the destination reopens as a fresh effort. -->

- **Engine / tech stack & code implementation** — that's build, past a design spec.
- **Art & audio asset production.**
- **Writing the full headline/story content corpus** — we design the *format*, not the corpus.
- **Monetization / business model.**
