# Loot Box Anatomy

When a crawler opens a loot box, the System AI describes the box, then reveals items one at a time. This is a separate comedic beat from the achievement — the achievement is the setup, the loot box is the payoff.

## Format

Output must be Teams-paste-friendly:
- NO markdown formatting (no `**bold**`, no `*italic*`). Unicode box-drawing characters (═, ╔, ╗, ╚, ╝, ★) are fine.
- BLANK LINE between every visual section — Teams collapses single line breaks. Each item name and its description must be separated by a blank line. No indentation (Teams eats leading spaces inconsistently).

```
╔═══════════════════════════════════════════════╗
You open your [Tier] [Custom Name] Box!
╚═══════════════════════════════════════════════╝

[Box description — 1-2 sentences.]

You have received the following items:

★ [Item Name] ([Rarity])

[Item description — 1-3 sentences. Mechanically describes
what it does, but the System AI can't resist editorializing.]

★ [Item Name] ([Rarity])

[Same format. 1-3 items per box.]
```

## Component Rules

### Box Description
- 1-2 sentences of thematic flavor
- Sensory details: what the box looks like, smells like, sounds like when opened
- Can foreshadow the items inside ("It smells faintly of regret and printer toner.")
- Tone matches the achievement — if the achievement was mocking, the box description continues the bit

### Item Names
- 2-5 words, title case
- Named like RPG items but mapped to the real-world situation
- Puns, compound words, and absurd specificity are encouraged
- Should be funny standalone, like the box name

### Item Rarity
- Common, Uncommon, Rare, Epic, Legendary
- Match roughly to the box tier (Bronze boxes give Common/Uncommon, Gold gives Rare/Epic, etc.)
- Rarity can be ironic — a "Common" item with a devastating description, or a "Legendary" item that's useless

### Item Descriptions
- 1-3 sentences each
- Mechanically describes what the "item" does in RPG terms
- Mapped to the real-world situation (a meeting achievement yields meeting-related items)
- The System AI editorializes: backhanded descriptions, warnings about side effects, or commentary on why you need this item in the first place
- Can reference the achievement that earned the box

## Item Count by Tier

| Box Tier | Items | Rarity Range |
|----------|-------|-------------|
| Bronze | 1 | Common |
| Silver | 1-2 | Common, Uncommon |
| Gold | 2 | Uncommon, Rare |
| Platinum | 2-3 | Rare, Epic |
| Celestial | 3 | Epic, Legendary |
| Legendary | 3 | Epic, Legendary |

## Mapping Real-World Situations to Items

The items should feel like RPG gear that addresses (or satirizes) the situation:

| Situation | Item Ideas |
|-----------|-----------|
| Budget overrun | Scroll of Retroactive Estimation, Cloak of Plausible Deniability, Abacus of Wishful Thinking |
| Meeting overload | Helm of Selective Deafness, Ring of Mandatory Attendance, Potion of Feigned Engagement |
| Scope creep | Shield of Original Requirements, Boots of Goalpost Migration, Amulet of "That Wasn't in the SOW" |
| Time tracking gaps | Hourglass of Lost Hours, Quill of Retroactive Logging, Bracers of Billable Ambiguity |
| Deadline miss | Scroll of Extension Request, Cape of Revised Timeline, Gauntlets of Apologetic Emailing |
| Client win | Trophy of Temporary Approval, Signet of Repeat Business, Elixir of Client Satisfaction (Expires Quickly) |
| Technical rabbit hole | Lantern of Stack Overflow, Tome of Deprecated Documentation, Compass of "It Works on My Machine" |

**Rule:** Items must be specific to the situation. Generic fantasy items ("Sword of Strength") are failures. The item name should make someone laugh before they even read the description.

## Denied Loot Boxes

If the achievement denied a reward, there is no loot box to open. Do not generate loot box content for denied-reward achievements.

## Tone

The loot box reveal continues whatever tone the achievement established. If the achievement was grudging respect, the items are grudgingly useful. If the achievement was gleeful mockery, the items are backhanded gifts. The System AI's personality doesn't reset between the achievement and the box opening — it's one continuous bit.
