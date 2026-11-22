<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
CIRCUIT-WORKBENCH — repository foundation
-->

# Architecture

## Current executable surface

The checkout contains:
- repository validation tooling;
- dedicated tests;
- workflow definitions;
- native documentation.

No domain component of Circuit Workbench is implemented yet. The metadata keeps domain capabilities, claims and qualified record formats empty.

## Intended data flow

1. **Review request** submits headless operation or inspection requests exclusively through Circuit Flow and Circuit Core admission.
2. **Verbatim review rendering** loads pinned design views, run observations, acceptance verdicts, clamp envelopes and custodied evidence summaries without re-computing or truncating caveats.
3. **Digest-verified approval handoff** presents the exact summary digest and rate/batch context for enrolled person-in-role signing, feeding admitted model-slot or gate decisions back to Circuit Core.

## Ownership

**This project owns** the planned Circuit Workbench records and boundary rules.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| admission, compartments and approval verification | Circuit Core |
| workflow dispatch | Circuit Flow |
| sign-off verdicts and statistical caveats | Circuit Acceptance |
| safety clamps and lockout recovery | Circuit Automation |
| neuromorphic visualisations | SC-NC Studio |

## Interpretation

- **Presentation.** Displaying an artefact verifies its digest and provenance headers, not its physical correctness.

Read [the documentation architecture](docs/ARCHITECTURE.md) for the planned records, domain rules and schema identifiers.
