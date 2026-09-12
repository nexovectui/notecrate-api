# notecrate-api

Tiny REST API for saving and tagging bookmarks

Small but I use it weekly.

## Install

```bash
npm install
npm run dev
```

## What it does

- Morgan logging and centralized error handler
- In-memory store with optional JSON persistence
- Request validation helpers, no framework magic
- REST endpoints: list / create / delete / search
- env-driven port, runs anywhere Node does

## How to use

```bash
curl -X POST localhost:3000/api/bookmarks \
  -H 'content-type: application/json' \
  -d '{"url": "https://example.com", "tags": ["reading"]}'
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   └── faq.md
├── examples/
│   └── quickstart.md
├── src/
│   ├── config.js
│   ├── index.js
│   └── store.js
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
└── package.json
```

## Development

```bash
npm install
```

## License

MIT licensed, see LICENSE.
