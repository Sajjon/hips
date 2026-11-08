# Combat-log proof-of-concept prompt

Generated with the built-in image-generation tool from the screenshot supplied on 2026-11-07 and revised on 2026-11-08. The current image shows **Info**, with expert mass `'Slow'`, an indented resistance outcome, quoted spell names, and no movement or stack-creation detail. The transcript preserves the screenshot's primary damage figures; ownership assignments, round boundaries, labels, proficiency, and supplementary events are illustrative. This is a visual design proposal, not a reconstruction of the battle.

## Initial generation · 2026-11-07

This first prompt produced the earlier **Verbose** mockup. The revision below edits that image as committed in `74a09ff`.

```text
Use case: precise-object-edit / ui-mockup.
Asset type: repository proof-of-concept screenshot for Heroes of Might and Magic III with Horn of the Abyss and HD Mod.
Edit target: the attached screenshot at /Users/sajjon/Desktop/Screenshot 2026-11-07 at 08.04.27.png. Make ONE polished, highly readable screenshot edit, maintaining its landscape aspect ratio and resolution. Keep the original adventure map, game frame, sidebar, battlefield artwork and pixel-art visual identity wherever not covered by the redesigned modal. No modern app/dashboard styling, no callout arrows or external explanatory diagram.

PRIMARY EDIT: Replace the small central battle-log popup with an expanded, almost full-screen COMBAT LOG modal. It should extend beyond the original battle window into the adventure-map area, with a narrow strip of the recognizable source screenshot visible around it. Use the same ornate red/gold/beveled frame, dark brown leather/parchment background and crisp, light ivory game typography. Use the space for readable text, not enormous headings or decorative empty panels. Render at high resolution with sharp legible text. Rough panel bounds at original size: x=100 to 1870, y=90 to 1170. No clipping or horizontal truncation.

CONTROLS AND HIERARCHY: Compact title row "Combat Log"; right-hand native game buttons "Info", "Verbose", "Copy to clipboard", "Restore". Verbose is visibly selected. Next row a small ownership legend: "Lilith · Red" and "Indestructib · Purple", and a small spell-school legend with "Fire", "Earth", "Water", "Air" colored respectively red, green, blue, purple. A working-looking vertical scrollbar inside the right edge. Footer center button "Close [Enter]". Footer note in readable small muted type exactly: "POC: round boundaries, labels, positions and proficiency are illustrative." This is a demonstration, not a verified battle replay.

TYPOGRAPHY AND COLOR RULES (CRITICAL):
- Main narration and all damage/casualty numbers: light ivory for maximum contrast.
- Every occurrence of a RED army stack's full name AND its label: bright readable warm red/coral (#ff7068). RED stacks are Arch Devils (A), Phoenixes (B), Titans (C), Jotunn Warlords (D), Gold Dragons (E).
- Every occurrence of a PURPLE army stack's full name AND its label: bright readable lavender (#c995ff). PURPLE stacks are Azure Dragons (a), Steel Elves (b), Great Shamans (c), Jotunn Warlords (d), Jotunn Warlords (h). (h) is a newly created clone and must have a distinct lowercase label.
- Hero names Lilith and Indestructib: BOLD, in their own red or purple player color.
- Spell names: ITALIC, in their MAGIC SCHOOL color, irrespective of the owner's color. Prayer and Clone are WATER BLUE (#79baff). Fire Shield is FIRE RED (#ff9576). Names of spells are not all gold or all the owner's color.
- Elixir of Life: ITALIC and the owning player's red color.
- Round headers: gold, with a subtle horizontal rule. Round events indented below the header; reactive/secondary effect lines indented a second level. Leave a blank line between rounds.
- Add thousands separators to every large number in the new log.
- Coordinates use row:column; uppercase labels for attackers, lowercase for defenders. Keep letter case exact.
- Differentiate subtle verbose movement/creation lines by a muted small "Move" / "Create" prefix, but retain their stack name colors. Do not dump computer code or raw CCN syntax into this human-readable view.

TRANSCRIPT: Render the following compact log, in this exact order, with color/weight/italic rules applied to individual words as above. Indentation below is meaningful. It is fine to wrap a long line with a hanging indent; do NOT omit lines, reverse casualty attribution, or invent other numbers. All lines must fit comfortably at a legible game UI font size. Keep the original damage values. Two supplemental lines (movement and secondary breath) demonstrate verbose detail and multi-target damage.

ROUND 6
    Lilith casts Prayer [Expert · Water Magic].
    Phoenixes (B) defend and gain +24 Defense.
    Arch Devils (A) regenerate 50 HP due to Elixir of Life.
    Arch Devils (A) wait.

ROUND 7
    Move · Arch Devils (A): 3:2 → 3:4.
    Azure Dragons (a) attack Jotunn Warlords (D): 70,966 damage; 187 perish.
        Breath also hits Titans (C): 1,200 damage; 4 perish.
        Fire Shield on Jotunn Warlords (D) hits Azure Dragons (a): 59,307 damage; 47 perish.
        Jotunn Warlords (D) retaliate against Azure Dragons (a): 161 damage; 0 perish.
    Azure Dragons (a) reach Rune Level 6.
    Titans (C) attack Steel Elves (b): 5,988 damage; 476 perish.
    Steel Elves (b) attack Titans (C): 25,804 damage; 68 perish.
        Fire Shield on Titans (C) hits Steel Elves (b): 66,354 damage; 1,952 perish.
    Jotunn Warlords (D) regenerate 50 HP due to Elixir of Life.
    Jotunn Warlords (D) attack Great Shamans (c): 471 damage; 10 perish.
        Great Shamans (c) retaliate against Jotunn Warlords (D): 21,317 damage; 50 perish.
        Fire Shield on Jotunn Warlords (D) hits Great Shamans (c): 23,581 damage; 502 perish.
    Jotunn Warlords (d) regenerate 50 HP.
    Indestructib casts Clone [Expert · Water Magic] on Jotunn Warlords (d).
        Create · Jotunn Warlords (h), clone of (d), at 5:12.
    Jotunn Warlords (d) attack Phoenixes (B): 13,397 damage; 53 perish.
        Phoenixes (B) retaliate against Jotunn Warlords (d): 49 damage; 0 perish.
        Fire Shield on Jotunn Warlords (d) hits Phoenixes (B): 0 damage; fire immunity.
    Jotunn Warlords (d) reach Rune Level 9.
    Gold Dragons (E) regenerate 50 HP due to Elixir of Life.
    Bad luck affects Gold Dragons (E).
    Gold Dragons (E) attack Jotunn Warlords (d): 11,934 damage; 32 perish.

The reaction line with zero fire damage demonstrates explicit immunity reporting. Do not imply that ordinary dragon breath is a fire spell or that general spell immunity blocks reflected Fire Shield damage. Distinguish two Jotunn Warlord stacks (D) and (d) consistently.

Finish as a convincing native in-game screenshot, not a website. The combined log demonstrates expanded layout, round grouping, identity labels, owner colors, school-colored italic spells and proficiency, player-colored bold hero names, artifact attribution, damage-source/target clarity, explicit secondary and immunity outcomes, movement/creation events, Info/Verbose, copying, Enter dismissal, and thousands separators. Do not add unrelated gameplay panels or reveal enemy equipment.
```

## Revision · 2026-11-08

```text
Edit the supplied combat-log proof-of-concept image. This image is the edit target, not merely a style reference. Preserve the exact existing screenshot composition, ornate game frame, brown texture, UI layout, typography, title, colors, round headings, legend, copy/restore/close controls, event order, and every damage/casualty figure. Make only the following changes and the small vertical reflow they require. Do not redesign or enlarge the modal.

1. In ROUND 6 replace the first event with exactly:
"Lilith casts 'Slow' [Expert · Earth Magic · Mass]."
Lilith remains bold red. The spell text 'Slow', including its surrounding straight single quote marks, is italic and EARTH GREEN, matching the green Earth legend. The Earth Magic label should also use green, matching the existing school-label treatment. Expert and Mass are ivory.
Directly below this cast, indent a reactive outcome line one level deeper than the cast:
"Crystal dragons (e) and Black dragons (g) resist the spell."
Render "Crystal dragons (e)" and "Black dragons (g)" in the same purple used for all defending stacks; leave "and" and "resist the spell." ivory. Keep lowercase labels (e) and (g) exact. This line belongs under the Slow event, not under the round heading as a peer event.
Remove Prayer completely from the image.

2. In every log event put ALL SPELL NAMES in straight single quotes while keeping their existing italic and magic-school colors. Replace every "Fire Shield" with "'Fire Shield'" (italic fire-red) and "Clone" with "'Clone'" (italic water-blue). Slow above is green, Clone blue, Fire Shield fire-red. Do NOT quote artifact names: Elixir of Life remains italic owner-red without added quotation marks. Do not quote school names, creature names, ability names or the spell-school legend.

3. Select "Info" at the top instead of "Verbose". Move the gold checkmark and active gold highlight to the Info button. Verbose must have no checkmark and the same inactive appearance as the old Info button. Keep BOTH buttons and their labels.

4. The Info view must omit verbose movement and creation detail. REMOVE these two complete rows without leaving gaps:
"Move · Arch Devils (A): 3:2 → 3:4."
"Create · Jotunn Warlords (h), clone of (d), at 5:12."
Do not display tile coordinates or movement/creation detail elsewhere. Keep the normal Clone cast event, damage events, secondary-breath damage, resistances, immunity, waits, defense, regeneration, rune levels, and all other existing rows. Keep their values and ownership colors exactly. Reflow upward just enough to close the two deleted rows and accommodate the added resistance line. Preserve the clear blank separator between ROUND 6 and ROUND 7.

5. Update only the small footer's illustrative note to:
"POC: round boundaries, labels and proficiency are illustrative. This is a demonstration, not a verified battle replay."
Keep it readable and preserve "Close [Enter]".

Check text carefully: 'Slow' is Expert Earth and Mass, 'Clone' Expert Water, all 4 existing 'Fire Shield' rows quoted, Crystal dragons (e) and Black dragons (g) purple, Info selected, Verbose unselected, NO Move row, NO Create row, NO tile coordinates. No spelling mistakes, no altered numbers, no added events or columns. Produce a crisp faithful image edit, not a new interpretation.
```
