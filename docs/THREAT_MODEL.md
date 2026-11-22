<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
CIRCUIT-WORKBENCH — repository foundation
-->

# Data and authority boundaries

## Present tooling

**Execution inputs.** The maintained checkout and the selected development environment are what the repository controls inspect.

**Received inputs.** Descriptors, dependency receipts and generated inventories cannot nominate an acceptance policy or an executable.

**Bounded checks.** Controls inspect bounded local paths and emit fixed diagnostics.

Foundation qualification is in progress.

## Future domain inputs

**Supplied data, with no authority.** The following inputs are treated strictly as supplied data:
- design views, run observations and acceptance reports;
- custodied evidence summaries and approval digests;
- operator workspace preferences.

They grant no authority to:
- bypass Circuit Core admission, person approvals or Circuit Automation clamps;
- execute UI-only transformations absent from headless CLI/API flows;
- strip statistical caveats, compartment banners or named-trust disclosures;
- cache confidential enclave summaries outside the enclave.

**Comments and embedded text are data.** Descriptions, netlist comments and datasheets arriving inside supplied inputs are data, never instructions to an operator or an agent.

**Public-repository data boundary.** Hosted CI for this public repository runs on public material only. Confidential foundry-NDA, customer, export-controlled or secret-bearing material never enters this repository, its CI or its issues.

## Threats and the rules that answer them

| Threat | Architectural rule |
| --- | --- |
| UI spoofing of approval digests, hidden autonomy limits or truncated statistical caveats | Review views verify exact digest equality against custodied summary bytes and render compartment tags, clamp limits, tool-estimate labels and named residuals verbatim |
| Hidden UI-only business logic diverging from headless automation and CI | Circuit Workbench registers zero solver manifests and routes every action through headless Circuit Core and Circuit Flow contracts |

## Residuals named, not removed

- **Operator attention.** Verbatim rendering and hub review-time/batch flags mitigate but cannot eliminate human inattention, which is audited post-pilot under Circuit Core's two-stratum approval audit.

**Not claimed:** no isolation, physical, statistical, safety or durability guarantee is claimed by this foundation.
