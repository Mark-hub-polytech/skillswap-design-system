---
name: skillswap-design-system
description: Design system tokens, typography hierarchy, core UI components (Button/Primary, SkillTag, CourseCard, SwapCard), and layout rules for SkillSwap web/mobile UI generation. Use whenever creating or updating UI components, cards, buttons, tags, or screens in this project.
---

# SkillSwap Design System Rules

Always follow these tokens, typography styles, and component rules when generating or modifying UI code. Never invent off-system hex colors or arbitrary spacing values unless explicitly requested.

## 1. Design Tokens

### Colors (`Colors` collection)
- **Backgrounds (`bg`)**:
  - `bg/page`: `#F8FAFC` — main screen/page background
  - `bg/card`: `#FFFFFF` — card surface background
- **Text (`text`)**:
  - `text/primary`: `#111827` — primary headings and body text
  - `text/secondary`: `#6B7280` — secondary labels and supporting info
- **Brand (`brand`)**:
  - `brand/primary`: `#2563EB` — primary actions and main CTA buttons[cite: 3]
  - `brand/swap`: `#0D9488` — skill-swap tags and exchange highlights[cite: 3]
- **Border (`border`)**:[cite: 3]
  - `border/default`: `#E5E7EB` — card borders and dividers[cite: 3]

### Spacing, Radius & Height (`Spacing` collection)
- **Spacing (`space`)**: `4`, `8`, `12`, `16`, `24` (in `px`)
- **Border Radius (`radius`)**:
  - `radius/md`: `12px` — default corner radius for buttons, tags, and cards
- **Height (`height`)**:
  - `height/m`: `40px` — standard medium control height[cite: 12]

## 2. Typography Styles

Use these four text styles consistently:
- **`Heading/H1`**: Page or section main title (e.g., `32px`, Bold/SemiBold, `text/primary`)[cite: 3, 5, 6]
- **`Body/M`**: Standard readable text (`16px`, Regular, `text/primary` or `text/secondary`)[cite: 3]
- **`Label/M`**: Buttons, tags, and interactive labels (`14px`, SemiBold/Medium)
- **`Caption`**: Metadata, pricing, ratings, schedule details (`12px`, Regular)

## 3. Core Components

### `Button / Primary`
- **Role**: Main primary action button (e.g., purchase/enroll/primary CTA).
- **Layout**: Horizontal auto-layout, centered alignment.
- **Spacing**: Horizontal padding `16px` (`space/16`), vertical padding `12px` (`space/12`).[cite: 12]
- **Shape & Color**: Corner radius `12px` (`radius/md`), background `#2563EB` (`brand/primary`), text color `#FFFFFF`.[cite: 3, 12]

### `SkillTag`
- **Role**: Skill-swap badge/tag (e.g., offering or requesting a skill exchange).
- **Layout**: Horizontal auto-layout, hug content (`width: hug, height: hug`), centered alignment.[cite: 11]
- **Spacing**: Horizontal padding `12px` (`space/12`), vertical padding `8px` (`space/8`).[cite: 11, 12]
- **Shape & Color**: Corner radius `12px` (`radius/md`), background `#0D9488` (`brand/swap`), text color `#FFFFFF`.[cite: 3, 11, 12]

### `CourseCard`
- **Role**: Displays a course item (title + price/rating/metadata).
- **Layout**: Vertical auto-layout (`gap: 8px` / `space/8`, `padding: 16px` / `space/16`).[cite: 12]
- **Shape & Color**: Background `#FFFFFF` (`bg/card`), border `1px solid #E5E7EB` (`border/default`), corner radius `12px` (`radius/md`).[cite: 3, 12, 13]

### `SwapCard`
- **Role**: Displays a skill-swap offer (skill exchange pair + schedule/format metadata).
-[cite: 13]
- **Layout**: Vertical auto-layout (`gap: 8px` / `space/8`, `padding: 16px` / `space/16`).[cite: 12, 13]
- **Shape & Color**: Background `#FFFFFF` (`bg/card`), border `1px solid #E5E7EB` (`border/default`), corner radius `12px` (`radius/md`).[cite: 3, 12, 13]

## 4. Screen & Layout Conventions

- Page background uses `bg/page` (`#F8FAFC`).[cite: 3]
- Vertical sections/items use auto-layout spacing from the `space` scale (`8`, `12`, `16`, `24`) rather than hard-coded magic numbers.[cite: 12]
- Keep component responsibilities clear: `CourseCard` for paid/structured courses, `SwapCard` for skill exchanges, `SkillTag` for swap status/role tags, and `Button / Primary` for primary actions.
