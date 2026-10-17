# Annand Thinking Tools

A Claude skill that turns Claude into a thinking partner rather than an answer machine. It packages the
six tools from Anand Vengurlekar's workshop on wisdom, learning velocity and AI (Greenhouse, 15 October
2026). The central idea: AI can regurgitate knowledge for anyone now, so the human edge has moved to
wisdom and to the questions nobody else asks. Every tool pulls that wisdom out of you instead of
replacing it with the model's.

| Tool | What you say | What Claude does |
|---|---|---|
| 1. Dual-column wisdom notes | "Help me take two-column notes on this transcript" | Left column: what was said. Right column: prompts for your own reaction, left blank for you |
| 2. Question-storming | "What questions should we be asking about this process?" | Ranked questions, no solutions, with the unspoken assumption named |
| 3. Critical-thinking review | "Poke holes in this proposal" | Paul and Elder hazy, bias and logic reflection questions, each anchored to a section. No verdict |
| 4. Incubation | "I've been stuck on this for three days" | Diagnoses the stage, closes the brief, sends you away from the screen, verifies the idea when you return |
| 5. Reading with AI | "Where do I start with this book?" or "Feynman me on chapter 5" | Adler's inspectional reading, chapter prep, and the Feynman "what did I miss" check |
| 6. Narrative structures | "Turn this memo into a deck for the board" | Picks from eleven structures (STAR, SCQA, Pyramid, PREP, A3, Monroe, PIIR, Before-After-Bridge, What/So what/Now what, 4C, Story Spine), gives you a storyboard to approve before any slide is built |

## Install

### On claude.ai (web, desktop app, mobile)

1. Download [`dist/annand-thinking-tools.skill`](dist/annand-thinking-tools.skill).
2. In Claude, open **Settings, Capabilities, Skills** and choose **Upload a skill**.
3. Pick the file. It appears in your skills list, switched on.

Skills need a Pro, Max, Team or Enterprise plan. On Team and Enterprise an admin can publish it to the
whole workspace from the same page.

### In Claude Code

Add this repository as a plugin marketplace, then install the plugin:

```bash
claude plugin marketplace add sergenassour/annand-thinking-tools
```

```bash
claude plugin install annand-thinking-tools@annand-thinking-tools
```

Or copy the folder `skills/annand-thinking-tools` into `~/.claude/skills/` (for every project) or into a
project's `.claude/skills/` (for that project only).

## Use

Claude triggers the skill on its own when you ask to review a proposal, build a deck, take notes on a
talk, read a book, or say you are stuck. To force it, say "use the Annand tools" or name the tool.

Two habits the skill enforces that are worth knowing in advance:

- It will not build a deck until you have approved a storyboard. The narrative has to be yours.
- It returns questions to reflect on, not verdicts. You know the context the document is going into;
  the model does not.

## Layout

```
skills/annand-thinking-tools/
  SKILL.md                                  the skill: stance, principles, six tools, output formats
  references/
    dual-column-notes.md                    the note-taking method and template
    question-storming.md                    lenses and examples (Uber, iPod, iPhone keynote)
    critical-thinking-cheatsheet.md         Paul and Elder handout, 8 elements by 3 red-flag families
    incubation.md                           Wallas's four stages in full
    reading-with-ai.md                      Adler's six steps, chapter protocol, Feynman prompts
    narrative-structures.md                 eleven structures with practice questions
    workshop-source.md                      provenance and the framing stories
  evals/evals.json                          test prompts used while building
dist/annand-thinking-tools.skill            packaged for claude.ai upload
```

## Credits

See [NOTICE.md](NOTICE.md). The content is Anand Vengurlekar's, shared with his permission. The skill
was written by Serge Nassour with Claude.
