# shopify-skills

A collection of Claude Code skills for building and maintaining Shopify themes.

Each skill is a focused rule set for a specific area of a Shopify theme — sections, snippets, blocks, Liquid, CSS, JavaScript, performance, accessibility, and more. When you drop this repo into your project's `.claude/skills/` directory, Claude Code auto-discovers and activates the skills, using them as context whenever a matching task comes up.

## Skills included

| Skill | Covers |
|---|---|
| `shopify-sections` | `sections/*.liquid` — schema, structure, presets |
| `shopify-snippets` | `snippets/*.liquid` — LiquidDoc, params, render |
| `shopify-blocks` | `blocks/*.liquid` — theme blocks, static vs dynamic |
| `shopify-templates` | `templates/*.json` + `gift_card.liquid` |
| `shopify-layout` | `layout/theme.liquid` + `password.liquid` |
| `shopify-assets` | `assets/` — asset_url, image_tag, SVG a11y |
| `shopify-config` | `config/settings_schema.json` + `settings_data.json` |
| `shopify-locales` | `locales/` — translation keys, fallback chain |
| `shopify-liquid` | Liquid syntax, tags, filters |
| `shopify-css` | CSS standards, `{% stylesheet %}` scope pitfall |
| `shopify-javascript` | JS, Custom Elements, `{% javascript %}` bundle |
| `shopify-theme-store` | Theme Store submission requirements |
| `shopify-accessibility` | WCAG 2.1 AA patterns |
| `shopify-performance` | Lighthouse / Core Web Vitals |
| `shopify-cli-tools` | Shopify CLI, theme-check, Prettier, Inspector |

## Installation

Clone or copy this repo into your project's `.claude/skills/` directory:

```bash
git clone https://github.com/mattiadragone/shopify-skills .claude/skills/shopify
```

Or add it as a git submodule:

```bash
git submodule add https://github.com/mattiadragone/shopify-skills .claude/skills/shopify
```

Claude Code will discover the skills automatically on the next session start.

## Sources

- [Skeleton theme](https://github.com/Shopify/skeleton-theme)
- [Horizon rules reference](https://github.com/Shopify/horizon/tree/main/.cursor)
- [Shopify themes docs](https://shopify.dev/docs/storefronts/themes)
- [Theme Store requirements](https://shopify.dev/docs/storefronts/themes/store/requirements)
