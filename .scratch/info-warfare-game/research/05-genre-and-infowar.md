# Research Brief 05 — Genre Teardown & Real-World Information-Warfare Concepts

**Ticket:** `research` (wayfinder map input)
**Scope:** (A) Mechanics teardown of comparable "editor / gatekeeper / choose-what-to-publish" games; (B) real-world information-warfare theory mined for game-mechanic potential.
**Date:** 2026-08-11

---

## A) Comparable games — mechanics teardown

We are building an editor-under-time-pressure game that can escalate into an information-operator, with factions, routes, and multiple endings including an overt and a hidden state-media route. The closest ancestors are Lucas Pope's two games, the newspaper-censorship pair (Westport, Headliner), the surveillance-selection game (Orwell), and the "petitioners exceed resources" throne/tribunal games (Yes Your Grace, We The Revolution). Below, each is torn down on the four axes you asked for: **pressure**, **consequence & branching**, **decision surface**, **pitfalls**.

### The Republia Times (Lucas Pope, 2012) — the direct ancestor

- **Pressure:** A countdown clock ticks toward *press time*. Many wire stories are available each day but only a limited number fit a fixed **4×5 newspaper grid**. Large articles give a bigger loyalty bonus but eat grid space; small articles are weaker individually but pull more readers. The pressure is spatial + temporal: not enough room and not enough time, forcing a triage every day. ([TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/TheRepubliaTimes), [TheGamer](https://www.thegamer.com/papers-please-lucas-pope-dystopian-newspaper-editing-game-the-republia-times/))
- **Consequence & branching:** Two competing meters — **Loyalty** (demanded by the Ministry of Media) and **Readership**. You must hit both. A hidden third pressure: the **rebels** secretly ask you to run damaging stories while still growing readership. Over an **11-day** run this accumulates into one of two "made it" endings (loyal collaborator vs. covertly aided the resistance) plus a fail ending if you miss the metrics. ([Wikipedia](https://en.wikipedia.org/wiki/The_Republia_Times), [TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/TheRepubliaTimes))
- **Decision surface:** Drag-and-drop wire stories from a feed onto the front-page grid; optional "puff up / play down" slant on each story. That's the whole verb set — placement + emphasis.
- **Personal stakes:** The editor personally opposes the regime, but his **wife and children are hostages** to his loyalty numbers. Coercion is the engine that makes the "obvious state-media route" feel forced rather than chosen — directly relevant to our overt vs hidden state route.
- **Pitfalls:** Very short; the meter-juggling can feel like an optimization puzzle rather than a moral one once you learn which stories move which meter. The morality lives almost entirely in the framing device, not in the mechanic.

### Papers, Please (Lucas Pope, 2013) — the pressure & branching gold standard

- **Pressure:** Fixed real-time daily limit; income is per-correct-decision, so throughput matters. The **deliberately clunky interface** (click, hold, drag each document to a reading area) makes moral calculation physically slow and stressful. Rules compound daily (new required documents, discrepancies to cross-check), so cognitive load rises even as the clock stays fixed. Family survival (rent, heat, food, medicine) is a parallel economic meter squeezing every choice. ([Delayed Respawnse](https://delayedrespawnse.com/games/papers-please/), [Medium: Design of Oppression](https://medium.com/@ishikasoni50/the-design-of-oppression-in-papers-please-1b83b16a3079))
- **Consequence & branching:** **20 endings**, most of them bad. Branching is driven by discrete decision points and a **token/flag system** — helping certain entrants, cooperating with or betraying the **EZIC** resistance, fleeing to Obristan, staying loyal. You cannot get all endings in one run because required choices conflict; players savepoint around Days 11/12/23/29 to branch. A **"Where are they now"** epilogue reports each traveler's fate, making abstract choices concrete after the fact. ([Sort the Court: 20 endings](https://www.sort-the-court.com/games/papers-please/all-endings), [Papers Please Wiki: Endings](https://papersplease.fandom.com/wiki/Endings))
- **Decision surface:** Approve / deny + interrogate discrepancies; escalating tools (transcript, fingerprints, body scan). Small verb set, deep because rules stack.
- **Pitfalls (design lessons):** The friction is the point but risks feeling like busywork; Pope's answer is to keep *raising the stakes of a mistake* rather than adding verbs. Branching is invisible mid-run — players only learn the map by replaying, which is fine for a 20-ending structure but means a single playthrough can feel arbitrary.

### Headliner: NoviNews (Unbound Creations, 2018) — closest thematic sibling

- **Pressure:** Each day you **approve/reject a small set of news stories**, then walk home through streets where the public reacts to yesterday's front page. Less time-pressure than Pope; the pressure is *social/consequential* — you see the fallout embodied in NPCs (your brother, bartender, neighbors) the next day. ([Save or Quit](https://saveorquit.com/2018/11/15/review-headliner-novinews/), [Unbound Creations](https://unboundcreations.com/games/headliner-novinews/))
- **Consequence & branching:** Story world advances **exclusively** based on which articles you run. Endings are **combinatorial** — assembled from how each named character fared + the country's state (e.g., border policy, a new health drink's safety) + the Headliner's personal fate. **No golden ending** by design. Strong replay draw (short runs, visible divergence). ([TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/HeadlinerNoviNews), [NintendoSoup](https://nintendosoup.com/game-review-headliner-novi-newsswitch/))
- **Decision surface:** Binary approve/reject per article, sometimes choosing *which slant* of the same event to print.
- **Pitfalls (heavily cited by reviewers — read these before we design):** **Too heavy-handed / no nuance** — characters literally state which slant helps or hurts them, so you always know the outcome before you choose; "not a moment surprised me." Decisions are too **binary**, replay yields little new insight, and the late game becomes a **guilt trip** because every choice visibly dooms a likable character. ([GodisaGeek](https://godisageek.com/reviews/headliner-novinews-review/), [Digitally Downloaded](https://www.digitallydownloaded.net/2019/09/review-headliner-novinews-nintendo.html), [OpenCritic](https://opencritic.com/game/7872/headliner-novinews/reviews)) → **The central risk for our game: telegraphed consequences kill tension.**

### The Westport Independent (Double Zero One Zero, 2016) — censorship-editor cousin

- **Pressure:** Over **12 weeks** you edit a paper for a post-war Loyalist regime: toggle headlines between two framings and **strike out paragraphs** to change meaning. You also assign stories to staff, lay out the paper, and manage **distribution to distinct city districts** with different tastes (gossip, crime, finance, workers' rights). Pressure = commercial (sell papers to survive) vs political (nudge public opinion toward Loyalists or Rebels). ([Steam](https://store.steampowered.com/app/352240/The_Westport_Independent/), [TheSixthAxis](https://www.thesixthaxis.com/2016/02/12/battling-state-censorship-in-the-westport-independent/))
- **Consequence & branching:** Faction letters (Loyalist / Rebel) act as running feedback; a long end cutscene shows city-wide outcomes based on accumulated slant, plus per-staff fates.
- **Decision surface:** Headline toggle + paragraph deletion + story-to-audience assignment. Editing *within* an article (not just accept/reject) is the distinctive verb — closer to real editing than Headliner.
- **Pitfalls:** Reviewers flag **flat one-dimensional characters** and, critically, **choices don't bite until ~week 3 of 12** — the opening feels inert. PC Gamer 67/100, ~40 min runtime felt laborious despite replay hooks. ([Wikipedia](https://en.wikipedia.org/wiki/The_Westport_Independent), [We Got This Covered](https://wegotthiscovered.com/gaming/westport-independent-review/)) → **Lesson: front-load consequence; don't make players wait a third of the game to matter.**

### Orwell: Keeping an Eye On You (Osmotic Studios, 2016) — the selection/gatekeeping engine

- **Pressure:** Cognitive, not reflexive — no timer, no combat. You scrape fragments (social posts, chats, medical records, news) and **drag only chosen "datachunks" into a target's profile**. The stress is **information overload + irreversibility**: uploaded data can't be recalled, and conflicting facts force you to decide *what is true* and *what to forward to security forces*. ([Steam](https://store.steampowered.com/app/491950/Orwell_Keeping_an_Eye_On_You/), [SuperJump](https://www.superjumpmagazine.com/unseen-gazes-in-orwell-keeping-an-eye-on-you/))
- **Consequence & branching:** What you highlight steers arrests and public perception of the government; some threads resolve, others spiral. Investigations gate on which datachunk you believed.
- **Decision surface:** Select-and-submit individual facts. The genius: **partial truths** — two chunks each true but together implying a falsehood. This is the most sophisticated "you decide the narrative from raw material" verb in the genre and maps directly onto our editor-choosing-framing loop.
- **Pitfalls:** Because there's no clock, tension relies entirely on story stakes and the weight of irreversibility; when the mystery sags, so does engagement.

### Yes, Your Grace (Brave At Night, 2020) — "demand exceeds resources" pacing model

- **Pressure:** A weekly line of **petitioners** in the throne room, each wanting Gold, Supplies, Army, or a favor. Deliberately, **a week's collective demands exceed what you have** — you must refuse people, and refusals lower Contentment (which lowers future tax income). Scarcity is engineered so you're always disappointing someone. ([Steam](https://store.steampowered.com/app/1115690/Yes_Your_Grace/), [TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/YesYourGrace))
- **Consequence & branching:** Choices compound into resource states that gate later crises; multiple endings from accumulated goodwill/resources. 93%+ positive over 11k reviews — the "not enough to go around" loop is proven.
- **Decision surface:** Grant / deny per petitioner, plus occasional larger narrative decisions.
- **Relevance:** This is the cleanest existing model of your **"more to read than time allows"** brief — reframe petitioners as *incoming stories competing for finite front-page slots and finite editor attention.*

### We. The Revolution (Polyslash, 2019) — multi-faction balancing under judgment

- **Pressure:** As a Revolutionary-Paris tribunal judge you review evidence, interrogate, and **render verdicts — but verdicts are about pleasing factions, not truth.** Three power blocs (commoners, revolutionaries, aristocrats) each track your favor; you can't satisfy all, and falling out with any is dangerous. A separate **Intrigue** metagame lets you plant allies and blackmail enemies — i.e., you can *escalate from judge to operator*, exactly our editor→operator arc. ([TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/WeTheRevolution), [Age of Revolutions](https://ageofrevolutions.com/2019/07/29/affecting-revolutionary-justice-a-review-of-we-the-revolution/))
- **Consequence & branching:** Each decision shifts faction meters, family standing, and self; branching flows from which blocs you've kept onside.
- **Decision surface:** Evidence review → questioning → verdict + report, plus the Intrigue board.
- **Pitfalls:** "Splendid as revolution emulation, faulty as a game" — the many mini-systems can feel disjointed, and juggling three faction meters plus intrigue plus family can tip into spreadsheet management. 74% positive. → **Lesson: multiple faction meters are great for tension but need a legible UI or they become bookkeeping.**

### Cross-game synthesis

| Axis | What works across the genre |
|---|---|
| **"Too much / too little time"** | A **finite container** (grid slots, daily quota, weekly petitioner line, press-time clock) that is *always* smaller than incoming demand. Triage, not completion, is the verb. Papers/Republia use a clock; Yes Your Grace uses resource scarcity; both engineer forced refusal. |
| **Consequence & branching** | **Accumulating hidden meters** (loyalty, faction favor, readership) that resolve into **combinatorial endings** (Headliner) or **flag/token-gated discrete endings** (Papers Please, 20). Epilogue "where are they now" screens (Papers, Headliner, Westport) convert abstract choices into felt outcomes. |
| **Decision surface** | Best-in-class is **framing/emphasis, not just accept-reject**: Westport's paragraph-striking and Orwell's partial-truth datachunks are richer than Headliner's binary. Slant-the-same-event beats approve/reject. |
| **Biggest shared pitfall** | **Telegraphed outcomes** (Headliner) and **delayed stakes** (Westport week-3). Also: **short runtime + thin characters** limit replay despite branching. |

---

## B) Real-world information-warfare concepts → candidate mechanics

Each concept below is followed by **→ Mechanic**: how it could become a system in our game.

### 1. Agenda-setting theory (McCombs & Shaw)
Media doesn't tell people *what to think* but *what to think about*; sustained coverage of an issue raises its public salience and policy pressure. ([Wikipedia](https://en.wikipedia.org/wiki/Agenda-setting_theory), [Communication Theory](https://www.communicationtheory.org/agenda-setting-theory/))
→ **Mechanic:** A per-issue **Salience meter**. Front-paging or repeatedly running a topic raises its salience; high salience unlocks/forces later events (protests, elections, crackdowns). The player shapes the *world agenda* by allocation of scarce slots, independent of the slant.

### 2. Gatekeeping theory (Lewin / White)
Editors are **gatekeepers** who admit or block stories by "newsworthiness," filtered through corporate and government interests. What the audience can even know is set at the gate. ([Gardner-Webb honors thesis](https://digitalcommons.gardner-webb.edu/cgi/viewcontent.cgi?article=1022&context=undergrad-honors), [Pressbooks](https://pressbooks.openeducationalberta.ca/insightsintocommstudies/chapter/chapter-8-mass-media/))
→ **Mechanic:** This *is* the core loop — the **finite front-page gate**. Every story killed at the gate is invisible to the public and to the meters. Add **kill/hold/run** as the three-way primary verb (vs. binary).

### 3. Framing
Same event, different emphasis: selecting which facts to highlight promotes a particular interpretation (Watergate went from "third-rate burglary" to "constitutional crisis" purely via framing). ([Pressbooks](https://pressbooks.openeducationalberta.ca/insightsintocommstudies/chapter/chapter-8-mass-media/))
→ **Mechanic:** Per-story **slant selector** (à la Westport headline toggle / Orwell chunk choice): each story ships with 2–3 framings that move different faction meters in different directions. This is where nuance lives — decouple *whether* to run from *how* to run.

### 4. The Propaganda Model — five filters (Herman & Chomsky)
News is filtered by (1) concentrated **ownership**, (2) **advertising** as the paymaster, (3) reliance on official **sources**, (4) **flak** (organized pushback that punishes outlets), (5) an enemy/"folk-devil" **ideology**. Serving-power stories pass easily; challenging ones get blocked. ([LibreTexts](https://human.libretexts.org/Workbench/Communication_and_Critical/Cultural_Studies/04:_The_Propaganda_Model/4.01:_The_Five_Filters_of_the_Propaganda_Model), [Chomsky.info](https://chomsky.info/consent01/))
→ **Mechanics (a whole constraint layer):**
- **Ownership/Advertiser pressure** = a **budget/sponsor meter**; certain stories anger sponsors and cut your operating funds (cf. Papers Please rent). This is the *soft* version of Republia's hostage coercion — the **hidden state-media route** can be reached simply by always bowing to sponsor/ownership pressure without ever being "ordered."
- **Source dependency** = privileged **official wire stories** arrive pre-written and free; independent stories cost time/money to verify. Leaning on official sources is fast but slants you.
- **Flak** = running hostile stories triggers **lawsuits/harassment/ad boycotts** events that raise pressure and eat time.

### 5. Firehose of falsehood (RAND, Paul & Matthews 2016)
Four traits: **high volume**, **multichannel**, **no commitment to objective reality**, **no commitment to consistency**. Works because repetition across many apparent sources breeds belief, and volume overwhelms fact-checking. ([RAND PE-198](https://www.rand.org/pubs/perspectives/PE198.html), [Wikipedia](https://en.wikipedia.org/wiki/Firehose_of_falsehood))
→ **Mechanic (escalation / operator mode):** Once the player escalates to *operator*, they can **flood the feed** — spawn many low-quality bot stories to bury a true story's salience or drown a rival faction's narrative. Volume overwhelms the *reader's* finite attention (mirroring our own core constraint back at the world). Cheap, effective, and *corrosive to your credibility meter* — the cost side.

### 6. Astroturfing & manufactured consensus
Fabricating the *appearance* of grassroots support: "making the voices of the few sound like the roar of the many." Requires coordination + false authenticity. ([SAGE: Chan 2024](https://journals.sagepub.com/doi/10.1177/01914537221108467), [Springer](https://link.springer.com/article/10.1007/s13278-021-00815-2))
→ **Mechanic:** A **fake-comment / fake-poll** action that inflates a story's apparent public support, shifting the **Salience** and **Contentment**-style meters without any real event. Detectable → risk of exposure scandal.

### 7. Coordinated inauthentic behavior (CIB) & troll/bot farms
Networks of bots, cyborgs, paid trolls, and duped real users amplify content while posing as authentic identities; the Internet Research Agency is the archetype. Detection is possible but arms-races with sophistication. ([BiPartisan Policy](https://bipartisanpolicy.org/article/coordinated-influence-operations/), [Medium: IRA](https://medium.com/@thecyberhuntress/troll-farms-and-the-internet-research-agency-understanding-the-machinery-behind-online-c2cc4c969eb7))
→ **Mechanic (the "bots & escalation" system):** The player **builds and tunes a bot network** as a resource: capacity (how many stories/comments it can push per cycle), authenticity (how bot-like it looks), and heat (how close detectors are). Higher output ↔ higher detection risk. This is the tech-tree of the operator arc and the mechanical bridge from "editor" to "information warrior."

### 8. Detection / exposure as a counter-pressure
Astroturf and CIB can be detected via content and network analysis; sophistication buys evasion. ([Springer: astroturf detection](https://link.springer.com/article/10.1007/s13278-025-01557-1), [arXiv: troll footprint](https://arxiv.org/pdf/2409.07720))
→ **Mechanic:** A rising **Scrutiny/Exposure meter** driven by inauthentic actions; crossing thresholds triggers investigations, deplatforming, or a scandal ending. Gives the operator powers a real cost and creates the risk curve that keeps escalation tense.

---

## Implications for our design tickets

### Core loop (Ticket 03)
- **Adopt a finite-container triage loop.** Steal Republia's grid × Yes-Your-Grace's "demand > capacity": each cycle, more stories arrive than fit the front page *and* than you have time to read/verify. The core verbs are **read (costs time) → kill / hold / run (gate) → slant (frame)**. Reading is itself a scarce resource — you often must publish stories you didn't fully read, which is the "too much to read" tension made mechanical (cf. Orwell's overload, Papers' clock).
- **Make framing, not accept/reject, the expressive verb.** Every runnable story carries 2–3 framings (Westport toggle / Orwell partial-truth). This is the single biggest lever against Headliner's fatal flaw.
- **Front-load stakes.** Westport's choices don't bite until week 3 — reviewers hated it. Ensure a meaningful consequence lands within the first 1–2 cycles.

### Consequence model (Ticket 07)
- **Hidden accumulating meters → combinatorial endings.** Run parallel meters (per-faction favor, per-issue Salience, Readership, Credibility, Sponsor/Budget, Scrutiny). Resolve endings *combinatorially* like Headliner (country state × faction fates × player fate) rather than one golden path — "no golden ending" is both thematically right and proven popular.
- **Avoid telegraphing.** Headliner's #1 criticism is you always know the outcome before choosing. Introduce **uncertainty**: framings should have *probabilistic* or *delayed* or *partial-info* effects, and some "facts" should be Orwell-style partial truths that backfire. The player should sometimes be *wrong*.
- **Use "where are they now" epilogues.** Papers/Headliner/Westport all convert abstract meter shifts into concrete named-character fates at the end (and ideally in mid-game vignettes). Cheap, high emotional payoff.
- **Legibility over volume of meters.** We. The Revolution shows 3+ faction meters + intrigue can become bookkeeping. Cap visible meters or roll them into a clean dashboard.

### Bots & escalation (Ticket 10)
- **Model the bot network as a tunable resource with a heat cost.** Three dials from the CIB/astroturf research: **output capacity**, **authenticity**, **detection heat**. Operator actions — **firehose/flood** (bury a story via volume), **astroturf** (fake consensus on a story), **CIB amplify** (make one narrative look multi-sourced) — each spend network capacity and raise a **Scrutiny/Exposure** meter.
- **Escalation must be a ratchet with a downside.** Editing is legitimate; operator powers are potent but every use raises Exposure toward investigation/scandal/deplatform endings. This is the risk curve that keeps the back half tense — it's the operator-arc analog of Papers Please raising the cost of a mistake rather than adding verbs.
- **Turn our own core constraint into a weapon.** Firehose works by overwhelming *finite attention* — the same scarcity the player suffers in the core loop. Letting the player weaponize volume against the world's readers is thematically tight and mechanically reuses existing systems.

### Routes (Ticket 11)
- **Overt state-media route = coercion (Republia model).** An explicit Ministry/owner that *orders* loyalty numbers, with a personal-hostage or shut-down stake. Obvious, sign-posted, "safe but damned."
- **Hidden state-media route = the propaganda model's soft capture.** Reach it *without ever being ordered* — by habitually bowing to **sponsor/ownership** and **official-source** filters (fast, free, profitable). The player slides into being a state organ through convenience, and only the epilogue reveals they became what they feared. This is the more interesting, emergent version and directly implements Herman-Chomsky.
- **Resistance/independent route = the covert-rebel line from Republia + EZIC from Papers.** A hidden faction that asks for damaging-but-true stories while you keep your cover meters up; betrayable in both directions.
- **Branch via flags + savepoints, not one linear meter.** Papers Please's 20-ending, conflict-choice, savepoint-to-branch structure is the model: routes should be mutually exclusive within a run to drive replay, with a discoverable map rather than a signposted fork.

---

### Sources (primary references)
- The Republia Times — [Wikipedia](https://en.wikipedia.org/wiki/The_Republia_Times), [TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/TheRepubliaTimes), [TheGamer](https://www.thegamer.com/papers-please-lucas-pope-dystopian-newspaper-editing-game-the-republia-times/)
- Papers, Please — [Delayed Respawnse](https://delayedrespawnse.com/games/papers-please/), [Design of Oppression (Medium)](https://medium.com/@ishikasoni50/the-design-of-oppression-in-papers-please-1b83b16a3079), [20 endings](https://www.sort-the-court.com/games/papers-please/all-endings), [Endings wiki](https://papersplease.fandom.com/wiki/Endings)
- Headliner: NoviNews — [TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/HeadlinerNoviNews), [Save or Quit](https://saveorquit.com/2018/11/15/review-headliner-novinews/), [GodisaGeek (criticism)](https://godisageek.com/reviews/headliner-novinews-review/), [Digitally Downloaded](https://www.digitallydownloaded.net/2019/09/review-headliner-novinews-nintendo.html)
- The Westport Independent — [Steam](https://store.steampowered.com/app/352240/The_Westport_Independent/), [TheSixthAxis](https://www.thesixthaxis.com/2016/02/12/battling-state-censorship-in-the-westport-independent/), [Wikipedia](https://en.wikipedia.org/wiki/The_Westport_Independent)
- Orwell: Keeping an Eye On You — [Steam](https://store.steampowered.com/app/491950/Orwell_Keeping_an_Eye_On_You/), [SuperJump](https://www.superjumpmagazine.com/unseen-gazes-in-orwell-keeping-an-eye-on-you/)
- Yes, Your Grace — [Steam](https://store.steampowered.com/app/1115690/Yes_Your_Grace/), [TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/YesYourGrace)
- We. The Revolution — [TVTropes](https://tvtropes.org/pmwiki/pmwiki.php/VideoGame/WeTheRevolution), [Age of Revolutions](https://ageofrevolutions.com/2019/07/29/affecting-revolutionary-justice-a-review-of-we-the-revolution/)
- Agenda-setting — [Wikipedia](https://en.wikipedia.org/wiki/Agenda-setting_theory), [Communication Theory](https://www.communicationtheory.org/agenda-setting-theory/)
- Gatekeeping & framing — [Gardner-Webb](https://digitalcommons.gardner-webb.edu/cgi/viewcontent.cgi?article=1022&context=undergrad-honors), [Pressbooks](https://pressbooks.openeducationalberta.ca/insightsintocommstudies/chapter/chapter-8-mass-media/)
- Propaganda model — [LibreTexts (five filters)](https://human.libretexts.org/Workbench/Communication_and_Critical/Cultural_Studies/04:_The_Propaganda_Model/4.01:_The_Five_Filters_of_the_Propaganda_Model), [Chomsky.info](https://chomsky.info/consent01/)
- Firehose of falsehood — [RAND PE-198](https://www.rand.org/pubs/perspectives/PE198.html), [Wikipedia](https://en.wikipedia.org/wiki/Firehose_of_falsehood)
- Astroturfing / CIB / bot farms — [SAGE (Chan 2024)](https://journals.sagepub.com/doi/10.1177/01914537221108467), [BiPartisan Policy](https://bipartisanpolicy.org/article/coordinated-influence-operations/), [IRA (Medium)](https://medium.com/@thecyberhuntress/troll-farms-and-the-internet-research-agency-understanding-the-machinery-behind-online-c2cc4c969eb7), [Springer (detection)](https://link.springer.com/article/10.1007/s13278-025-01557-1)
