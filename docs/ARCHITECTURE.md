<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-COMPILER — repository foundation
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
| IR graph | A spiking network as an intermediate-representation graph, with its numeric formats | Graph checks and equivalence with the source network on declared cases |
| RTL lowering bundle | The register-transfer-level design a network lowers to, with its sources and constraints | Lowered design checked against the IR on declared vectors |
| Photonic hand-off | The description of a network's photonic implementation handed to the photonics platform | Hand-off checks against the IR and the target's declared limits |

## Planned record schemas

- `sc_nc_compiler.ir_graph.v1`
- `sc_nc_compiler.rtl_lowering_bundle.v1`
- `sc_nc_compiler.photonic_handoff.v1`

These are planned identifiers. None of them is registered or qualified here.

It also takes over, unchanged, sc-neurocore.scnir (v0.7) and sc-neurocore.mlir_bundle_manifest (v1) from SC-NeuroCore when their code moves here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
