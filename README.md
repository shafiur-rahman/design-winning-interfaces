# Design Winning Interfaces

**Make your AI a research-first design director.**

Design Winning Interfaces is a portable Agent Skill for creating distinctive, production-ready websites and product interfaces. It makes the agent research the category before choosing a visual direction, design the complete experience rather than only the surface, implement within the existing stack, and validate the result through accessibility, responsiveness, performance, and screenshot-based QA.

## Why this exists

AI-generated interfaces often converge on the same visual defaults: gradient blobs, interchangeable card grids, oversized centered headlines, excessive pills, glass effects, and decoration without product meaning.

This skill replaces those defaults with a repeatable design process grounded in audience needs, category evidence, brand strategy, interaction design, and production constraints.

## What it does

- Researches direct competitors, adjacent products, conventions, and visual saturation
- Defines a product-specific visual thesis and reusable signature device
- Plans content hierarchy, task journeys, responsive behavior, and trust mechanics
- Covers loading, empty, partial, success, validation, error, offline, permission, and destructive states
- Implements with reusable tokens, semantic structure, accessibility, and performance awareness
- Audits the finished interface with a weighted 100-point quality rubric
- Rejects generic AI-design patterns unless the product genuinely calls for them

## Quality bar

The skill treats “award-winning” as a quality standard, not a guaranteed award. A result should score at least 85/100, have no blocker or critical functional issue, and pass its relevant accessibility and responsive checks before being considered complete.

## Structure

    design-winning-interfaces/
    ├── SKILL.md
    └── references/
        ├── category-research.md
        ├── creative-direction.md
        ├── evaluation-and-qa.md
        ├── experience-architecture.md
        ├── implementation-craft.md
        └── interaction-and-errors.md

## Installation

### Claude Code

Clone the repository into your personal skills directory:

    git clone https://github.com/shafiur-rahman/design-winning-interfaces.git ~/.claude/skills/design-winning-interfaces

For a project-only installation, clone or copy it into:

    .claude/skills/design-winning-interfaces

### Claude.ai

1. Select **Code → Download ZIP** on this repository.
2. In Claude, open **Settings → Features → Skills**.
3. Upload the downloaded ZIP.

Custom Skills require a Claude plan and environment that supports Skills and code execution.

### Codex

Clone the repository into your Codex skills directory:

    git clone https://github.com/shafiur-rahman/design-winning-interfaces.git ~/.codex/skills/design-winning-interfaces

## Usage

Ask the agent naturally, or explicitly name the skill:

> Use design-winning-interfaces to research this category and redesign my landing page into a distinctive, production-ready experience.

> Audit this dashboard with design-winning-interfaces, rank the problems by severity, and fix the critical issues.

> Turn this screenshot into an original responsive interface without copying the source design.

## Workflow

1. Frame the business goal, audience, task, emotional target, and constraints.
2. Inspect the current product, brand, design system, and codebase.
3. Build a concise category evidence board.
4. Commit to one defensible creative direction.
5. Map content, journeys, responsive behavior, and interaction states.
6. Implement with production-quality craft.
7. Render, score, test, and iterate.

## Compatibility

The package follows the portable Agent Skills format: a SKILL.md file with YAML metadata and progressively loaded references. It contains no executable scripts or runtime dependencies.

The quality of category research, visual rendering, and implementation depends on the tools available to the agent using the skill.

## Standards referenced

- [Awwwards evaluation system](https://www.awwwards.com/about-evaluation/)
- [Nielsen Norman Group usability heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/)
- [WCAG 2.2](https://www.w3.org/TR/WCAG22/)
- [web.dev Core Web Vitals guidance](https://web.dev/articles/top-cwv)

## Author

Created by [Shafiur Rahman](https://github.com/shafiur-rahman).
