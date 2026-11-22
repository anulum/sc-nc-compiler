<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-COMPILER — repository foundation
-->

# SC-NC Compiler

SC-NC Compiler is being built as the compiler split out of SC-NeuroCore: the intermediate representation of a spiking network, its lowering to register-transfer-level hardware bundles, the photonic hand-off, compression, energy models and export. It imports SC-NC Core, SC-NC Catalogue and SC-NC Engine, and it hands its bundles to the circuit platform. Its current executable surface is repository validation tooling. It has no installed network compiler, RTL lowering runner, photonic hand-off writer or qualified record schema.

SC-NC Compiler is part of the **SC Neuromorphic Computing Systems** group (SC-NEUROMORPHIC-COMPUTING-SYSTEMS). The [group and project map](https://github.com/anulum/sc-neurocore/blob/main/docs/ecosystem.md) shows the whole programme and where this repository sits in it.

Read [Architecture](ARCHITECTURE.md), [validation tooling](validation-tooling.md), [data boundaries](THREAT_MODEL.md) and the [repository boundary decision](adr/0001-repository-boundary.md).
