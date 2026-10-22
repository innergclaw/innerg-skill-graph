# ⚡️ InnerG Skill Graph

**Live:** https://innergclaw.github.io/innerg-skill-graph/

An interactive map of Nasirr "Nas" Mayo's skills, the InnerG ecosystem, clients, SI teammates and stack. Human-led, with SI as partner.

![Skill Graph Preview](preview.png)

## Features
- Dark InnerG theme with a glowing force-directed network
- Legend that doubles as a group filter (tap a group to hide or show it)
- Search (Enter jumps to the first match)
- Click any node for a detail panel: description, live links, connections (tap a connection to jump)
- **Competency view** toggle: hub-and-spoke rings centered on Nas (skills, ecosystem, teammates, clients, stack)
- Freeze physics, reset, export JSON
- Mobile friendly (bottom sheet panel)

## Groups
| Group | Use for |
|---|---|
| `core` | Nas and Home Base |
| `venture` | InnerG Intel, Learn, Agent Academy, Reads, INNERG PULSE, INNERG ID, OwnYourWeb Systems, SHOPNASGFX |
| `client` | Real client sites |
| `agent` | Grok Bot SI teammates (MARROW, InnerG Studio, Market Pulse, Trading Lab, Niche Lab, The Final Frequency Editor, SOC Coach) |
| `skill` | Capabilities |
| `tool` | Stack (GitHub, Pages, Supabase, Stripe, X, Substack, Discord, YouTube, Grok Bot) |
| `legacy` | Retired setups (OpenClaw / Codex / Hermes) |

## Editing
Everything lives in `graphData` inside `index.html`:

```js
{ id:'new-id', label:'Name', group:'venture', size:24, desc:'One line.', links:[['Site','https://...']] }
// edges: [from, to, label]
['nas','new-id','founded']
```

House rules for copy: say SI or superintelligence, use ~ instead of em dashes, ⚡️ is the InnerG emoji, only real and verifiable items.

## Built with
[vis-network](https://visjs.org/) from a CDN, plain HTML/CSS/JS, GitHub Pages. No build step, no secrets.
