# Achievement Anatomy

Every DCC achievement follows a consistent notification structure. This file defines the format, tiers, and naming conventions.

## Format

Output must be Teams-paste-friendly:
- NO markdown formatting (no `**bold**`, no `*italic*`). Use UPPERCASE for emphasis in titles and the achievement header.
- Unicode box-drawing characters (═, ╔, ╗, ╚, ╝, ★) are fine — they render correctly in Teams.
- BLANK LINE between every visual section. Teams collapses single line breaks, so every paragraph/section boundary needs a double newline. No indentation on content lines (Teams eats leading spaces inconsistently).
- The reward line should have a blank line before AND after the closing ═══ bar.

```
═══════════════════════════════════════════════
NEW ACHIEVEMENT!
[ACHIEVEMENT TITLE IN CAPS]!
═══════════════════════════════════════════════

[Trigger line — one or two sentences stating what the crawler did
to earn this. Factual but already dripping with judgment.]

[System AI commentary — 2-5 sentences. This is the main event.
The sarcasm, the rhetorical questions, the false reassurance,
the tangents. See system-ai-voice.md for patterns.]

Reward: You've received a [Tier] [Custom Name] Box!

═══════════════════════════════════════════════
```

### Component Rules

**Achievement Title:**
- 2-6 words
- Often a pun, pop culture reference, nursery rhyme twist, or darkly ironic phrase
- Exclamation marks are common but not required
- Can be a quote, a command, a noun phrase, or a question
- Should be memorable enough to reference later

**Trigger Line:**
- States the mechanical fact of what was done
- Written in second person ("You have...")
- Often includes a specific number or threshold ("more than five", "six or more")
- Already slightly loaded — the word choice hints at the commentary to come

**System AI Commentary:**
- The soul of the achievement. 2-5 sentences.
- Must use at least one signature device from system-ai-voice.md (rhetorical question, setup-undercut, false compliment, tangent, or confessional)
- Specific to the situation — not generic snark that could apply to anything
- Ends on the strongest beat. The last sentence should land.

**Reward Line:**
- Always formatted: `**Reward: You've received a [Tier] [Custom Name] Box!**`
- Exception: some achievements deny rewards entirely ("Bitches don't get rewards." / "Reward: You're totally going to hell.")
- Denied rewards are funny but use them sparingly — max 1 in 5

## Loot Box Tiers

Six tiers, matching the severity/impressiveness of the achievement:

| Tier | When to Use | Examples |
|------|-------------|---------|
| **Bronze** | Minor everyday moments, small competencies | Reading a sign, basic combat, mundane tasks |
| **Silver** | Notable accomplishments, early milestones | First 5000 to enter, first kill with bare hands |
| **Gold** | Major wins or spectacular moral failures | War Criminal, significant boss kills |
| **Platinum** | Exceptional feats, career-defining moments | Surviving impossible odds, massive viewer counts |
| **Celestial** | Mythic-tier, reality-breaking achievements | Apex Predator, system-level accomplishments |
| **Legendary** | One-of-a-kind, first-ever accomplishments | First crawler with a cat, unprecedented feats |

**For real-world achievements:** Bronze and Silver are your bread and butter. Gold for genuinely impressive (or impressively bad) things. Platinum for career-level moments. Celestial and Legendary should be rare — maybe 1 in 20 achievements.

## Custom Box Names

The box name is thematically tied to the achievement. This is a creative opportunity — get specific.

### Naming Patterns from the Books

| Achievement Type | Box Name Pattern | Examples |
|-----------------|-----------------|---------|
| Combat/violence | Weapon or warrior themed | Weapon Box, Predator Box |
| Moral failure | Insult-based | Asshole's Box, (no reward — "going to hell") |
| Luck/survival | Fortune-based | Lucky Bastard Box |
| Pets/companions | Pet-themed | Pet Box |
| Popularity/fame | Fan-themed | Fan Box |
| Feet-related | Footwear-themed | Shoe Box |
| Exploration | Adventure-themed | Adventurer Box |
| Power/dominance | Authority-themed | Tyrant's Box |

### For Real-World Achievements

Extend the pattern to consulting/work contexts:

| Achievement Type | Box Name Ideas |
|-----------------|---------------|
| Meeting overload | Meeting Martyr's Box, Calendar Hostage's Box |
| Time tracking | Timesheet Purgatory Box, Billable Hour Hoarder's Box |
| Deadline survival | Deadline Dodger's Box, Last-Minute Larry's Box |
| Scope creep | Scope Creep Survivor's Box, Moving Goalpost Box |
| Email management | Inbox Zero Mythologist's Box, Reply-All Victim's Box |
| Code/tech work | Stack Overflow Pilgrim's Box, Config File Casualty's Box |
| Client work | Client Whisperer's Box, SOW Shapeshifter's Box |
| Procrastination | Procrastinator's Box, Tomorrow's Hero Box |
| Over-engineering | Premature Optimizer's Box, Yak Shaver's Box |

**Rule:** Never use a generic name. "Achievement Box" or "Reward Box" are failures. The name should make someone laugh on its own.

## Special Achievement Types

### The Denied Reward

Some achievements give no loot box. Instead, the reward line IS the joke:

- "Bitches don't get rewards."
- "Reward: You're totally going to hell."
- "Reward: Those past twenty seconds, when your conscience started to ease? That was your reward."

Use sparingly. The denied reward works best for moral failures or situations where the crawler was passive/victimized.

### The Meta-Achievement

The System AI occasionally gives achievements about itself or about the achievement system:

- "Mass Layoffs!" — The System AI talks about its own therapy
- Achievements that reference previous achievements
- Commentary about the ratings or viewer reactions

These work well for vault-aware mode when the System AI can reference patterns across multiple situations.

### The Backhanded Compliment Achievement

Grudging respect disguised as an insult. The title sounds positive, the commentary reveals the System AI is impressed despite itself:

- "Not bad. Not good, but not bad. Which, given your track record, is basically a miracle."
- Title: "Competence?!" — expressing genuine shock that you did something right
