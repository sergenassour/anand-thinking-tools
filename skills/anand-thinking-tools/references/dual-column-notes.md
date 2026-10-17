# Dual-column wisdom notes

## The problem with the notes we learned to take

School and university taught one kind of note: the lecturer said something, you wrote it down, because an
exam was coming and you needed to reproduce it. That is retention note-taking. It captures new knowledge
and nothing else.

But three people with different roles and training, listening to the same stakeholder, are not listening
with the same ears. While the new knowledge comes in, each person's wisdom is already reacting: "why did he
say that", "that doesn't sound right", "I know what I'll do with that", "I should speak to John". Those
reactions are at least as valuable as the content, and standard notes lose them. When you return to the
notes a week later, the knowledge is there and the wisdom is gone.

The presenter uses this method on geopolitical and policy-crisis projects with lobbyists and strategy
teams: while absorbing new information they must write down what occurs to them, because "new knowledge is
not the point. The point is what are we going to do."

## The method

Draw a line down the middle of the page.

- **Left column: what is said.** The new knowledge, as the speaker framed it.
- **Right column: what your wisdom says.** Reactions, questions, disagreements, connections, instincts,
  delights, and biases.

On bias: a participant asked how to tell wisdom from bias. The answer was that both go in the right
column. "If part of your subconscious says 'I think Anand is talking crap', write that down." Wisdom does
not talk in straight sentences; the subconscious speaks indirectly. Several of the business examples in
the workshop began as a vague "there's something here" that nobody could name and became billions in
sales. Filter nothing on the right.

Handwriting matters: the hand-to-mind connection reinforces differently from typing, so where the user
writes by hand, the AI's job is to prepare the left column and the prompts, and leave the right column to
the pen.

## Tooling

- Cornell layout or "academic layout" notebooks (available at Kinokuniya).
- reMarkable has this as a built-in template; so do Boox and other e-ink notebooks.
- GoodNotes and similar apps: use a two-column template.
- Plain markdown: the table format in SKILL.md.

## What the AI does and does not do

Does:
- Build the left column faithfully from the source, with markers (timestamps, sections, slide numbers, or
  paragraph numbers you assign when the source has none).
- Write one prompt per row in the right column that invites the user's reaction, specific to the row.
- Offer to interview the user row by row to fill the right column by conversation.
- Pull "what are we going to do" from the user's right-column answers.

Does not:
- Fill the right column with its own opinions. The AI has no wisdom about the user's context.
- Summarise the source so tightly that the triggers for reaction disappear. Keep the speaker's framing
  and examples; those are what provoke the right column.
- Clean up the user's biases. They are data.

## Right-column prompt patterns

| Row type | Prompt pattern |
|---|---|
| A claim | "Does this match what you have seen in [their context]? Where would it break?" |
| A number | "Which number in your own work is this closest to, and is yours higher or lower?" |
| A story or case | "Who in your organisation is the equivalent of [person in the story]?" |
| A recommendation | "What would stop you doing this on Monday?" |
| A framework | "Which part of your current problem does this not cover?" |
| Something the speaker rushed | "This went fast. What did you want to push back on?" |

## Template

```
# [Title] : wisdom notes
Source: [speaker / document], [date], [where]

| What was said | What my wisdom says |
|---|---|
| [00:00] [point, in the speaker's framing] | [prompt] ______ |
| ... | ... |

## What are we going to do
- [to fill after reflection]
```
