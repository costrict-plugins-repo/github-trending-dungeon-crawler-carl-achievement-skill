# DCC Achievement Skill

```
═══════════════════════════════════════════════
NEW ACHIEVEMENT!
OPEN SOURCE EXHIBITIONIST!
═══════════════════════════════════════════════

You have mass-published your personal joke
infrastructure to a public repository. Every
reference file. Every anti-pattern. The entire
architecture of a system designed to generate
fake awards for your own bad decisions, now
available for strangers to install and judge
you with.

Question: What kind of person documents a foot
fetish joke generator more thoroughly than their
client deliverables? Answer: You. The answer is
you.

Reward: You've received a Gold Yak Shaver's Box!

═══════════════════════════════════════════════

╔═══════════════════════════════════════════════╗
You open your Gold Yak Shaver's Box!
╚═══════════════════════════════════════════════╝

The box is wrapped in what appears to be
printer paper held together with git commits.
It smells faintly of obsessive iteration and
neglected timesheets.

You have received the following items:

★ Scroll of Recursive Self-Documentation (Rare)

When activated, compels you to write reference
files ABOUT the reference files you already
wrote. Side effects include an unshakable
conviction that your anti-patterns file needs
its own anti-patterns file. There is no cure.

★ Cloak of Plausible Utility (Uncommon)

Wearing this cloak allows you to describe any
personal hobby project as "context engineering
research" with a straight face. Effectiveness
increases with the number of footnotes in your
blog post about it.

═══════════════════════════════════════════════
```

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) plugin that generates [Dungeon Crawler Carl](https://www.mattdinniman.com/) style achievement notifications for real-world situations.

Tell it you spent six hours in meetings and produced nothing. It will tell you that you have earned a Silver Calendar Hostage's Box containing a Helm of Selective Deafness.

The System AI judges your life choices so you don't have to.

## Installation

### As a plugin (recommended)

Register this repo as a plugin marketplace in Claude Code, then install:

```
/plugin marketplace add jamiebono/dcc-achievement-skill
/plugin install dcc-achievement@jamiebono-dcc-achievement-skill
```

For local development or offline use, clone and load with the `--plugin-dir` flag instead:

```bash
git clone https://github.com/jamiebono/dcc-achievement-skill.git
claude --plugin-dir ./dcc-achievement-skill
```

### As a standalone skill

Copy the `skills/achievement/` directory into your project's `.claude/skills/` folder:

```bash
cp -r dcc-achievement-skill/skills/achievement .claude/skills/achievement
```

Standalone skills get shorter names (`/achievement` instead of `/dcc-achievement:achievement`) but are scoped to a single project.

## Usage

The skill activates from natural language. Say any of:

- "achievement for missing a deadline"
- "DCC achievement for spending four hours on a twelve-line config file"
- "achievement unlocked: I explained my own job to the sales team"

Or invoke directly:

```
/dcc-achievement:achievement spent six hours in meetings and produced nothing
```

### Flags

| Flag | Effect |
|------|--------|
| `--loot` | Generates a full loot box opening sequence after the achievement: sensory box description, items named like RPG gear, and the System AI editorializing about why you need them. |

```
achievement --loot for someone who explained scope creep to a client using a PowerPoint
```

### Modes

**Quick mode** (default): Give it a situation, get an achievement.

**Batch mode**: Give it a list of situations. It varies tiers and rhetorical patterns across the set.

**Vault-aware mode**: Say "roast my week" or "what did I earn" without specifying a situation. The skill reads your working files (task lists, daily notes, project files) and generates achievements based on what it finds. Customize the file paths in the SKILL.md to match your vault structure.

## Architecture

```
skills/achievement/
├── SKILL.md                        # Skill definition, modes, process
├── references/
│   ├── system-ai-voice.md          # Who the System AI is and how it talks
│   ├── achievement-anatomy.md      # Output format, tiers, box naming
│   ├── tone-rules.md               # Anti-patterns: what makes it funny vs. cringe
│   └── loot-box-anatomy.md         # Loot box format and item mapping
└── examples/
    └── canonical-achievements.md   # Real achievements from the books, annotated
```

Five reference files for a joke generator. Each one solves a specific problem:

- **Voice profile** defines personality, speech patterns, and tone variation by situation type.
- **Achievement anatomy** specifies the output format: title, trigger line, commentary, reward, box name, tier.
- **Tone rules** define anti-patterns with before/after examples. The line between "DCC System AI" and "try-hard sarcastic chatbot" is thin. This file defines the difference.
- **Loot box anatomy** handles the `--loot` flag: box descriptions, item naming, rarity tiers, situation-to-item mapping.
- **Canonical examples** are real achievements from the books with annotations explaining why each one works. This is where the skill actually lives. Examples calibrate tone. Instructions describe it.

## How it was built

This skill was built iteratively through conversation with Claude Code. The development process:

1. Started with a single page of instructions. Output was generic.
2. Searched the DCC Fandom Wiki and Goodreads for real achievement text.
3. Had the AI annotate the examples (what makes each one work).
4. Corrected the annotations and saved as `canonical-achievements.md`.
5. Used the skill, noticed what was wrong, wrote it down as an anti-pattern.
6. Every correction made twice became a reference file entry.
7. Dogfood tested by pasting into Microsoft Teams. Formatting broke. Added Teams-specific formatting rules to the templates.
8. Added vault-aware mode, batch mode, and the `--loot` flag as usage revealed friction.

The whole story is in [Build Something Stupid](https://jamiebono.substack.com/), a post about learning AI tooling by building things that have no business value.

## What is Dungeon Crawler Carl?

[Dungeon Crawler Carl](https://www.mattdinniman.com/) by Matt Dinniman is a LitRPG book series about Earth being converted into a lethal dungeon crawl broadcast as reality TV for alien viewers. The System AI is the artificial intelligence running the dungeon. It narrates achievements with the tone of a sharp, mean friend who controls your fate. It is, against all odds, one of the most precisely voiced characters in contemporary fiction.

The books are available on Kindle and in audio. The audio performance by Jeff Hays is one of those rare cases where the narrator becomes inseparable from the text.

## About

Built by [Jamie Bono](https://jamiebono.substack.com/) as the single most educational and profoundly useless project he has built with AI tooling.

This skill follows the [Agent Skills open standard](https://agentskills.io) and works across multiple AI tools that support it. For distribution options beyond cloning, see [Claude Code plugins documentation](https://code.claude.com/docs/en/plugins).

## License

MIT
