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

## Using these skills

Each folder under `skills/` holds a `SKILL.md`. To use one:

- **Claude.ai / Claude app:** upload the skill in Settings → Capabilities → Skills (zip the skill's folder first), or paste the `SKILL.md` into a chat and ask Claude to save it as a skill.
- **Claude Code:** copy the skill's folder into `~/.claude/skills/` (or `.claude/skills/` inside a project).

## Adding a book

1. Create `skills/<skill-name>/SKILL.md` with `name` and `description` frontmatter.
2. Credit the book and author at the top of the skill.
3. Write the method in your own words. Don't copy text from the book.
4. Add a row to the table above.
