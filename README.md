# *Heroes of Might and Magic III* improvement proposals

Scope: *Horn of the Abyss* with the *HD Mod* installed.

## Global UI

### `hip-0001` - Close every UI with `Esc`
Make every menu, dialog, and pop-up dismissible with `Esc`. For example, the artifact-selection pop-up opened by `Shift`-clicking an equipped `artifact` slot in the **Hero screen** cannot currently be closed with `Esc`.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

## Main menu UI

### `hip-0002` - Sort games on save date
Add a sortable **save date** column to the **Load Game** and **Save Game** screens.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0003` - Combine scenario filters and sorting
Add independent, combinable filters to the **Available Scenarios** screen, including a game/version filter for *Horn of the Abyss*, *The Shadow of Death*, *Armageddon's Blade*, and *Restoration of Erathia*. Filtering and sorting should be independent, so a player could show only `XL` *Horn of the Abyss* maps while sorting them by title.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

## Adventure Map UI

### `hip-0004` - Show newly learned town spells
Whenever a hero learns one or more `spells` from a town's `Mage Guild`, show a notification listing the newly learned `spells`, similar to the notification shown when heroes exchange `spells` through the `Scholar` secondary skill. Show it even when the hero visits the town without opening the **Town screen**.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0005` - Apply `Stables` bonuses automatically
Apply a `Castle` town's `Stables` movement bonus as soon as a hero visits the town, without requiring the player to open the **Town screen**. Still show a pop-up or another clear visual indication that the bonus was applied.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0006` - Preview next-day movement
Add a key modifier that previews how far the selected hero could travel on the following day from the hero's current tile, treating the hero's remaining `movement points` for the current day as zero. This would complement the existing modifier that displays movement costs for the current day and make next-day hero chains easier to plan.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0007` - Interrupt enemy-turn movement
Make the enemy-turn movement sequence interruptible. While enemy heroes are moving, allow the player to open the **in-game main menu**—for example, to load the **autosave** and correct an undefended town before ending the previous turn. This is especially important on maps with many opponents and heroes, where the sequence can take a long time at slower animation speeds.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0008` - Announce captured towns
Show a notification when an enemy captures one of the player's unguarded towns during the enemy turn. Consider making this notification configurable in the *HD Mod* settings.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0009` - Add an intermediate movement speed
Add an enemy-hero movement speed between the current **Fastest** setting and the next-slower setting.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0010` - Filter teleport destinations
Add text filtering to the `Town Portal` destination selector: typing `Mach`, for example, should show only a town named `Machina`, while typing `L` could show `Lanting` and `Lewindale`. Apply the same filtering to the `Inferno` `Castle Gate` destination selector if applicable.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0011` - Show enemy movement on the minimap
While the camera follows an enemy hero moving on the `Adventure Map`, indicate the viewed location on the minimap. This is particularly useful on `H`, `XH`, and other very large maps.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

## Hero UI — artifacts

These `backpack` features must not change the hero's equipped `artifacts`.

### `hip-0012` - Group artifacts by class
When `backpack` grouping is enabled, place identical `artifacts` together and organize them by the four `artifact classes`: `Treasure`, `Minor`, `Major`, and `Relic`. Show `combination artifacts` in a separate group, because they are not a fifth `artifact class`, and place classless `artifacts` such as `spell scrolls` in an **Unclassified** group.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0013` - Toggle backpack grouping
Add a toggle for grouping `artifacts` in the hero's `backpack`. When grouping is disabled, retain the original behavior and display `artifacts` in acquisition order.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0014` - Move all duplicate artifacts
Add a **Move all duplicates** action when transferring `artifacts` from the `backpack` to another hero.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0015` - Move all Minor artifacts
Add a **Move all Minor artifacts** action when transferring `artifacts` from the `backpack` to another hero.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0016` - Move all Major artifacts
Add a **Move all Major artifacts** action when transferring `artifacts` from the `backpack` to another hero.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0017` - Move all Relic artifacts
Add a **Move all Relic artifacts** action when transferring `artifacts` from the `backpack` to another hero.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0018` - Keep combination artifact components
Add a key modifier to the class-based bulk-transfer actions that retains `artifacts` that are components of `combination artifacts` instead of moving them to the other hero.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

## Kingdom Overview UI

### `hip-0019` - Expand Kingdom Overview
Scale the **Kingdom Overview** window to use the full screen at *HD Mod* resolutions.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

## Town UI

### `hip-0020` - Name the `Mana Vortex` recipient
In the `Mana Vortex` confirmation, explicitly name the hero whose `spell points` will be filled to twice their normal maximum and identify that hero as the visiting/guest hero when two heroes are in the `Dungeon` town.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0021` - Enter target resource amounts
Allow numeric keyboard input in the `Marketplace` to specify the desired amount of the target `resource`. For example, pressing `5` should request five `gems` and automatically calculate the required amount of the source `resource`; the target amount is the useful constant when the player is a few `resources` short of constructing a building such as the `Portal of Glory`.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

## Artifact selling and sacrifice UI

These proposals apply to `Artifact Merchants`, the `Altar of Sacrifice`, and the `Cove`'s `Grotto`.

### `hip-0022` - Show the entire artifact backpack
Expand the `backpack` view so all carried `artifacts` can be seen at once instead of showing only five at a time.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0023` - Group artifacts when selling or sacrificing
Reuse the **Hero UI**'s `backpack` grouping and ordering behavior in these interfaces.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0024` - Open the backpack from artifact slots
Allow the player to `Shift`-click an `artifact` slot to open the `backpack` in these interfaces.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

## Creature recruitment UI

### `hip-0025` - Enter recruitment quantities
Allow numeric keyboard input in **creature-recruitment screens**, whether opened in a town or at an `external dwelling`. For example, pressing `5` should set the number of `creatures` to recruit to five.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Trivial**

## Scenario restart behavior

### `hip-0026` - Clarify restart randomization
Make **Restart Scenario** handle randomized starting content consistently, or clearly explain the distinction. It currently rerolls a random artifact but retains the previously selected random hero, which is confusing.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

## Combat UI

### `hip-0027` - Show every active spell effect
Show every `spell` currently affecting a `creature stack`, rather than showing only a subset of its active `spell effects`.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0028` - Show own morale and luck sources
For each of the player's own `creature stacks`, show the exact `morale` and `luck` values together with a complete breakdown of the positive and negative sources contributing to each value. Do not show this source breakdown for enemy stacks, because it could reveal hidden information about the enemy hero's equipped `artifacts` or other modifiers.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0029` - Label every creature stack
Assign a stable, unique, single-character label to every `creature stack`: uppercase `A`–`T` for the attacking army and lowercase `a`–`t` for the defending army. Assign the next available label to every stack created during combat, including `Demons` summoned by `Pit Lords`, `Air Elementals`, `Earth Elementals`, `Fire Elementals`, and `Water Elementals` summoned by `spells`, and `Fangarms` raised by the `Horn of the Abyss` artifact. Annotate every `creature stack` with its label. For example:

* “Jotunn Warlords (`C`) take a defensive stance and gain +25 `Defense Skill`.”
* “Trolls (`b`) regenerate 40 hit points.”
* “War Mammoths (`D`) reach `Rune Level 6`.”

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0030` - Expand the combat log to full screen
Allow the **combat log** to expand across the full screen, even beyond the normal combat-window bounds. When reading the log, maximize the number of visible events.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

## Combat Log UI

### `hip-0031` - Color stack names by player
In the **combat log**, color every `creature stack` name using its controlling player's color. Use gray for neutral wandering monsters when there is no opposing hero.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Trivial**

### `hip-0032` - Structure the log by combat round
Add a header for each `combat round` and indent every event belonging to that round beneath it. Finish each round with an empty line before the next round's header.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0033` - Style hero and artifact events
In the **combat log**, color every hero name using that hero's player color and render the name in **bold**, including when the hero casts a `spell`. When a `combination artifact` produces a log event, color its name using the owning player's color and render it in *italics*.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0034` - Show spell level and school
For every `spell` cast during combat, show its casting proficiency—`Basic`, `Advanced`, or `Expert`. Render the `spell` name in *italics* and color it by its `school of magic`, matching the labels in the **Spell Book**: `Fire Magic` red, `Earth Magic` green, `Water Magic` blue, and `Air Magic` purple.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0035` - Toggle the combat log with `Enter`
Press `Enter` to show the **combat log**, and press `Enter` again to hide it.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Trivial**

### `hip-0036` - Identify attack sources and all targets
> [!IMPORTANT]
> **Depends on:** `hip-0029`

For every attack recorded in the **combat log**, identify the attacker and every affected `creature stack` using the labels from `hip-0029`. Report the damage and number of creatures that perish separately for each stack; do not collapse an area-of-effect attack into a combined total. Include secondary, adjacent, and friendly-fire targets, as well as affected stacks that take zero damage because of an immunity, and preserve the order in which the game resolves them.

For example: “Black Dragons (`F`) attack Black Dragons (`b`), inflicting 7,286 damage; 5 creatures perish. Dragon breath also hits Titans (`c`), inflicting 1,200 damage; 4 creatures perish.” Apply the same structure to `Heat Stroke`, `Death Cloud`, `Fireball Attack`, attacks against all adjacent stacks, and every other attack that can affect multiple stacks.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0037` - Name artifact-granted regeneration
> [!IMPORTANT]
> **Depends on:** `hip-0029`

When a living `creature stack` regenerates because its hero has the *Elixir of Life* equipped, identify the `combination artifact` as the source in the **combat log**. This distinguishes artifact-granted `Regeneration` from an innate creature ability. For example: “Azure Dragons (`b`) regenerate 50 hit points due to *Elixir of Life*.”

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0038` - Label every battlefield hex
Assign a stable coordinate to every `hex` on the battlefield. Use the format `row:column`: number the 11 rows from top to bottom, then number the 15 hexes within each row from left to right. For example, `1:3` identifies the third hex from the left in the top row. Display these coordinates on the battlefield grid and keep them unchanged regardless of terrain, obstacles, highlights, or occupying stacks.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Average**

### `hip-0039` - Log every battle-affecting action
> [!IMPORTANT]
> **Depends on:** `hip-0029`, `hip-0038`

Record every action or event that changes the battle state in the **combat log**, including movement, attacks and retaliations, spell casts and their effects, waiting, defending, and the creation of new `creature stacks`. Classify every entry as either `.info` or `.verbose`. Use `.info` for the classic combat-log events and outcomes that players should see by default. Use `.verbose` for the additional detail required to reconstruct the battle exactly using Cyon Combat Notation (`CCN`), including starting positions, exact movement paths, attack vectors, state counters, and complete resolved effects. Do not record interface interactions that leave the battle state unchanged; for example, opening and closing the **Spell Book** without casting a `spell` is not a battle action.

At the start of combat, record the starting coordinate of every `creature stack`. If a hero can rearrange stacks during the `Tactics phase`, record only each stack's final position when that phase ends; do not record intermediate rearrangements. The final `Tactics phase` position is the stack's starting position for combat.

Identify stacks using the labels from `hip-0029` and positions using the coordinates from `hip-0038`. For movement, record the destination hex. When a creature occupies two hexes, use its leftmost occupied hex as its position. For example, if Archangels (`b`) move to occupy `1:2` and `1:3`, log: “Archangels (`b`) move to hex `1:2`.”

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**

### `hip-0040` - Toggle combat-log detail
> [!IMPORTANT]
> **Depends on:** `hip-0039`

Add an **Info / Verbose** detail-level toggle to the **combat log**. Default to **Info**, which shows only `.info` entries in the classic style. **Verbose** shows both `.info` and `.verbose` entries, including details such as `creature stack` movement. Changing the level only filters the view; it must not change which events are recorded or exported.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**

### `hip-0041` - Add Cyon Combat Notation
> [!IMPORTANT]
> **Depends on:** `hip-0029`, `hip-0036`, `hip-0038`, `hip-0039`

Define Cyon Combat Notation (`CCN`), a versioned, canonical, machine-readable text format for recording an entire combat. Like a chess `FEN` position followed by a move score, a `CCN` record consists of a complete initial snapshot followed by an ordered action-and-effect stream. It must be deterministic, lossless, and compact: an independent implementation applying the statements in order must reproduce every intermediate state and the exact final state without consulting the saved game, animations, an RNG, or unrecorded engine state.

`CCN` records resolved facts, not how the game randomly selected them. Do not store an RNG seed, generator state, draw number, raw roll, or failed invisible roll. Instead, record every result that affects the battle: the chosen battlefield layout and obstacle hexes, exact `Quicksand` and `Land Mine` positions, selected targets and paths, triggered luck or morale, ability activations, damage, casualties, and resulting state. This keeps replay independent of engine version and RNG call order.

The canonical form is ASCII without whitespace. Every statement ends with `;`. Decimal integers are used for exact values, signed rational numbers use `numerator/denominator`, `-` means not applicable, and `*` means unlimited. A coordinate is `row:column`; a footprint or ordered area is `[coordinate,coordinate,...]`. The six directions are `E`, `NE`, `NW`, `W`, `SW`, and `SE`, with an optional decimal run length such as `E3NE2`. Identifiers contain only ASCII letters, digits, `_`, `.`, and `-`; custom display text is UTF-8 percent-encoded using uppercase hexadecimal bytes in the dictionary. Lists are enclosed in `[]` and retain their order.

Use this top-level grammar:

```text
record = "CCN1;" snapshot { round | phase | turn | event } result
round  = "r" integer ";"
phase  = "p" ("a" | "i" | "m" | "w") ";"
turn   = "t" entity ["+" | "-"] ";"
event  = level actor ":" opcode "(" [value {"," value}] ")"
         [">" effect {"," effect}] ";"
level  = "!" | "~"
uint   = "0" | nonzero-digit {digit}
int    = ["-"] uint
ratio  = int "/" nonzero-digit {digit}
hex    = uint ":" uint
id     = id-character {id-character}
entity = ("A"..."T") | ("a"..."t") | "HA" | "HD" | "@" id
list   = "[" [value {"," value}] "]"
text   = "'" {id-character | "%" hex-digit hex-digit} "'"
value  = int | ratio | hex | id | entity | list | text | "-" | "*"
```

`digit` is `0`–`9`, `nonzero-digit` is `1`–`9`, `hex-digit` is uppercase `0`–`9` or `A`–`F`, and `id-character` is an ASCII letter, digit, `_`, `.`, or `-`. A `text` value contains percent-encoded UTF-8 bytes. Context determines whether a numeric pair is a rational number or a coordinate: coordinates occur only in coordinate-typed fields, while rational numbers occur only in numeric-value fields. Core opcodes and effect names are case-sensitive.

`!` means `.info` and `~` means `.verbose`. `r12;` starts round 12, so following statements do not repeat the round number. `pa;`, `pi;`, `pm;`, and `pw;` start the automatic, initial-and-defend, morale-and-wait, and wait phases. Use `r0;pa;` for start-of-combat effects that occur after the final `Tactics phase` positions are known but before round 1. A turn marker such as `tF;` starts stack `F`'s normal activation, `tF+;` starts its extra positive-morale activation, and `tF-;` records that negative morale consumed its activation. The next turn, phase, round, or result statement closes the current activation.

Use uppercase `A`–`T` and lowercase `a`–`t` for stacks as defined by `hip-0029`, `HA` and `HD` for the attacking and defending heroes, and `@identifier` for `war machines`, siege structures, battlefield objects, and automatic actors. Snapshot statements have these exact field orders:

```text
h(game,hota,hd,rules-digest);
b(kind,terrain,magic-terrain,template,passability-mask,[global-state]);
s(side,hero,level,[attack,defense,power,knowledge],[skill:rank],specialty,
  [artifact],mana,[spell],casts-remaining,[temporary-bonus],formation);
u(id,side,type,count,top-hp,anchor,[footprint],facing,attack,defense,speed,
  morale,luck,shots,casts,retaliations,[state],[active-effect]);
o(id,type,[footprint],orientation,owner,visibility,duration,hp,[state]);
q([entity,entity,...]);
d(id,kind,[field:value,field:value,...]);
```

`h` identifies the exact game, *Horn of the Abyss*, and *HD Mod* builds plus the SHA-256 digest of the static rules registry, written as `sha256-` followed by 64 lowercase hexadecimal digits. `b` defines the battlefield, including field, siege, naval, `creature bank`, and other special templates. Its `passability-mask` contains the 165 battlefield bits in `1:1` through `11:15` row-major order, packed most-significant bit first into 21 bytes with the final three padding bits set to zero, then encoded as unpadded Base64url. `s` occurs once per side and uses `-` for an absent hero. `u` occurs for every stack, summon, clone, corpse, and `war machine`; `top-hp` is the remaining health of the top creature. `o` occurs for every obstacle, peril, wall, tower, gate, drawbridge, moat, `Fire Wall`, `Force Field`, `Quicksand`, `Land Mine`, and other battlefield object. `visibility` is `A`, `D`, `AD`, or `-` for attacker, defender, both, or neither. `q` is the initial ordered initiative queue. `d` declares custom or namespaced content not present in the rules registry; its fields are sorted by field name. Snapshot order is `h`, `b`, attacker `s`, defender `s`, all `d` statements sorted by ID, all `u` statements sorted by entity ID, all `o` statements sorted by object ID, then `q`.

Core action opcodes and their exact operands are:

```text
m(mode,start,path,end)
a(kind,target,target-hex,contact-hex,vector,[result-tag])
c(spell,proficiency,target,[result-tag])
x(ability,origin,vector,[ordered-area],target,[result-tag])
w()
d()
f(retreat|surrender)
```

Movement `mode` is `w`, `f`, `t`, or `b` for walking, flying, teleporting, or burrowing. `path` is a direction run or `-` when no intermediate hex is traversed. The resulting position effect always supplies the complete footprint and facing. Attack `kind` is `m`, `s`, `r`, or `p` for melee, shot, retaliation, or preemptive shot. `target-hex` is the selected hex of the target, `contact-hex` is the attacker's attacking hex, and `vector` is the ordered direction run from contact to target; ranged attacks retain the complete ray needed to reproduce wall interaction. A stack that moves and attacks has `m` followed by `a` in the same turn; a stack that attacks without moving has no intervening `m` event.

`c` records a hero or creature `spell`. `x` records every alternative, automatic, or activated ability using a stable namespaced identifier. A `Heat Stroke` event, for example, records `hota.heat_stroke`, its origin, chosen direction, complete ordered area, optional selected target, resolved luck tag, and all resulting damage effects. Dragon breath, `Death Cloud`, `Fireball Attack`, attacks against all adjacent stacks, double attacks, `Fire Shield`, regeneration, life drain, creature spellcasting, `Catapult` fire, and every other special mechanic use either the applicable core opcode or a namespaced `x` ability; they must never be approximated as an ordinary single-target attack.

The optional ordered `result-tag` list records resolved facts needed to reproduce behavior or presentation, such as `luck+`, `luck-`, `morale+`, `resisted`, `death-blow`, `no-retaliation`, or a namespaced ability result. It never contains probabilities or random numbers.

Effects are applied strictly from left to right and use these exact forms:

```text
D(entity,damage,perished,count-after,top-hp-after)
H(entity,healed,resurrected,count-after,top-hp-after)
P(entity,anchor,[footprint],facing)
C(entity,counter,value)
E+(entity,effect,source,duration,value)
E-(entity,effect,source)
N(u(...)|o(...))
R(entity-or-object)
V(object,visibility)
S(entity.field,value)
child = "^{" level actor ":" opcode "(" [value {"," value}] ")"
        [">" effect {"," effect}] "}"
```

`D` always names the affected stack and records the exact damage, number of creatures that perish, remaining count, and remaining health of the top creature. An area attack emits one `D` effect per affected stack in resolution order, including zero-damage results. `H` does the same for healing and resurrection. `P` changes position. `C` sets an absolute counter such as shots, creature casts, hero spell points, hero casts remaining, retaliations, preemptive shots, wait, or defend state. `E+` and `E-` add and remove a sourced effect. `N` creates a complete unit or object, `R` removes one, `V` changes hidden-object visibility, and `S` sets another registry-defined state field such as control, life state, siege health, gate position, or turn order. Absolute after-values make every record self-checking and prevent accumulated ambiguity.

The `^{...}` form embeds a complete `.info` or `.verbose` reactive child event at its exact point in an effect list; omit `>effects` inside the braces only when the child has no state effect. Use it when order matters within one action, such as a `Fire Shield` response from each stack hit by a Hydra, a retaliation between the first and second strikes of a double attack, or a triggered peril during movement. Child events may contain their own ordered effects and nested children, allowing any chain to be represented without inventing an RNG history.

For example, this pretty-printed fragment starts round 12, moves a two-hex stack east by two hexes, records its complete resulting footprint, then records a lucky melee attack and the defender's retaliation. Its canonical serialization removes the line breaks:

```text
r12;pi;tF;
~F:m(w,5:3,E2,5:5)>P(F,5:5,[5:5,5:6],E);
!F:a(m,b,5:7,5:6,E,[luck+])>D(b,7286,5,12,114);
!b:a(r,F,5:6,5:7,W,[])>D(F,900,0,20,100),C(b,retaliations,0);
```

No statement may omit a state change required for replay. This includes positions and facing; attacks and every individually damaged stack; damage, healing, casualties, resurrection, summoning, cloning, transformation, control, death, and corpses; shots, casts, spell points, retaliations, and extra actions; active effects, sources, durations, dispels, and immunities; obstacle creation, revelation, triggering, expiration, and removal; and `war machine`, wall, tower, gate, drawbridge, and moat state. The exact chosen hexes are recorded when `Quicksand`, `Land Mine`, `Remove Obstacle`, `Earthquake`, or another effect changes the battlefield. `Fire Shield` and similar reactive damage never consume a retaliation unless an explicit counter effect says so.

End the record with `z(winner,reason,[attacker-casualty],[defender-casualty],final-digest);`. Each casualty item is `entity:permanently-lost`; items are sorted by entity ID. `winner` is `A`, `D`, or `-`, and `reason` is a registry value such as `defeat`, `retreat`, or `surrender`. `final-digest` is `sha256-` followed by the lowercase SHA-256 digest of the final `s`, `u`, `o`, and `q` statements in canonical snapshot order. A parser must reject a record when an after-value, final casualty total, or final digest disagrees with the state produced by the preceding statements.

The `.verbose` **combat log** is a human-readable rendering of this structured stream; `CCN` must never be reconstructed by parsing prose. A valid exporter must reject or explicitly mark an incomplete record if any action, affected entity, ordered effect, or state transition cannot be represented. Extensions use namespaced identifiers and dictionary declarations, and readers preserve unknown extension data when round-tripping.

A full `CCN` record may contain hidden information needed for exact replay, including enemy `artifacts`, invisible perils, and unrevealed effects. Record that information internally, but do not expose it through the live **combat log** or a player-accessible export while it could affect an ongoing game. Public views must retain the existing information boundaries; full replay data may be revealed only when the combat is over and doing so cannot leak information relevant to continued play.

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Complex**
