# Layout Guide

This guide defines the shared structure for the `via-layouts/*/README.md` files and their matching `*.layout.json` files.

## Source Of Truth

- The `*.layout.json` file is the source of truth for macro slot order.
- The README documents the same layout in human-readable form.
- Any macro slot change must be reflected in both places.
- The `macros` array must always contain exactly 16 entries (`M0` through `M15`).
- Never delete empty trailing slots; keep placeholders so slot numbers stay stable.

## Required README Order

1. Title and short description
2. Reference diagram
3. Layer 0 table
4. Layer 1 table
5. Encoder table
6. Macros table

## Reference Diagram

Use the same diagram in every layout README:

```text
┌────────┬────────┬───────┬───────┐
│ Knob 1 │        │ Key 1 │ Key 2 │
├────────┼────────┼───────┼───────┤
│ Knob 2 │ Key 3  │ Key 4 │ Key 5 │
├────────┼────────┼───────┼───────┤
│        │ Key 6  │ Key 7 │ Key 8 │
└────────┴────────┴───────┴───────┘
```

## Layer Tables

- Layer tables should use `Key 1` through `Key 8`.
- Use `M# (action result)` for keys that trigger macros.
- Use the action result text, not the raw command, in the layer tables.
- Keep the layer tables aligned across all layout READMEs.

Example:

- `M0 (Take screenshot)`
- `M5 (Toggle HDR in Windows 11)`

## Encoder Table

- Use one encoder table for all READMEs.
- Keep the same row labels in every file.
- Use `—` when a control has no mapping on a layer.

Suggested format:

| Control | Layer 0 | Layer 1 |
| --- | --- | --- |
| `Knob 1 rotate` | `...` | `...` |
| `Knob 1 press` | `...` | `—` |
| `Knob 2 rotate` | `...` | `...` |
| `Knob 2 press/hold` | `...` | `—` |

## Macros Table

- Put the macros table at the end of the README.
- List all 16 slots from `M0` to `M15`.
- Keep the command column aligned with the JSON slot order.
- Mark unused slots as `Unused`.
- If a slot is unused, keep the entry and mark it `Unused` instead of removing it.

## Validation

Run this check before finishing layout changes:

```bash
jq '.macros | length' via-layouts/*/*.layout.json
```

Each file should report `16`.

## Sync Rules

- If a macro is added, removed, or shifted, update the JSON array and the README together.
- Keep the `macros` array length at 16.
- If a command is duplicated by design, document it clearly in the README.
- If a command is moved to a new slot, update all layer references that point to it.
