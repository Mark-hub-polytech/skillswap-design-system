# SkillSwap — Component keys

Source file: `SkillSwap (Copy)` — file key `6RJxzF2lBjRd0QTyi7D4Tq`
Read from Figma on 2026-11-20 via the Plugin API (`use_figma`, read-only).

## Pages

| Page | Page node id |
|---|---|
| Foundations | `0:1` |
| Components | `7:50` |
| Screens | `7:51` |

## Components (all on the `Components` page)

| Component | Node id | Component key | Type | Size (w × h) |
|---|---|---|---|---|
| `Button / Primary` | `10:64` | `119a1a2c978aa3c5a8fc6e359e4247407ba3cc47` | COMPONENT | 94 × 41 |
| `SkillTag` | `10:68` | `c809b09418d996ff2ca6da28259248d11b00a5e6` | COMPONENT | 98 × 33 |
| `CourseCard` | `10:71` | `7768bc770cb10a06572e627f1d82c01ca7551cce` | COMPONENT | 151 × 68 |
| `SwapCard` | `10:75` | `29715e6eb53b24965fd039c01e259284315fb9e3` | COMPONENT | 242 × 64 |

## Layout of each component

| Component | Auto layout | Padding (T / R / B / L) | Item spacing | Corner radius |
|---|---|---|---|---|
| `Button / Primary` | HORIZONTAL | 12 / 16 / 12 / 16 | 10 | 12 |
| `SkillTag` | HORIZONTAL | 8 / 12 / 8 / 12 | 10 | 12 |
| `CourseCard` | VERTICAL | 16 / 16 / 16 / 16 | 8 | 12 |
| `SwapCard` | VERTICAL | 16 / 16 / 16 / 16 | 8 | 12 |

## Content (children)

| Component | Child node id | Child type | Sample text in the file |
|---|---|---|---|
| `Button / Primary` | `10:62` | TEXT | `Сатып алу` |
| `SkillTag` | `10:66` | TEXT | `Үйретемін` |
| `CourseCard` | `10:69` | TEXT | `Python негіздері` / `12 000 ₸ · 4.9 ★` (two lines in one text node) |
| `SwapCard` | `10:72` | TEXT | `Гитара сабақтары ↔ Ағылшын тілі` / `Аптасына 2 рет · Онлайн` (two lines in one text node) |

## Variants and properties

None of the four components has variants or component properties.

- All four are standalone `COMPONENT` nodes; their parent is the `Components` page, not a `COMPONENT_SET`.
- `componentPropertyDefinitions` is empty for each of them (no TEXT, BOOLEAN, INSTANCE_SWAP or VARIANT properties).
- `description` is empty for each of them.
- Text content is not exposed as a property. To change it, the text layer inside an instance has to be overridden directly.

## Other nodes on the Components page

| Node id | Name | Type | Note |
|---|---|---|---|
| `10:61` | `Rectangle 1` | rounded rectangle, 407 × 407 | Background panel behind the components; not a component. |

## Publish status

- The plugin API returned a `key` for every component, and `remote` is `false` (the components are local to this file).
- The API does not report whether the library has been published, so publication is **not verified here**. Check in Figma: Assets → Libraries (book icon) → Publish. If the keys above stop resolving in other files, publish the library again.
- Keys of local components stay the same after publishing.
