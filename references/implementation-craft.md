# Implementation craft

Use this when converting the direction into production code.

## Reconnaissance

Before editing:

- read repository instructions;
- identify routing, rendering model, styling system, tokens, components, icons, fonts, assets, data contracts, and test commands;
- locate existing responsive and accessibility conventions;
- note unrelated worktree changes and avoid touching them.

Prefer the smallest coherent edit surface. Reuse the product’s primitives unless they prevent the requested outcome.

## Systemize decisions

Represent repeated values as tokens:

- color roles;
- type roles and scale;
- spacing steps;
- radii;
- border and elevation;
- container and breakpoint rules;
- motion duration and easing.

Use components for repeated behavior, not merely repeated markup. Keep one-off art direction local when abstraction would hide intent.

## Structure and accessibility

- Use semantic HTML and native controls before ARIA.
- Keep heading order and landmarks meaningful.
- Associate labels, descriptions, errors, and status messages programmatically.
- Ensure visible focus, logical tab order, keyboard completion, and usable target sizes.
- Provide useful alternative text; treat decorative media as decorative.
- Meet WCAG 2.2 AA unless the project has a stricter requirement.

## Responsive implementation

- Design from content priority, not device names.
- Test the narrowest supported width, an intermediate width, and a large width.
- Prevent accidental horizontal scrolling, clipped focus rings, orphaned headings, and unreadable line lengths.
- Adapt dense tables, charts, and multi-column controls intentionally rather than shrinking them.

## Media and motion

- Reserve intrinsic dimensions or aspect ratios to prevent layout shift.
- Serve appropriate formats and sizes; defer noncritical media.
- Keep the main visual discoverable early when it drives the first view.
- Animate transform and opacity when possible; avoid expensive continuous effects.
- Never make content or controls unavailable until an entrance animation completes.

## Product integrity

- Keep existing APIs, auth, analytics, localization, and data behavior intact.
- Do not fabricate backend behavior to make a mockup appear complete.
- Use the project’s established patterns for errors, loading, permissions, and optimistic updates.
- Remove dead code and abandoned visual experiments introduced during iteration.

## Verification

Run the narrowest relevant formatter, type check, test, and build commands. Then run broader checks when cost is reasonable. Inspect browser console and network failures for the changed experience. Report any check that could not run and why.
