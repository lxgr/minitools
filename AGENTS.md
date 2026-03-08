# AGENTS – mt.lxgr.net

## Mission
- Keep this repo ready for lightweight single-page apps that are mounted under `mt.lxgr.net/<tool>`.
- Prefer portable, dependency-free HTML/CSS/JS so updates from Codex Cloud (phone) stay manageable.

## Repository conventions
- Each tool lives in its own top-level folder (e.g., `hello/`) with an `index.html`.
- Keep shared assets minimal; if needed, place them inside the tool folder to avoid cross-tool coupling.
- Document any non-obvious behavior or helper scripts inside the relevant folder README.

## Deployment notes
- Pushing to `main` triggers GitHub Pages to deploy directly to mt.lxgr.net—no manual steps.
- Assume contributors might only have the Codex Cloud environment, so avoid workflows that require local binaries.
- If a build process ever becomes necessary, capture the exact commands here and ensure they can run in the hosted environment.

## Skills & automation
- When adding Codex skills, place them under `skills/<name>/SKILL.md` and describe their scope plus any required assets.
- Reference available skills inside `README.md` so mobile contributors know they exist.
- For new automations, log intent and schedule details here so agents know how deployments are orchestrated.

## Current demo
- `hello/` is the live smoke-test page (available at `mt.lxgr.net/hello`). Update or expand it only when adding a better functional check.
