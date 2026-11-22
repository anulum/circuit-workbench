<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
CIRCUIT-WORKBENCH — repository foundation
-->

# Repository architecture

## Current executable tooling

**What it contains:** the repository's metadata, source-provenance, workflow, dependency-alignment, documentation, inventory and preflight controls.

**What each control does:** it inspects its fixed, declared local scope.

**What received metadata cannot do:** select another acceptance policy or grant domain authority.

Foundation qualification is in progress.

## Intended domain boundaries

| Record | Responsibility | Required evidence |
| --- | --- | --- |
| Workspace session | Authenticated operator session state, active compartment ceiling, pinned view selections and headless request correlation | Strict enforcement of the operator's compartment ceiling and zero hidden state mutations |
| Review view | Verbatim presentation of a candidate artefact, its acceptance report, its autonomy/clamp limits, the exact canonical approval digest and the structured evidence summary retrieved by digest from application custody | Byte-exact match between the displayed summary digest and the digest signed in the person-in-role approval record |

## Anti-spoofing and summary-digest integrity

- **What the reviewer sees is what is signed.** A review view resolves the evidence summary by its exact content digest from application custody, displays data compartments, statistical caveats (`inconclusive at this n`, tool-estimate seeds, named trusts) and autonomy ceilings unabridged, and refuses rendering on any digest mismatch.

## Planned record schemas

- `circuit_workbench.workspace_session.v1`
- `circuit_workbench.review_view.v1`

These are planned identifiers. None of them is registered or qualified here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
