# AGENTS.md

Based on guidelines from *Understanding the AGENTS.md File in OpenAI Codex (Vibe Coding Workflow)* citeturn0file0

## Project Overview

* Repository: `chronicles-of-communication`
* Purpose: Digital archive & VR modules for communication history.
* Structure:

  * `/timeline`: JSON data for timeline entries.
  * `/vr-modules`: VR experiences grouped by era.
  * `/assets`: Audio and 3D models.
  * `/docs`: Design specifications and conventions.

## Code Style

* Use Prettier for JavaScript/TypeScript formatting.
* Use ESLint with Airbnb rules; fix all lint errors before commit.
* File names: kebab-case (e.g., `ancient-messenger.js`).
* Variable names: `camelCase` for JS, `PascalCase` for React components.

## Build & Test Instructions

* Install dependencies: `npm install`.
* Run unit tests: `npm test`.
* Build VR modules: `npm run build`.
* Verify build: `npm run lint` and `npm run test` must pass before finalizing.

## File & Module Guidelines

* New timeline entries: add JSON in `/timeline/data.json` and corresponding VR folder under `/vr-modules`.
* VR module entry point: `index.js` in each era subfolder.
* Assets: place new audio in `/assets/audio`, 3D models in `/assets/models`.

## Testing & Verification

* After code changes, run `npm run build` and `npm test`.
* ESLint: `npm run lint`; failures must be fixed.
* For VR modules, perform smoke test in local headset.

## Commit & PR Guidelines

* Commit message prefix: `[Feat]`, `[Fix]`, `[Refactor]`, `[Docs]`.
* Commit title: `<prefix> Short description`.
* PR description template:

  1. **Overview**: Summary of changes.
  2. **Testing Done**: List of tests executed.
  3. **Notes**: Any relevant context or TODOs.

## Additional Context

* Skip VR smoke tests for pure documentation updates.
* For assets larger than 5MB, use Git LFS.
* Use `docs/design-specs.md` for UI/UX guidelines.
