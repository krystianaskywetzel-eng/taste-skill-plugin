# taste-skill — Cowork plugin

A repackaging of **[Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)** in the canonical Claude plugin layout, so it installs cleanly in **Cowork** (and Claude Code) by URL. The upstream repo ships a `source: "./"` marketplace without a `plugin.json`, which Cowork's sync rejects; this repo puts the plugin under `plugins/taste-skill/` with its own `plugin.json`.

The skill itself (`design-taste-frontend`) is leonxlnx's original work, licensed MIT (see [LICENSE](./LICENSE)) — unmodified. This repo only adds plugin manifests.

## Install in Cowork

1. In Cowork: **Customize → Plugins → Add**, point it at `https://github.com/krystianaskywetzel-eng/taste-skill-plugin`
2. **Sync**, then **Install** the `taste-skill` plugin.

## Install in Claude Code

```bash
/plugin marketplace add krystianaskywetzel-eng/taste-skill-plugin
/plugin install taste-skill@taste-skill
```

## Updating

To pull upstream changes later, re-copy the skill into `plugins/taste-skill/skills/taste-skill/` from [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) and commit.

## Credit

Skill by **[leonxlnx](https://github.com/Leonxlnx)** — [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill). Unofficial repackaging for plugin-based installation.
