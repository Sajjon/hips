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

### `hip-0036` - Identify attack sources and targets
> [!IMPORTANT]
> **Depends on:** `hip-0029`

For every attack between `creature stacks` recorded in the **combat log**, identify both the attacker and the target using the labels from `hip-0029`. For example: “Black Dragons (`F`) attack Black Dragons (`b`), inflicting 7,286 damage; 5 creatures perish.”

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Trivial**

### `hip-0037` - Name artifact-granted regeneration
> [!IMPORTANT]
> **Depends on:** `hip-0029`

When a living `creature stack` regenerates because its hero has the *Elixir of Life* equipped, identify the `combination artifact` as the source in the **combat log**. This distinguishes artifact-granted `Regeneration` from an innate creature ability. For example: “Azure Dragons (`b`) regenerate 50 hit points due to *Elixir of Life*.”

> **Author:** Alexander Cyon · **Date:** 2026-10-10 · **Status:** **DRAFT** · **Estimate:** **Simple**
