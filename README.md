# OpenBMS Designer

OpenBMS Designer is an early-stage, vendor-neutral web application for sizing
Building Management System (BMS) architectures from a point list.

The project aims to replace repetitive spreadsheet calculations with a simple,
auditable workflow:

**Point list → sizing engine → bill of materials → architecture overview**

> [!IMPORTANT]
> This repository is an early prototype. Results must be reviewed by a qualified
> building-automation professional before they are used on a real project.

## Current MVP

- Manual entry of DI, DO, AI and AO points
- CSV point-list import
- Configurable spare-capacity percentage
- Generic controller and I/O module sizing
- Modbus and BACnet device-capacity checks
- Bill of materials with installed and spare capacity
- Simple architecture overview
- Browser-only operation with no data sent to a server
- Automated tests for the sizing engine

## Demo

No build step is required.

```bash
git clone https://github.com/t4p8cvydv5-ops/openbms-designer.git
cd openbms-designer
npm test
npm start
```

Then open <http://localhost:8080>.

## CSV format

Use the following headers:

```csv
name,type,quantity
Supply fan run status,DI,2
Supply fan command,DO,2
Supply air temperature,AI,1
Heating valve command,AO,1
Energy meters,MODBUS,12
Room controllers,BACNET,20
```

Accepted point types are `DI`, `DO`, `AI`, `AO`, `MODBUS`, and `BACNET`.

## Scope and design principles

OpenBMS Designer is intended for building-automation engineers, system
integrators, technicians and students. The core stays vendor-neutral: equipment
libraries describe public technical capacities, while the sizing engine works
against a common data model.

The project prioritizes:

1. **Traceability** — show how every quantity was calculated.
2. **Reviewability** — never present an automatic result as an approved design.
3. **Portability** — run locally in a browser and export standard formats.
4. **Extensibility** — add equipment libraries without rewriting the engine.

## Project status

The project is in early development. The current release is a functional
proof-of-concept, not a production design tool. See [ROADMAP.md](ROADMAP.md) for
planned work, [CONTRIBUTING.md](CONTRIBUTING.md) to contribute, and
[PUBLISHING.md](PUBLISHING.md) for the first GitHub publication.

## Repository description

Suggested GitHub description:

> Vendor-neutral open-source tool for sizing BMS controllers, I/O modules and communication networks from a point list.

Suggested topics: `bms`, `building-automation`, `hvac`, `bacnet`, `modbus`,
`energy-management`, `open-source`.

## License

Released under the [MIT License](LICENSE).
