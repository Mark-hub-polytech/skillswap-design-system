# SkillSwap Components Reference

This reference describes how to structure and use the four core components from Figma (`Components` page) in UI code.

## 1. `Button / Primary`
- **Purpose**: Main call-to-action (CTA) button for primary actions such as buying/enrolling in a course or confirming an action.
- **Structure**:
  - Container: Horizontal auto-layout, centered alignment.
  - Padding: Horizontal `16px` (`space/16`), vertical `12px` (`space/12`).
  - Corner radius: `12px` (`radius/md`).
  - Background: `#2563EB` (`brand/primary`).
  - Label: Uses `Label/M` text style (`14px`, SemiBold/Medium), color `#FFFFFF`.
- **Usage rule**: Use for the primary action in a section or card; avoid placing multiple competing primary buttons side by side.

## 2. `SkillTag`
- **Purpose**: Compact badge/tag used in skill-swap flows (e.g., offering a skill like "Үйретемін" or requesting a skill).
- **Structure**:
  - Container: Horizontal auto-layout, hug content (`width: hug, height: hug`), centered alignment.
  - Padding: Horizontal `12px` (`space/12`), vertical `8px` (`space/8`).
  - Corner radius: `12px` (`radius/md`).
  - Background: `#0D9488` (`brand/swap`).
  - Label: Uses `Label/M` text style (`14px`, SemiBold/Medium), color `#FFFFFF`.
- **Usage rule**: Use specifically for skill-exchange role/status tags rather than standard primary form submission.

## 3. `CourseCard`
- **Purpose**: Card displaying a course item with its title and supporting metadata (such as price and rating).
- **Structure**:
  - Container: Vertical auto-layout (`gap: 8px` / `space/8`, `padding: 16px` / `space/16`).
  - Surface: Background `#FFFFFF` (`bg/card`), border `1px solid #E5E7EB` (`border/default`), corner radius `12px` (`radius/md`).
  - Content: Course title on top, metadata line (e.g., price, rating, format) below using `Caption` (`12px`).
- **Usage rule**: Use for structured courses/listings; keep vertical spacing and card surface tokens consistent.

## 4. `SwapCard`
- **Purpose**: Card displaying a skill-swap offer (for example, exchanging two skills along with schedule and format details).
- **Structure**:
  - Container: Vertical auto-layout (`gap: 8px` / `space/8`, `padding: 16px` / `space/16`).
  - Surface: Background `#FFFFFF` (`bg/card`), border `1px solid #E5E7EB` (`border/default`), corner radius `12px` (`radius/md`).
  - Content: Skill exchange pair/title on top, schedule/format metadata below using `Caption` (`12px`).
- **Usage rule**: Use for peer-to-peer skill exchange items (`SwapCard`) alongside `SkillTag` when indicating skill-swap roles.
