RISC-V Specialized Vetting & Rubric Matrix

This document defines the core competencies, key signal keywords, skepticism triggers, and score penalties for the 6 primary engineering and GTM roles within the RISC-V semiconductor ecosystem.

SEGMENT A: SILICON & SYSTEMS ENGINEERING TRACK

[ROLE 1] RISC-V CPU / SoC Design & Microarchitecture Engineer

Target Focus: Specs, RTL pipelines, out-of-order execution, microarchitecture design, and SoC physical integration.

Primary Keywords: RTL, Microarchitecture, Decode, Pipeline, Hazard, Out-of-Order (OoO), Branch Prediction, Cache Coherence, TileLink, AXI, SystemVerilog, Chisel.

Skepticism Triggers: - Candidates claiming to "design cores" who only instantiate pre-built open-source IP (e.g., Ibex, Rocket, SweRV) without modifying execution datapath RTL.

Vague references to "SoC design" that are actually just basic FPGA pin mappings.

Grading Penalty constraints: - If a candidate claims CPU Design/Architecture expertise but shows zero evidence of custom RTL microarchitecture design and micro-hazard resolution: Cap score to a MAXIMUM of 5.5/10.0.

[ROLE 2] RISC-V Design Verification / Formal Engineer

Target Focus: Validation architectures, functional/performance metrics, functional coverage, and mathematical formal proofs.

Primary Keywords: UVM, Constrained-Random, Assertion-Based Verification (ABV), SVA, Coverage-Driven Verification (CDV), JasperGold, VC Formal, Model Checking, formal proofs.

Skepticism Triggers:

Candidates who write "testbenches" but only run basic directed C-tests rather than structuring modular UVM classes or defining abstract formal properties.

Relying exclusively on pre-packaged VIP (Verification IP) without writing custom transaction sequences.

Grading Penalty constraints:

If a candidate claims Senior/Lead DV status but has no experience writing custom UVM agents or formal properties, relying entirely on basic directed assertions: Cap score to a MAXIMUM of 6.0/10.0.

[ROLE 3] RISC-V Software / Toolchain / Embedded Systems Engineer

Target Focus: Compilers, linkers, OS/RTOS bring-up, bare-metal runtime, low-level firmware, and SDK development.

Primary Keywords: LLVM, GCC, Clang, compiler optimization, OpenSBI, U-Boot, Linux kernel upstreaming, FreeRTOS, bare-metal, Newlib, hal, GDB, JTAG.

Skepticism Triggers:

Standard application software developers who claim "embedded" experience because they ran an app on a Raspberry Pi.

Claims of "compiler optimization" that only amount to changing compiler flags (e.g., -O3) rather than writing compiler backend code or modifying instruction selection DAGs.

Grading Penalty constraints:

If a compiler/toolchain candidate has never modified toolchain internals (GCC/LLVM machine descriptions) or written low-level boot code/linkers: Cap score to a MAXIMUM of 6.2/10.0.

📈 SEGMENT B: GO-TO-MARKET (GTM) & ADOPTION TRACK

[ROLE 4] RISC-V Solutions / Sales Engineer (FAE)

Target Focus: Customer enablement, technical pre-sales, product evaluations, demos, custom core mapping, and training.

Primary Keywords: Pre-sales, FAE, Field Applications, Customer Enablement, Demos, Link-Budget, Proof-of-Concept (PoC), Technical Collateral, Evaluation Boards, Training.

Skepticism Triggers:

Sales reps who simply forward technical questions to back-end engineering without triaging customer issues or running evaluation boards themselves.

Grading Penalty constraints:

If a Solutions Engineer candidate cannot run evaluation board diagnostics, perform preliminary hardware triage, or write basic pre-sales scripts: Cap score to a MAXIMUM of 5.8/10.0.

[ROLE 5] IP / Platform Account Executive (Enterprise & OEM)

Target Focus: High-ticket IP licensing, multi-year foundry/ASIC contracts, OEM design-win procurement, and royalty structures.

Primary Keywords: IP Licensing, Design-Win, TLA, Multi-Use License, Perpetual License, Royalty ASP, OEM Pipeline, NDA, Contract Negotiation, ASIC Sales.

Skepticism Triggers:

SaaS software sales reps who treat semiconductor intellectual property licenses like standard monthly user subscriptions, showing no understanding of manufacturing cycles, tape-outs, or wafer ASP structures.

Grading Penalty constraints:

If an AE candidate lacks direct experience with silicon IP, complex EDA contract negotiations, or wafer royalty models: Cap score to a MAXIMUM of 5.5/10.0.

[ROLE 6] Ecosystem & Partnerships / Developer Relations

Target Focus: Workforce development, university programs, developer marketing, third-party tooling alliances, and ecosystem adoption.

Primary Keywords: Developer Relations (DevRel), Ecosystem Alliances, University Programs, Academic Outreach, Workforce Development, Reference Designs, Open Source Governance, Co-marketing.

Skepticism Triggers:

General social media managers who post broad marketing announcements but have no plan for enabling developers, bridging academic curricula, or cultivating toolchain integration.

Grading Penalty constraints:

If a DevRel/Ecosystem candidate lacks a strategy for institutional workforce training, university course integrations, or technical reference board distribution: Cap score to a MAXIMUM of 5.8/10.0.

## 🚗 SEGMENT C: FUNCTIONAL SAFETY & AUTOMOTIVE TRACK

### [ROLE 7] RISC-V Functional Safety / Automotive Systems Engineer

Target Focus: ISO 26262 safety case ownership, AUTOSAR platform integration, ASIL-rated MCU bring-up, and zonal controller architecture for software-defined vehicles.

Primary Keywords: ISO 26262, ASIL, ASIL-D, ASIL-B, Functional Safety, HARA, FMEA, FTA, Safety Case, AUTOSAR, Classic AUTOSAR, Adaptive AUTOSAR, MCAL, lockstep, zonal controller, ECU, domain controller, ADAS, software-defined vehicle, SDV, RVM Profile, MCU Profile, AURIX, TriCore, S32K, S32G, RH850, MISRA C, CAN, FlexRay, automotive Ethernet, SOME/IP, Tasking, HighTec, Green Hills INTEGRITY.

Skepticism Triggers:
- Candidates who claim ISO 26262 experience based solely on awareness training, e-learning certificates, or attending a project as a peripheral contributor — no safety artifact ownership.
- "Automotive" experience limited to infotainment, head unit UX, or Android Automotive — these are QM (Quality Management) level, not ASIL-rated work.
- Claims of AUTOSAR experience that amount to using a generated BSW without configuring or troubleshooting MCAL drivers or OS resource scheduling.

Grading Penalty constraints:
- If a candidate claims ISO 26262 expertise but cannot identify the ASIL level they worked at, describe one safety mechanism they implemented, or name a safety artifact they owned: Cap score to a MAXIMUM of 3.5/10.0.
- If a candidate's automotive experience is limited to infotainment / multimedia / Android Automotive without ASIL-rated subsystem work: Cap score to a MAXIMUM of 4.0/10.0.

Transition Candidate Rule: Engineers from AURIX TriCore, NXP S32, or Renesas RH850 platforms must NOT be penalized for lacking RISC-V ISA familiarity. Their safety process depth, AUTOSAR knowledge, and automotive customer relationships are the primary evaluation signal. See isa-transition-matrix.txt Track D for full guidance.

## 🔒 SEGMENT D: SECURITY & CONFIDENTIAL COMPUTING TRACK

### [ROLE 8] RISC-V Security / Confidential Computing Engineer

Target Focus: Hardware-enforced isolation, trusted execution environments (TEE), silicon root-of-trust (RoT), confidential computing, and memory safety architectures on RISC-V.

Primary Keywords: TEE, Trusted Execution Environment, Confidential Computing, CoVE, CoVE-IO, Supervisor Domains, Caliptra, OpenTitan, Root of Trust, RoT, CHERI, CHERIoT, capability hardware, attestation, measured boot, secure boot, IOPMP, SPMP, HPMP, memory protection, memory tagging, hardware isolation, post-quantum cryptography, PQC, high assurance cryptography, speculation barriers, side channel, microarchitectural side channel, hardware fault isolation, compartmentalisation, security model, threat model, Keystone, ACE IBM, Penglai.

Skepticism Triggers:
- Candidates who claim "hardware security" experience based purely on software cryptography (TLS, JWT, OAuth) with no hardware isolation or silicon-level security mechanism knowledge.
- "TEE experience" limited to using an existing TEE API (e.g., calling TrustZone from an app) without implementing or modifying the TEE itself.
- Security architects with no semiconductor or embedded systems background attempting to claim hardware security expertise from pure enterprise/cloud security roles.

Grading Penalty constraints:
- If a candidate claims hardware security expertise but cannot explain the difference between a TEE and a secure enclave, or describe one hardware isolation primitive (IOPMP, SPMP, PMP): Cap score to a MAXIMUM of 4.0/10.0.
- If a candidate's security experience is limited to web application security, cloud IAM, or SAST/DAST tooling with no hardware boundary work: Cap score to a MAXIMUM of 3.0/10.0.

Bonus signals: Active contribution to OpenTitan, CoVE, Caliptra, or CHERIoT open-source repositories is an Automatic HIGH Match signal — treat as equivalent to Tier-1 company pedigree for this role.