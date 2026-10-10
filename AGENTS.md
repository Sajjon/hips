# Repository guidance

## Purpose

This repository maintains improvement proposals for *Heroes of Might and Magic III* with *Horn of the Abyss* and the *HD Mod*. `README.md` is the proposal catalogue and source of truth.

## Proposal format

- Organize categories under level-two headings (`##`) and individual proposals under level-three headings (`###`).
- Give every proposal a globally unique, sequential ID in the form `hip-NNNN`. Derive the next ID from `README.md`; do not reuse or renumber an existing ID unless the user explicitly requests it.
- Use a short, descriptive title: ``### `hip-NNNN` - Title``.
- Put the proposal text directly below its heading. Explain the desired behavior precisely enough to distinguish it from current game behavior.
- When one proposal depends on another, put this block immediately below its heading:

  ```markdown
  > [!IMPORTANT]
  > **Depends on:** `hip-NNNN`
  ```

- End every proposal with this metadata footer, using the proposal's creation date and one of the four allowed estimates:

  ```markdown
  > **Author:** Alexander Cyon · **Date:** YYYY-MM-DD · **Status:** **DRAFT** · **Estimate:** **Trivial|Simple|Average|Complex**
  ```

- Leave exactly one blank line before each heading. Put a proposal's first content line directly below its heading, separate its subsequent blocks with one blank line, and end every text file with a newline.

## Language and styling

- Correct spelling and grammar while preserving the proposal's intent.
- Italicize game and expansion names, such as *The Shadow of Death* and *Horn of the Abyss*.
- Use **bold** for visible UI labels, screens, and actions.
- Use inline code for game concepts, mechanics, object names, key names, identifiers, and values, such as `Scholar`, `artifact`, `Regeneration`, and `Esc`.
- Keep titles short and proposal descriptions concrete. Include examples when they remove ambiguity.

## Accuracy

- Understand every proposal before editing it. Verify game mechanics and canonical terminology against the relevant pages on the [Heroes 3 wiki](https://heroes.thelazy.net/index.php/Main_Page); do not rely only on memory.
- Preserve information boundaries. In particular, detailed `morale` and `luck` sources are shown only for the player's own stacks so enemy artifacts remain hidden.
- The four `artifact classes` are `Treasure`, `Minor`, `Major`, and `Relic`. `Combination artifacts` are a separate category, and `spell scrolls` are classless.
- *Elixir of Life* is a `combination artifact` that gives living creatures `Regeneration`, which restores at most 50 health. Trolls have innate `Regeneration`; Azure Dragons regenerate only when an effect such as *Elixir of Life* grants it.
- `Runes` allows at most 3, 6, or 9 `Rune Levels` at `Basic`, `Advanced`, or `Expert` proficiency, respectively.
- The stack-label proposal uses uppercase `A`–`T` for the attacking army and lowercase `a`–`t` for the defending army, including stacks created during combat.

## Validation

- Run `pre-commit run --all-files` before committing. The hook and CI both run the Rust-based `typos` CLI.
- Run `git diff --check`.
- Confirm that proposal IDs are unique and sequential, and that the proposal-heading count equals the metadata-footer count.
- Treat reported spelling mistakes as defects. Add an entry to `_typos.toml` only after confirming that it is a genuine project-specific term or other false positive; keep every exception as narrow as possible.

## Commits

Use Conventional Commits, such as `docs: add combat log proposal` or `ci: add typo checks`.
