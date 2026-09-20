# Roadmap

OpenBMS Designer is developed incrementally. Dates are intentionally omitted
until there is enough contributor capacity to make reliable commitments.

## 0.1 — Foundation

- [x] Manual point-count entry
- [x] CSV import
- [x] Generic equipment library
- [x] Controller and expansion-module sizing
- [x] Communication capacity checks
- [x] Bill of materials and architecture overview
- [x] Unit tests and continuous integration

## 0.2 — Project workflow

- [ ] Save and reopen projects locally
- [ ] Edit imported point lists in a table
- [ ] Export the BOM and calculation report to CSV
- [ ] Add validation errors with row-level CSV feedback
- [ ] Add French and English interfaces

## 0.3 — Equipment libraries

- [ ] Define a documented JSON schema for equipment libraries
- [ ] Import and export custom libraries
- [ ] Add versioning and source links for public technical data
- [ ] Compare valid equipment combinations
- [ ] Add configurable engineering constraints

## 0.4 — Architecture generation

- [ ] Create editable controllers, panels and communication buses
- [ ] Allocate points by equipment or plant zone
- [ ] Validate BACnet/IP and Modbus RTU segments
- [ ] Export architecture diagrams to SVG and PDF

## Longer term

- Collaborative project review
- Rules for redundancy and resilience
- Cable and panel capacity estimates
- Open project format and public API

## Non-goals for the early releases

- Replacing detailed engineering review
- Producing manufacturer-approved selections
- Claiming compliance without project-specific verification
