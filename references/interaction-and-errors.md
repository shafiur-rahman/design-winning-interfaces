# Interaction and error design

Use this for every flow that loads data, accepts input, changes persistent state, or can fail.

## Create a state inventory

Include only relevant states, but check each:

- idle and first use;
- hover, focus, pressed, selected, and disabled;
- loading and long-running progress;
- empty and zero-result;
- partial or stale data;
- success and confirmation;
- inline validation;
- recoverable and terminal error;
- offline or reconnecting;
- unauthorized, forbidden, and expired session;
- rate-limited or unavailable;
- destructive confirmation, completion, and undo.

## Specify behavior

For each important component or flow, record:

| State or event | Trigger | Visible response | Available choice | Recovery | Accessibility behavior |
| --- | --- | --- | --- | --- | --- |

Make state transitions deterministic. Prevent duplicate submissions and contradictory controls.

## Feedback rules

- Acknowledge an interaction immediately, even when completion takes longer.
- Prefer skeletons only when the final structure is predictable. Use progress or plain status for indeterminate work.
- Preserve layout where possible to avoid disruptive movement.
- Place feedback near its cause while maintaining a page-level summary for form errors when helpful.
- Keep success messages specific about what changed and what happens next.

## Error rules

Write errors in this order:

1. What happened in the user’s language.
2. What remains safe or saved.
3. What the user can do next.
4. A support or retry path when self-recovery is impossible.

Preserve valid input. Focus or link to the first invalid field. Do not expose stack traces, internal codes, or vague “something went wrong” messages as the only explanation.

## Destructive actions

- Distinguish reversible from irreversible actions.
- Prefer undo for low-risk reversible actions.
- Use confirmation when consequences are substantial or hard to recover from.
- Name the affected object and consequence in the confirmation.
- Keep the safe action visually clear without making the destructive choice hard to find.

## Motion and input

- Support keyboard and pointer input for every essential action.
- Provide a non-drag alternative for drag interactions.
- Avoid hover-only disclosure of essential controls.
- Keep focus visible and unobscured when overlays, sticky regions, or drawers appear.
- Cancel or simplify nonessential motion under reduced-motion preferences.
