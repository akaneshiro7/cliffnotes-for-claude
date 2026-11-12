# cliffnotes-for-claude

Knowledge distilled from books into agent skills.

Each skill takes the core method of a book and rewrites it, in my own words, as instructions Claude can follow, so the ideas actually get used instead of sitting on a shelf.

## Skills

### 📘 *The Art of Explanation* by Ros Atkins (2023)

| Skill | Use it for |
|---|---|
| [`explain-clearly`](skills/explain-clearly/SKILL.md) | Prepared explanations: reports, essays, presentations, scripts, pitches. The ten tests of a good explanation, plus the Seven-Step method. |
| [`dynamic-explanation`](skills/dynamic-explanation/SKILL.md) | Unscripted moments: interviews, meetings, Q&As. Build strands, practise out loud, and prepare for the questions. |
| [`quick-explanations`](skills/quick-explanations/SKILL.md) | Everyday emails, messages and quick calls. Bottom line up front, easy to skim, easy to reply to. |

### 📗 *The Mom Test* by Rob Fitzpatrick (2013)

| Skill | Use it for |
|---|---|
| [`customer-conversations`](skills/customer-conversations/SKILL.md) | Customer, client and stakeholder conversations that get the truth: ask about their life and past behaviour rather than your idea, avoid compliments and fluff, and push for real commitments. |

### 📙 *The Minto Pyramid Principle* by Barbara Minto (3rd ed., 2010)

| Skill | Use it for |
|---|---|
| [`pyramid-principle`](skills/pyramid-principle/SKILL.md) | Structuring memos, emails, decks and analyses answer-first. Situation, complication, question, answer; MECE groupings; action titles; issue trees. |

### 📕 *Crucial Conversations* by Patterson, Grenny, McMillan & Switzler (2nd ed., 2012)

| Skill | Use it for |
|---|---|
| [`high-stakes-conversations`](skills/high-stakes-conversations/SKILL.md) | Pushback, tough feedback, conflict, raising a mistake. Start with heart, make it safe, master your stories, STATE your path, AMPP listening, and finish with who does what by when. |

## Which skill should I use?

Each skill has one job. Several can work together on the same task.

| If you need to… | Use |
|---|---|
| Work out the **answer and the logic** of a recommendation, memo, analysis or deck storyline | `pyramid-principle` |
| Help people **understand** something in depth (an explainer, talk, essay or training) | `explain-clearly` |
| Write a **short email or message** that gets read and answered | `quick-explanations` |
| Know your material well enough to **answer anything live** (interviews, Q&A, meetings) | `dynamic-explanation` |
| **Learn the truth** from a client, customer or stakeholder | `customer-conversations` |
| Handle a **tense or emotional** conversation (pushback, feedback, conflict) | `high-stakes-conversations` |

Common combinations: a recommendation email uses `pyramid-principle` for the content and `quick-explanations` for the format. A big presentation uses `pyramid-principle` for the storyline and `explain-clearly` for the language and delivery. Pushing back on your MD uses `high-stakes-conversations` for how to say it and `pyramid-principle` for what you're proposing.

## Using these skills

Each folder under `skills/` holds a `SKILL.md`. To use one:

- **Claude.ai / Claude app:** upload the skill in Settings → Capabilities → Skills (zip the skill's folder first), or paste the `SKILL.md` into a chat and ask Claude to save it as a skill.
- **Claude Code:** copy the skill's folder into `~/.claude/skills/` (or `.claude/skills/` inside a project).

## Adding a book

1. Create `skills/<skill-name>/SKILL.md` with `name` and `description` frontmatter.
2. Credit the book and author at the top of the skill.
3. Write the method in your own words. Don't copy text from the book.
4. Add a row to the table above.
