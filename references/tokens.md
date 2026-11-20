# SkillSwap — Design tokens

Source file: `SkillSwap (Copy)` — file key `6RJxzF2lBjRd0QTyi7D4Tq`
Read from Figma on 2026-11-20 via the Plugin API (`use_figma`, read-only).

## Variable collections

| Collection | Collection id | Collection key | Modes | Variables |
|---|---|---|---|---|
| `Colors` | `VariableCollectionId:1:957` | `af0f74218f329143479781c39f96bbc0758e74f1` | `Mode 1` | 7 |
| `Spacing` | `VariableCollectionId:10:18` | `e243f8e70506acf46471aa4a4c02aa77a37376ff` | `Mode 1` | 7 |

Only one mode (`Mode 1`) exists in both collections, so there are no light/dark variants.

## Colors (type COLOR)

| Variable | Value | Variable id | Variable key |
|---|---|---|---|
| `bg/page` | `#F8FAFC` | `VariableID:10:11` | `ab1a6bf0186c8e0852792d0e473149c8d0c37cbc` |
| `bg/card` | `#FFFFFF` | `VariableID:10:12` | `efbdd7d2f5f228eddf46b1f841eb39be00b613f1` |
| `text/primary` | `#111827` | `VariableID:10:13` | `9509e93bcf0e4793c26605663ed6abaa129826a0` |
| `text/secondary` | `#6B7280` | `VariableID:10:14` | `f3577995a2db125d0df38db11af36cb30bccda7c` |
| `brand/primary` | `#2563EB` | `VariableID:10:15` | `ece8c6b765ecb6dde0947f1bb6be60bfbc232a67` |
| `brand/swap` | `#0D9488` | `VariableID:10:16` | `da360c09407aa8d33824ceaf9d6a595595bfc4cd` |
| `border/default` | `#E5E7EB` | `VariableID:10:17` | `ff212d3c6df45352df5a103ec21f1ea976ef0d2f` |

## Spacing, radius and height (type FLOAT, px)

| Variable | Value | Variable id | Variable key |
|---|---|---|---|
| `space/4` | 4 | `VariableID:10:35` | `5d3e0f7225773a61b1a33e4164a8df19e3b26216` |
| `space/8` | 8 | `VariableID:10:36` | `b65ce67261433c18b8b91c8ebe9c8a8d5d2ad6d6` |
| `space/12` | 12 | `VariableID:10:37` | `68329459dd9075e7736d588696584d39a7200511` |
| `space/16` | 16 | `VariableID:10:38` | `f7e2645acae34a06fdd3d9a23e72c47af176b23c` |
| `space/24` | 24 | `VariableID:10:39` | `3dabe914383cff99707ee5e65391bd09ab90db9d` |
| `radius/md` | 12 | `VariableID:10:40` | `7c104af1675e070d241b88ee9b92ced0afce8718` |
| `height/m` | 40 | `VariableID:10:41` | `2e38fc65ef2e112d6db4cc8796b3d752bf9ddb9e` |

All 14 variables have `scopes = ["ALL_SCOPES"]` (no restriction by property type).

## Text styles

The file has four local text styles. All use font family `Inter`, line height `AUTO`, letter spacing `0%`, text case `ORIGINAL`, no decoration.

| Style name | Font style | Size (px) | Style id | Style key |
|---|---|---|---|---|
| `Body/M` | Regular | 16 | `S:dbdb262c011c3fcb69499e331c5c005a58607b99,` | `dbdb262c011c3fcb69499e331c5c005a58607b99` |
| `Body/M` (second style with the same name) | Bold | 32 | `S:9746be61b436546ae921fc1a7a12cd07161e6d4e,` | `9746be61b436546ae921fc1a7a12cd07161e6d4e` |
| `Label/M` | Bold | 14 | `S:ed9cf13259b935301c68de5083f8ea6a5aa24c27,` | `ed9cf13259b935301c68de5083f8ea6a5aa24c27` |
| `Caption` | Regular | 12 | `S:f30a71c535a2bd9ef358d5967725ba287fc0945f,` | `f30a71c535a2bd9ef358d5967725ba287fc0945f` |

## Problems found in the file

1. **`Heading/H1` does not exist.** There is no text style with this name. Instead, two styles are both named `Body/M`: Regular 16 and Bold 32. The Bold 32 one has the size and weight expected of a heading, so it is most likely `Heading/H1` with the wrong name, but the file does not say so. Rename it in Figma (Text styles → right-click → Rename) to `Heading/H1` and publish again; its key stays the same.
2. **Duplicate style name.** Two styles named `Body/M` make references ambiguous. Use the style key, not the name, to tell them apart until the rename is done.
3. **Variable scopes are not set.** Every variable shows in every property picker. Restrict them if wanted: colors to fills/strokes, spacing to gap/padding, `radius/md` to corner radius.
4. **Publish status is not verified.** The API returns keys but does not report publication. Check Assets → Libraries in Figma.
