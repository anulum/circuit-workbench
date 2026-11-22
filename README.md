<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
CIRCUIT-WORKBENCH — repository foundation
-->

# Circuit Workbench

Circuit Workbench is being built as the thin, headless-backed operator inspection and review client of the circuit platform. It renders design views, run observations, acceptance reports, autonomy ceilings and canonical approval digests with their custodied evidence summaries — containing zero UI-only design, verification, learning or actuation logic. This checkout contains repository validation tooling and documentation only. Full foundation qualification is in progress. There is no installed workbench client, workspace-session service, review renderer or qualified record schema.

Circuit Workbench is part of the **SC Neuromorphic Computing Systems** group (SC-NEUROMORPHIC-COMPUTING-SYSTEMS). The [group and project map](https://github.com/anulum/sc-neurocore/blob/main/docs/ecosystem.md) shows the whole programme and where this repository sits in it.

**What does not exist yet:**
- a workbench client, session server or review-view renderer;
- a registered runtime record schema;
- any hosted web application.

## Boundary

**What this project owns:**

| Record | Scope |
|---|---|
| Workspace session | Authenticated operator session state, active compartment ceiling, pinned view selections and headless request correlation |
| Review view | Verbatim presentation of a candidate artefact, its acceptance report, its autonomy/clamp limits, the exact canonical approval digest and the structured evidence summary retrieved by digest from application custody |

**Static imports:** only Circuit Core and Circuit Flow.

**Records read without importing domain code:**

| Source | Records consumed |
|---|---|
| Circuit Core and Circuit Flow | entity references, operation requests, design views, approval records, autonomy envelopes, run plans and run observations |
| Circuit Acceptance | qualification records, acceptance plans and acceptance reports |
| Circuit Automation | command events, reconciliation records, safety-clamp envelopes and recovery plans |
| Circuit Learning | process model inventories and study templates |
| Circuit Manufacturing and Circuit Prototyping | manufacturing packages, work orders, dispositions, change proposals, supplier handoffs, RMA records and debug captures |
| SC-NC Studio | neuromorphic studio cross-view descriptors |

**Capability registration and handoffs:** Operates purely as a headless-backed client over Circuit Core and Circuit Flow (`0` solver manifests) and exchanges review views with Circuit Core and SC-NC Studio.

**Explicit non-claims and operating boundaries:**
- It registers zero solver manifests and contains zero UI-only schematic, layout, verification, learning or equipment-actuation logic: every operation exists headlessly through Circuit Core and Circuit Flow.
- It never constructs shadow approvals, hides autonomy or clamp limits, or alters an evidence summary's digest.
- Confidential enclave summaries are rendered strictly inside their enclave session and never cached into lower-class storage.

## Current tooling

Repository controls inspect:
- metadata and source attribution;
- workflows and dependency alignment;
- native documentation and repository inventory;
- preflight orchestration.

Metadata declares architecture-only maturity with empty implemented domain capability and claim inventories.

- Use the exact environment in [Contributing](CONTRIBUTING.md).
- Full CI and preflight belong in CI or in an explicitly admitted pre-push environment.
- See [Validation](VALIDATION.md) for the maintained validation scope.

## Intended evidence

Every future domain artefact will carry the platform's common provenance envelope, its source and environment digests, its confidentiality compartment and its explicit verification boundary. None of the planned record schemas is registered or qualified by this foundation.

## Documentation and support

Read [Architecture](ARCHITECTURE.md), [support](SUPPORT.md), [security reporting](SECURITY.md) and [citation metadata](CITATION.cff).

**Not claimed:**
- a hosted service, released package or DOI;
- a public CI status;
- a performed simulation, hardware measurement or sign-off verdict.

## Licence

Source is licensed under [AGPL-3.0-or-later](LICENSE). A commercial licence is available through the contact in [NOTICE](NOTICE.md).

![ANULUM](docs/assets/anulum_logo_company.jpg)

![Fortis Studio](docs/assets/fortis_studio_logo.jpg)

## Text and data mining reservation
The rightsholder, Miroslav Šotek (ANULUM), expressly reserves the use of the
works in this repository for text and data mining, including the collection of
this content for, and its use in, training, fine-tuning or evaluating machine
learning and artificial intelligence models, in accordance with Article 4(3) of
Directive (EU) 2019/790 and the national provisions transposing it.

No permission for such use has been granted beyond what the licence in
`LICENSE` grants. This reservation does not change that licence: uses the
licence permits remain permitted on its terms, including its attribution and
share-alike conditions.

Reservation made on 2026-11-22. Requests for permission: contact the
rightsholder through the contact listed in this repository.
