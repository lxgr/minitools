# minitools

Static hosting repo for mt.lxgr.net. Every mini tool lives in its own
subdirectory so it can be served as `mt.lxgr.net/<tool-name>` via GitHub Pages.

## How things are organized
- `/<tool>/index.html` (plus optional assets) represents a self-contained single
  page app. Keep tools additive—never nest unrelated tools together.
- `hello/` contains a simple hello-world page that verifies the routing works at
  `mt.lxgr.net/hello`.
- Optional Codex skills or helper docs can sit next to the apps in their own
  folders when needed.

## Deployment model
1. Push to `main` (from a laptop or Codex Cloud on a phone) and rely on the
   repo's GitHub Pages configuration to auto-build and deploy to mt.lxgr.net.
2. Changes are static, so no build step is required—GH Pages just serves the
   committed files.
3. To add a new app, create a new folder, drop an `index.html` (plus assets),
   and push. Subdirectories map directly to live URLs.

## Working from Codex Cloud / mobile
- Keep edits small and testable since you may not have a local preview.
- Update `README.md` and `AGENTS.md` with any new conventions so future edits
  from mobile stay in sync.
- Skills can automate repetitive tasks (e.g., scaffolding a new SPA); document
  their expectations inside `skills/<name>/SKILL.md`.

## Next steps / ideas
- Add more SPAs (e.g., timers, converters) following the subdirectory pattern.
- Document any skills or deployment tweaks inside `AGENTS.md` so automations
  know how to behave.
