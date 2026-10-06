# Steal a Thing

A chaotic little collector game inspired by the original Claude Chat build. Grab oddball characters from a moving conveyor, bring them back to your base, earn coins, and sneak loot from wandering NPCs. Random events keep each run lively.

## Play

Open [`index.html`](index.html) in a modern browser, or play the hosted GitHub Pages site after deployment. This is a static HTML app; it needs no build step or server.

## Controls

- **Move:** WASD, arrow keys, or drag on desktop; use the on-screen joystick on touchscreens.
- **Interact:** E on desktop or tap nearby characters/items on touchscreens.
- **Lock your base:** use the lock button near the bottom left.
- **Sell an item:** R near one of your occupied slots, or tap it.
- **Fullscreen / collection index:** F / I on desktop; use the corner buttons on touchscreens.

Progress and discovered characters are saved in your browser on that device. This GitHub Pages edition is single-player with NPCs; the original friend-code rooms used Claude's room service and are not part of this static build.

## GitHub Pages

The workflow in [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) publishes the repository root when a commit reaches `main`. Once Pages is available for the repository, select **GitHub Actions** under **Settings → Pages → Build and deployment → Source** if GitHub has not enabled that source automatically.
