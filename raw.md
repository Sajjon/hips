# Heroes of Might and Magic III improvement proposals

Scope: Horn of the Abyss with the HD Mod installed.

## Global UI

## `hip-0001`

Make every menu, dialog, and pop-up dismissible with `Esc`. For example, the artifact-selection pop-up opened by Shift-clicking an equipped-artifact slot in the Hero screen cannot currently be closed with `Esc`.

## Main menu UI

## `hip-0002`

Add a sortable **save date** column to the Load Game and Save Game screens.
## `hip-0003`

Add independent, combinable filters to the Available Scenarios screen, including a game/version filter for Horn of the Abyss, The Shadow of Death, Armageddon's Blade, and Restoration of Erathia. Filtering and sorting should be independent, so a player could show only XL Horn of the Abyss maps while sorting them by title.

## Adventure Map UI

## `hip-0004`

Whenever a hero learns one or more spells from a town's Mage Guild, show a notification listing the newly learned spells, similar to the notification shown when heroes exchange spells through the Scholar skill. Show it even when the hero visits the town without opening the Town screen.
## `hip-0005`

Apply a Castle town's Stables movement bonus as soon as a hero visits the town, without requiring the player to open the Town screen. Still show a pop-up or another clear visual indication that the bonus was applied.
## `hip-0006`

Add a key modifier that previews how far the selected hero could travel on the following day from the hero's current tile, treating the hero's remaining movement points for the current day as zero. This would complement the existing modifier that displays movement costs for the current day and make next-day hero chains easier to plan.
## `hip-0007`

Make the enemy-turn movement sequence interruptible. While enemy heroes are moving, allow the player to open the in-game main menu—for example, to load the autosave and correct an undefended town before ending the previous turn. This is especially important on maps with many opponents and heroes, where the sequence can take a long time at slower animation speeds.
## `hip-0008`

Show a notification when an enemy captures one of the player's unguarded towns during the enemy turn. Consider making this notification configurable in the HD Mod settings.
## `hip-0009`

Add an enemy-hero movement speed between the current **Fastest** setting and the next-slower setting.
## `hip-0010`

Add text filtering to the Town Portal destination selector: typing `Mach`, for example, should show only a town named `Machina`, while typing `L` could show `Lanting` and `Lewindale`. Apply the same filtering to the Inferno Castle Gate destination selector if applicable.
## `hip-0011`

While the camera follows an enemy hero moving on the Adventure Map, indicate the viewed location on the minimap. This is particularly useful on H, XH, and other very large maps.

## Hero UI — artifacts

These backpack features must not change the hero's equipped artifacts.

## `hip-0012`

Add a toggle for grouping artifacts in the hero's backpack. When grouping is disabled, retain the original behavior and display artifacts in acquisition order.
## `hip-0013`

When backpack grouping is enabled, place identical artifacts together and organize them by the four artifact classes: Treasure, Minor, Major, and Relic. Show combination artifacts in a separate group, because they are not a fifth artifact class, and place classless artifacts such as spell scrolls in an **Unclassified** group.
## `hip-0014`

Add a **Move all duplicates** action when transferring backpack artifacts to another hero.
## `hip-0015`

Add a **Move all Minor artifacts** action when transferring backpack artifacts to another hero.
## `hip-0016`

Add a **Move all Major artifacts** action when transferring backpack artifacts to another hero.
## `hip-0017`

Add a **Move all Relic artifacts** action when transferring backpack artifacts to another hero.
## `hip-0018`

Add a key modifier to the class-based bulk-transfer actions that retains artifacts that are components of combination artifacts instead of moving them to the other hero.

## Kingdom Overview UI

## `hip-0019`

Scale the Kingdom Overview window to use the full screen at HD Mod resolutions.

## Town UI

## `hip-0020`

In the Mana Vortex confirmation, explicitly name the hero whose spell points will be filled to twice their normal maximum and identify that hero as the visiting/guest hero when two heroes are in the Dungeon town.
## `hip-0021`

Allow numeric keyboard input in the Marketplace to specify the desired amount of the target resource. For example, pressing `5` should request five gems and automatically calculate the required amount of the source resource; the target amount is the useful constant when the player is a few resources short of constructing a building such as the Portal of Glory.

## Artifact selling and sacrifice UI

These proposals apply to Artifact Merchants, the Altar of Sacrifice, and the Cove's Grotto.

## `hip-0022`

Expand the backpack view so all carried artifacts can be seen at once instead of showing only five at a time.
## `hip-0023`

Reuse the Hero UI's backpack grouping and ordering behavior in these interfaces.
## `hip-0024`

Allow the player to Shift-click an artifact slot to open the backpack in these interfaces.

## Creature recruitment UI

## `hip-0025`

Allow numeric keyboard input in creature-recruitment screens, whether opened in a town or at an external dwelling. For example, pressing `5` should set the number of creatures to recruit to five.

## Scenario restart behavior

## `hip-0026`

Make **Restart Scenario** handle randomized starting content consistently, or clearly explain the distinction. It currently rerolls a random artifact but retains the previously selected random hero, which is confusing.

## Combat UI

## `hip-0027`

Improve battle-log readability by color-coding different event types and using formatting such as bold and italics where appropriate.
## `hip-0028`

Show every spell currently affecting a creature stack, rather than showing only a subset of its active spell effects.
## `hip-0029`

Show each creature stack's exact morale and luck values, together with a complete breakdown of the positive and negative sources contributing to each value.
