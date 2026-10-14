# Event Radar

A weekly email of concert announcements, presales, and Louisville arts, events and food — built and run by Claude.

- **Playbook:** [`SKILL.md`](SKILL.md) — what every run does, step by step.
- **Your settings:** [`config/`](config/) — artists and tiers, cities and venues, sources, preferences.
- **Memory:** [`state/`](state/) — every event already sent, your feedback, and a log of each run.
- **Look:** [`templates/email.html`](templates/email.html) — the fixed email layout.

## How to tune it
Reply to any Event Radar email with `+ Artist`, `- Artist`, `T1 Artist`, `more like Artist`,
`no <venue or category>`, or plain notes. The next run reads your reply, updates `config/`,
and records it in `state/feedback.md`. You can also edit files here directly.

## Roadmap
1. Claude-run weekly task (now).
2. Move concert collection (Ticketmaster API, venue calendars, dedupe) into code here,
   with Claude doing Louisville curation and the write-up.
