## What it does

Zero Slop edits a draft so it stops reading as machine-written: stock phrases, sentences that all run the same length, tidy template structure, and tone that performs instead of saying something. It never adds a fact the author didn't give. Names, numbers, quotes, links and claims about how the author felt all survive exactly, and a sentence that says nothing gets flagged and handed back to you instead of reworded.

The skill bundles local Python scripts that score the draft, point at the exact phrases behind the score, and reject any rewrite that adds or drops a name, number, quotation or link. The assistant does the reading and rewriting; the scripts do the measuring. A draft that already reads as human-written comes back unchanged.

## When to reach for it

Type `/zero-slop`, or the agent reaches for it automatically when a task fits.

| You want to… | Ask for |
| --- | --- |
| Clean up a draft before it goes out | a rewrite (the default) |
| See what reads as AI-written without changing anything | an inspection |
| Guess how a named audience would react, passage by passage | a reader review |

Reach for it on writing a person will read: posts, emails, newsletters, video titles and descriptions. For documents an agent reads (skills, `AGENTS.md`), use [writing-for-agents](https://aihero.dev/skills-writing-for-agents) instead.

## Prerequisites

Python 3 for the scoring scripts. Without it the skill still edits from its reference checklists, but it says so and reports no score.

## The writing score

The score runs from 0 to 100, and lower is better. It describes the writing, not who wrote it, so it never claims a draft was AI-generated. A clear score is a reason to look harder, not permission to stop. The scripts only see patterns tied to specific words. Balanced two-part contrasts, epigram endings and announced significance slip past them, so the assistant checks for those separately and reports the count, even when the count is zero.

The skill also refuses to swap AI-slop for **edgy-slop**: forced hot takes, invented first-person anecdotes, staccato drama. Overcorrection counts as a failure, not a fix.

## Common questions

**Does my draft get sent anywhere?**
Not in the skill's normal run. Scoring, fact checks and rewriting all happen locally and inside your assistant. Once per session it may check GitHub for a newer release, and that request carries only a version number. Set `ZS_NO_UPDATE_CHECK=1` to turn it off. The upstream project also has a hosted `deslop` command that sends text to a remote service, and the skill doesn't use it unless you ask.

**Will it help me hide AI use where disclosure is required?**
No. It refuses requests to get around disclosure rules at schools, journals or employers, and it won't imitate a named person.

## It's working if

- The edit is often smaller than you expected, and sometimes nothing changes at all.
- Every number, name and link from your draft is still there, and nothing new has appeared.
- Empty sentences come back flagged with a request for the missing substance, not reworded.
- The report points at exact phrases rather than giving a vague verdict.

## Where it fits

A reach-for-it-anytime standalone, used last before anything goes out. Its neighbour is [writing-for-agents](https://aihero.dev/skills-writing-for-agents), which covers the other kind of reader. The router over the whole set is [ask-matt](https://aihero.dev/skills-ask-matt).
