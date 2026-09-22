# Evaluation and visual QA

Use this after a meaningful implementation or for a design audit.

## Screenshot loop

1. Render the real experience with representative content and data.
2. Capture mobile, intermediate, and desktop widths relevant to the product.
3. Compare the images side by side.
4. Mark issues in focal order, composition, type, spacing, overflow, state clarity, and brand consistency.
5. Fix the highest-impact cause rather than polishing symptoms.
6. Recapture affected widths and repeat.

Inspect long content, short content, empty data, validation errors, loading, and at least one failure state when they exist.

## 100-point scorecard

| Dimension | Weight | Full-credit evidence |
| --- | ---: | --- |
| Strategy and research | 12 | Decisions connect to audience, category evidence, and business goal |
| Content and hierarchy | 12 | The message, task, and next action are immediately legible |
| Originality and brand fit | 12 | A product-specific thesis and repeatable signature device survive the swap-brand test |
| Typography | 10 | Roles, scale, measure, rhythm, and rendering are intentional |
| Color and contrast | 10 | Functional roles are coherent and states remain distinguishable |
| Composition and responsiveness | 10 | Alignment, density, silhouette, and reprioritization work across widths |
| Interaction and states | 10 | Feedback, loading, empty, error, and recovery behavior are complete |
| Accessibility and usability | 12 | Keyboard, focus, semantics, targets, labels, motion, and WCAG 2.2 AA checks pass |
| Performance and technical fit | 6 | The solution respects the stack and avoids avoidable loading or interaction cost |
| Detail and finish | 6 | Icons, edges, copy, media, transitions, and consistency withstand close inspection |

Target at least 85 out of 100. Do not pass a result with a blocker, broken primary task, critical accessibility failure, misleading content, or major responsive defect regardless of score.

## Severity

- Blocker: prevents the primary task, creates material harm, or makes the output unusable.
- Critical: causes severe confusion, exclusion, data loss risk, or failure at a major viewport.
- Major: visibly weakens hierarchy, trust, comprehension, or consistency.
- Minor: localized polish issue with low task impact.

Fix in that order.

## Heuristic review

Check:

1. system status is visible;
2. language and ordering match the user’s mental model;
3. cancel, back, undo, or exit exists where needed;
4. components and terms remain consistent;
5. risky errors are prevented;
6. choices are recognizable without memory burden;
7. frequent tasks are efficient;
8. every visible element earns its place;
9. errors are specific and recoverable;
10. help appears in context when needed.

## Accessibility checks

- Navigate the complete primary task using only the keyboard.
- Verify focus is visible and not hidden by sticky or overlay content.
- Check text, component, and state contrast.
- Check labels, headings, landmarks, names, roles, and status announcements.
- Check zoom and reflow, target sizing, reduced motion, and non-drag alternatives.
- Test error identification and recovery without relying on color alone.

## Performance checks

Measure when tooling is available. Pay particular attention to:

- discovery and priority of the main visual or content;
- unnecessary JavaScript and long interaction tasks;
- layout shifts from media, fonts, or injected content;
- excessive DOM size or expensive visual effects;
- font, image, animation, and third-party payloads.

## Evidence sources

- Awwwards evaluation system: https://www.awwwards.com/about-evaluation/
- Nielsen Norman Group usability heuristics: https://www.nngroup.com/articles/ten-usability-heuristics/
- W3C Web Content Accessibility Guidelines 2.2: https://www.w3.org/TR/WCAG22/
- W3C summary of new WCAG 2.2 criteria: https://www.w3.org/WAI/standards-guidelines/wcag/new-in-22/
- web.dev Core Web Vitals guidance: https://web.dev/articles/top-cwv

Use current official guidance when exact thresholds or conformance claims matter.
