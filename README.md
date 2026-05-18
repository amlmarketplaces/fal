# amlmarketplaces/fal

Claude Code marketplace federating all `@amlplugins/fal-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-fal": {
      "source": { "source": "github", "repo": "amlmarketplaces/fal" }
    }
  },
  "enabledPlugins": {
      "fal-client@aml-fal": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/fal`, cached under `~/.claude/plugins/cache/aml-fal/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (1 total)

- `fal-client` — [@amlplugins/fal-client](https://github.com/amlplugins/fal-client)

## Related

- npm packages: `@amlplugins/fal-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
