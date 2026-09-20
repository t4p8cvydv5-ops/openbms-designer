# Contributing

Thank you for helping improve OpenBMS Designer. The project is at an early
stage, so small, focused contributions are especially useful.

## Development setup

Requirements: Node.js 20+ and Python 3.

```bash
npm test
npm start
```

Open <http://localhost:8080>. The application uses native browser modules and
has no runtime dependencies.

## Before opening a pull request

1. Open or reference an issue for substantial changes.
2. Keep vendor-specific data separate from the generic sizing engine.
3. Add tests for sizing or validation logic.
4. Do not include confidential point lists or proprietary documentation.
5. Explain the engineering assumption behind every new rule.

## Commit style

Use short conventional commits when practical:

- `feat: add CSV export`
- `fix: avoid double-counting controller I/O`
- `docs: explain Modbus capacity assumptions`
- `test: cover zero-point projects`

## Reporting technical-data issues

Include the equipment reference, the affected field, a public source link and
the document revision. Do not upload copyrighted manuals to the repository.
