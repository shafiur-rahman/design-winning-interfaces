---
name: design-winning-interfaces
description: Research-first creative direction, UX architecture, interface design, frontend implementation, critique, and visual QA for distinctive production-ready websites, landing pages, dashboards, web apps, mobile interfaces, and product screens. Use when Codex is asked to design, build, redesign, polish, art-direct, or audit a digital interface; translate a brief or screenshot into UI; improve a generic-looking AI-generated site; establish a visual system; or raise an existing experience to portfolio, launch, or award-submission quality.
---

# Design Winning Interfaces

## Outcome

Create an interface that is specific to the product, legible under real use, technically credible, and memorable for a defensible reason. Treat “award-winning” as a quality bar, never as a guaranteed award.

## Operating contract

- Research the category before choosing a visual language for greenfield work or a substantial redesign.
- Inspect the existing product, code, brand assets, content, and design system before proposing replacements.
- Preserve working architecture and established brand equity unless the user explicitly requests a reset.
- Implement the interface when the user asks to build or change it. Do not stop at mood boards or advice.
- Make the strongest reasonable assumptions and state them briefly. Ask one focused question only when the missing answer would materially change the product architecture, brand, compliance, or audience.
- Derive inspiration from patterns; never clone a reference, copy its assets, or reproduce a recognizable composition.
- Prefer one coherent direction. Offer multiple directions only when exploration or stakeholder choice is part of the request.
- Use real or clearly labeled placeholder content. Never invent customer logos, testimonials, awards, usage metrics, or research findings.

## Route the task

| Mode | Primary action |
| --- | --- |
| Greenfield | Research the category, define the experience and visual thesis, then build |
| Redesign | Diagnose the current experience, preserve useful equity, and make targeted structural changes |
| Audit | Produce evidence-backed findings ordered by impact and severity; do not mutate files unless asked |
| Productionize | Convert an approved direction into complete responsive states and validate it in the existing stack |
| Visual translation | Extract principles from the supplied image or design, adapt them to the product, and avoid literal copying |

## Workflow

### 1. Frame the brief

Extract:

- product, offer, and business goal;
- primary audience and their highest-value job;
- desired action and proof needed before that action;
- required content, routes, states, devices, and constraints;
- existing brand rules, assets, component libraries, and technical stack;
- emotional target in plain language, such as assured, energetic, precise, warm, or editorial.

Write a one-sentence design challenge: “Help [audience] accomplish [job] while feeling [emotion], without [risk].”

### 2. Inspect the foundations

For an existing repository:

- Read the project instructions and identify the application entry points, routing, styling approach, tokens, shared components, assets, and test commands.
- Locate the smallest set of files that controls the target experience.
- Reuse compatible components and dependencies. Do not replace the framework or design system for stylistic convenience.
- Run the current page before editing when feasible and capture a baseline at representative viewports.

For a supplied screenshot or design, inventory hierarchy, grid, typography, color roles, component grammar, imagery, motion clues, and interaction assumptions.

### 3. Build a category evidence board

Read [category-research.md](references/category-research.md). Research current direct competitors, adjacent exemplars, category conventions, and user expectations when web access is available. Separate durable conventions from short-lived trends. Record sources and observations; do not treat screenshots as permission to copy.

Do not enter visual styling without a concise evidence board unless the user explicitly asks for an offline or rapid concept. In that case, label the research limitation.

### 4. Commit to a creative direction

Read [creative-direction.md](references/creative-direction.md). Define:

- a named visual thesis;
- the strategic tension it resolves;
- one signature device that belongs to this product;
- typography, palette, grid, spacing, shape, icon, imagery, and motion rules;
- explicit anti-goals that prevent drift into generic AI styling.

Every visible choice must support content hierarchy, brand meaning, interaction clarity, or memorability. Remove decoration that does none of these.

### 5. Design the experience, not only the surface

Read [experience-architecture.md](references/experience-architecture.md) and [interaction-and-errors.md](references/interaction-and-errors.md).

- Establish the page narrative or task journey before arranging sections.
- Define the primary action and one secondary action per context.
- Specify loading, empty, partial, success, validation, error, offline, permission, and destructive states as relevant.
- Make responsive layouts reprioritize content instead of merely shrinking it.
- Preserve user input and give a clear recovery path after failures.

### 6. Implement with craft

Read [implementation-craft.md](references/implementation-craft.md).

- Express the system through reusable tokens and components.
- Use semantic structure, keyboard-complete interactions, visible focus, sufficient contrast, and reduced-motion behavior.
- Use a consistent icon family; do not substitute emoji for interface icons.
- Keep media purposeful and optimized. Retrieve or generate imagery only when it materially improves the direction and usage rights are appropriate.
- Complete the full requested experience. Do not leave nonfunctional showcase controls or hidden placeholder states.

### 7. Render, score, and iterate

Read [evaluation-and-qa.md](references/evaluation-and-qa.md).

- Render the actual result at mobile, tablet, and desktop widths relevant to the product.
- Inspect screenshots for hierarchy, clipping, overflow, rhythm, density, focal order, and consistency.
- Exercise keyboard paths and the important interaction and failure states.
- Check console output, tests, build, accessibility, and performance using the project’s available tooling.
- Score the result against the 100-point rubric. Iterate until it scores at least 85, has no blocker, and has no accessibility or functional critical issue.
- If rendering is impossible, say so and perform the strongest available static checks; never imply visual validation occurred.

## Anti-generic guardrails

- Do not default to gradient blobs, aurora backgrounds, glass cards, glowing borders, excessive pills, bento grids, or floating decorative orbs.
- Do not wrap every section in a rounded card. Use grouping only when it communicates structure or interaction.
- Do not default to Inter, a purple-blue palette, or oversized center-aligned hero copy without evidence from the product or brand.
- Do not make every section use the same centered heading-plus-three-cards rhythm.
- Do not use random animation as proof of quality. Motion must explain change, reinforce causality, orient the user, or reward completion.
- Do not sacrifice comprehension, accessibility, speed, or conversion for novelty.
- Do not confuse minimal content with strong hierarchy or visual noise with originality.

## Handoff

Lead with the completed outcome. Briefly provide:

- the direction and why it fits;
- what was implemented or audited;
- the key validation result and any remaining limitation;
- exact files or artifact links when applicable.

Keep the research and design rationale concise unless the user asks for a full case study.
