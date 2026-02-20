> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

## How to use this guide

- Treat this file as the single source for agent instructions that should be updated whenever the documentation workflow or tooling changes.
- Replace placeholder sections (terminology, style, content boundaries) with real examples that describe the product and the team’s naming conventions.
- Link back to Mintlify references via the installed skill when you need UI or configuration context.

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Terminology

<!-- Add product-specific terms and preferred usage -->
<!-- Example: Use "workspace" not "project", "member" not "user" -->

- Use `MineClawd` when talking about the product itself; never shorten it to "Mine" or "Clawd."
- Capitalize `Session` when referring to a customer-facing session (for example, "a Session is active"); use lowercase `session` for other contexts.
- Refer to saved configurations as a `persona` (lowercase) to match the CLI commands; do not call it a "profile."
- Call the assistive feature **Assistive Touch** so the UI label matches the command link in navigation and docs.
- Treat `Souls` as the configuration section under `docs.json`; mention `souls` only when describing that exact block.
- Use `assets` to describe textures, models, or recordings that users upload; include context so it is clear which type of asset you mean.

## Style preferences

<!-- Add any project-specific style rules below -->

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Limit paragraphs to three sentences and open each one with the main action so users instantly see what to do.
- When explaining a command, name the command in code, then describe the expected outcome in plain sentences; avoid repeating the command text.
- Use Mintlify callouts (`> Warning`, `> Tip`) for advice that could mislead if overlooked and for optional steps.
- Use inline links sparingly and only when they point to another page in this repo or an official MineClawd resource.

## Content boundaries

<!-- Define what should and shouldn't be documented -->
<!-- Example: Don't document internal admin features -->

- Cover only sections that directly impact minecrawd.com users: installation, commands, configuration, tutorials, and troubleshooting.
- Do not document back-end services, unreleased features, or internal team process.
- Avoid in-depth technical explanations of Minecraft mod internals unless the documentation page already targets mod authors.
- Keep statements grounded in the current release; do not speculate about future behavior or plans.
