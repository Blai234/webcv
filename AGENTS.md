# AGENTS.md

## Repo Overview
Static HTML/CSS CV site, no build toolchain, no package dependencies.

## Deployment
GitHub Pages is enabled on the `master` branch (root path). Pushing to master automatically deploys to https://blai234.github.io/webcv/.

## Environment Notes
- SSH is unavailable: Use HTTPS Git remotes. Run `gh auth setup-git` to configure the Git credential helper for push access.
- No test, lint, or build commands exist: This is a static site with no compilation or validation steps.

## Git Practices
- Never force push to `master`: GitHub Pages auto-deploys on push, so force pushes will break live site history.
- Keep commits focused: Each commit should represent one logical change (e.g., "Update CV experience section" not "Updates").
- Verify changes locally: Open `index.html` in a browser before pushing to avoid deploying broken layouts.

## Key Files
- `index.html`: Main site content
- `styles.css`: Externalized site styles
- `opencode.json`: OpenCode workspace configuration (see file for OpenCode-specific instructions)
