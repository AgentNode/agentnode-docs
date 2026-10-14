# Documentation project instructions

The AgentNode docs at docs.goagentnode.com, built on [Mintlify](https://mintlify.com).
Pages are MDX files with YAML frontmatter; navigation and site settings live in
`docs.json`. Pushing to `main` deploys.

## Who reads this

Real estate agents who are not technical. Assume no knowledge of software terms.
Every page should make sense to someone who has never heard of a CSV, an API
key or a webhook.

## Keep it true to the product

The app lives in the `AgentNode/app` repo. Before naming a button, a screen or
a setting, check the label there (`apps/web/src`) and quote it exactly. Do not
document what is planned; document what ships. Nothing about staging or
internal tooling belongs here.

## Terminology

- **Assistant** (never "agent", which readers take to mean themselves) for
  Lead Nurture, Client Relations and Appointment Recovery. **Job** for what
  each does.
- **Lead** for a prospect, **contact** for anyone in Contacts. **Managed** for
  whether the assistants work on someone.
- **Carrier registration** and **carrier approval**, not "10DLC", "brand" or
  "campaign". Say "AgentNode's own approval" for the loaner while theirs is
  reviewed.
- **CSV file**, glossed as a plain spreadsheet file the first time on a page.
  **CRM**, glossed with an example (Follow Up Boss) the first time.
- **EIN**, glossed as the business's tax ID from the IRS the first time.
- **The menu on the left**, not "the left nav" or "the sidebar". **The AgentNode
  button at the bottom right** for the launcher.
- Paths as **Settings › Messaging**, with `›`.

## Style

- Second person, active voice, US spelling.
- One idea per sentence. Short sentences beat long ones joined with commas.
- Bold anything the reader presses or reads on screen, exactly as the screen
  says it: press **Create account**.
- Lead with what to do, then why. Explain a technical step once, briefly, and
  say who to ask if it is too much (support@goagentnode.com, or **Book
  onboarding call** in the app).
- Sentence case for headings. Numbers and durations in figures: 1 to 3 business
  days, about 15 minutes.
- Before pushing: `mint validate` and `mint broken-links` from this directory
  (`npm i -g mint`).
