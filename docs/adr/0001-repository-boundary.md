<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
CIRCUIT-WORKBENCH — repository foundation
-->

# Decision: restrict Circuit Workbench to a zero-authority, headless-backed review and inspection client

## Context

Interactive EDA GUIs frequently accumulate hidden netlist edits, waiver toggles or instrument commands that cannot be reproduced headlessly in CI or audited against signed approval digests.

## Decision

**What Circuit Workbench owns:**
- workspace session;
- review view;

**What it imports:** only Circuit Core and Circuit Flow.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| admission, compartments and approval verification | Circuit Core |
| workflow dispatch | Circuit Flow |
| sign-off verdicts and statistical caveats | Circuit Acceptance |
| safety clamps and lockout recovery | Circuit Automation |
| neuromorphic visualisations | SC-NC Studio |

## Consequences

**What can be qualified now:** repository governance and validation tooling, before domain code exists.

**What it cannot qualify:** unimplemented schemas, solvers, hardware or sign-off verdicts.

**Architectural consequences:**
- Circuit Workbench imports only Circuit Core and Circuit Flow and holds zero solver or actuation authority;
- every human review displays the exact digest-verified summary and caveats recorded in the approval trail.
