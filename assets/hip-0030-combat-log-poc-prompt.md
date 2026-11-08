# Combat-log proof-of-concept prompt

Current image specification for the built-in image-generation tool. The mockup shows **Info**, with expert `'Slow'`, school-first spell labels, **Unknown Level** for the opposing cast, an indented resistance outcome, quoted spell names, and no movement or stack-creation detail. The player's legend reads **Lilith · Red (You)**. The transcript preserves the source screenshot's primary damage figures; ownership assignments, round boundaries, labels, proficiency, and supplementary events are illustrative. This is a visual design proposal, not a reconstruction of the battle.

```text
Use case: precise-object-edit / ui-mockup.
Asset type: repository proof-of-concept screenshot for Heroes of Might and Magic III with Horn of the Abyss and HD Mod.
Edit target: the attached screenshot at assets/hip-0030-combat-log-reference.png. Make ONE polished, highly readable screenshot edit, maintaining its landscape aspect ratio and resolution. Keep the original adventure map, game frame, sidebar, battlefield artwork and pixel-art visual identity wherever not covered by the redesigned modal. No modern app/dashboard styling, no callout arrows or external explanatory diagram.

PRIMARY EDIT: Replace the small central battle-log popup with an expanded, almost full-screen COMBAT LOG modal. It should extend beyond the original battle window into the adventure-map area, with a narrow strip of the recognizable source screenshot visible around it. Use the same ornate red/gold/beveled frame, dark brown leather/parchment background and crisp, light ivory game typography. Use the space for readable text, not enormous headings or decorative empty panels. Render at high resolution with sharp legible text. Rough panel bounds at original size: x=100 to 1870, y=90 to 1170. No clipping or horizontal truncation.

CONTROLS AND HIERARCHY: Compact title row "Combat Log"; right-hand native game buttons "Info", "Verbose", "Copy to clipboard", "Restore". Info is visibly selected; Verbose is inactive. Next row a small ownership legend: "Lilith · Red (You)" and "Indestructib · Purple", and a small spell-school legend with "Fire", "Earth", "Water", "Air" colored respectively red, green, blue, purple. Keep the ownership labels spaced apart without overlap. A working-looking vertical scrollbar inside the right edge. Footer center button "Close [Enter]". Footer note in readable small muted type exactly: "POC: round boundaries, labels and proficiency are illustrative. This is a demonstration, not a verified battle replay."

TYPOGRAPHY AND COLOR RULES (CRITICAL):
- Main narration and all damage/casualty numbers: light ivory for maximum contrast.
- Every occurrence of a RED army stack's full name AND its label: bright readable warm red/coral (#ff7068). RED stacks are Arch Devils (A), Phoenixes (B), Titans (C), Jotunn Warlords (D), Gold Dragons (E).
- Every occurrence of a PURPLE army stack's full name AND its label: bright readable lavender (#c995ff). PURPLE stacks are Azure Dragons (a), Steel Elves (b), Great Shamans (c), Jotunn Warlords (d), Crystal dragons (e), Black dragons (g).
- Hero names Lilith and Indestructib: BOLD, in their own red or purple player color.
- Spell names: ITALIC, in their MAGIC SCHOOL color, irrespective of the owner's color. Enclose every spell name in straight single quotes. 'Slow' is EARTH GREEN; 'Clone' is WATER BLUE (#79baff); 'Fire Shield' is FIRE RED (#ff9576). Names of spells are not all gold or all the owner's color.
- Cast labels put the school before proficiency. Use exactly [Earth Magic • Expert level] for Lilith's 'Slow' and [Water · Unknown Level] for Indestructib's 'Clone'. Color the school by magic type; proficiency text is ivory. Do not add Mass to the Slow label or replace Unknown Level with hidden proficiency information about the opposing hero.
- Elixir of Life: ITALIC and the owning player's red color.
- Round headers: gold, with a subtle horizontal rule. Round events indented below the header; reactive/secondary effect lines indented a second level. Leave a blank line between rounds.
- Add thousands separators to every large number in the new log.
- Use uppercase labels for attackers and lowercase for defenders. Keep letter case exact.
- Info mode omits tile coordinates, movement rows, and detailed stack-creation rows. Do not dump computer code or raw CCN syntax into this human-readable view.

TRANSCRIPT: Render the following compact log, in this exact order, with color/weight/italic rules applied to individual words as above. Indentation below is meaningful. It is fine to wrap a long line with a hanging indent; do NOT omit lines, reverse casualty attribution, or invent other numbers. All lines must fit comfortably at a legible game UI font size. Keep the original damage values. The supplementary breath line demonstrates separate reporting for multiple targets.

ROUND 6
    Lilith casts 'Slow' [Earth Magic • Expert level].
        Crystal dragons (e) and Black dragons (g) resist the spell.
    Phoenixes (B) defend and gain +24 Defense.
    Arch Devils (A) regenerate 50 HP due to Elixir of Life.
    Arch Devils (A) wait.

ROUND 7
    Azure Dragons (a) attack Jotunn Warlords (D): 70,966 damage; 187 perish.
        Breath also hits Titans (C): 1,200 damage; 4 perish.
        'Fire Shield' on Jotunn Warlords (D) hits Azure Dragons (a): 59,307 damage; 47 perish.
        Jotunn Warlords (D) retaliate against Azure Dragons (a): 161 damage; 0 perish.
    Azure Dragons (a) reach Rune Level 6.
    Titans (C) attack Steel Elves (b): 5,988 damage; 476 perish.
    Steel Elves (b) attack Titans (C): 25,804 damage; 68 perish.
        'Fire Shield' on Titans (C) hits Steel Elves (b): 66,354 damage; 1,952 perish.
    Jotunn Warlords (D) regenerate 50 HP due to Elixir of Life.
    Jotunn Warlords (D) attack Great Shamans (c): 471 damage; 10 perish.
        Great Shamans (c) retaliate against Jotunn Warlords (D): 21,317 damage; 50 perish.
        'Fire Shield' on Jotunn Warlords (D) hits Great Shamans (c): 23,581 damage; 502 perish.
    Jotunn Warlords (d) regenerate 50 HP.
    Indestructib casts 'Clone' [Water · Unknown Level] on Jotunn Warlords (d).
    Jotunn Warlords (d) attack Phoenixes (B): 13,397 damage; 53 perish.
        Phoenixes (B) retaliate against Jotunn Warlords (d): 49 damage; 0 perish.
        'Fire Shield' on Jotunn Warlords (d) hits Phoenixes (B): 0 damage; fire immunity.
    Jotunn Warlords (d) reach Rune Level 9.
    Gold Dragons (E) regenerate 50 HP due to Elixir of Life.
    Bad luck affects Gold Dragons (E).
    Gold Dragons (E) attack Jotunn Warlords (d): 11,934 damage; 32 perish.

The reaction line with zero fire damage demonstrates explicit immunity reporting. Do not imply that ordinary dragon breath is a fire spell or that general spell immunity blocks reflected Fire Shield damage. Distinguish two Jotunn Warlord stacks (D) and (d) consistently.

Finish as a convincing native in-game screenshot, not a website. The combined log demonstrates expanded layout, round grouping, identity labels, owner colors, school-colored italic spells and proficiency, player-colored bold hero names, artifact attribution, damage-source/target clarity, explicit secondary and immunity outcomes, Info/Verbose, copying, Enter dismissal, and thousands separators. Do not add unrelated gameplay panels or reveal enemy equipment.
```
