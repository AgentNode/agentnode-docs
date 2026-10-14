# AgentNode docs

The user docs at [docs.goagentnode.com](https://docs.goagentnode.com), built on
[Mintlify](https://mintlify.com). Pages are MDX files in this directory;
`docs.json` holds the navigation and site settings. See [AGENTS.md](AGENTS.md)
for who the docs are for and how they are written.

## Preview locally

```bash
npm i -g mint
mint dev
```

Open `http://localhost:3000`. `mint validate` checks the build and
`mint broken-links` checks every internal link; run both before you push.

## Publishing

Pushing to `main` deploys to production through Mintlify's GitHub app. Open a
pull request for every change.
