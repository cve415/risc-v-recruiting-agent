Target Domains: Hardware Architecture, RTL Design, Verification, and Systems Toolchains.

1. ARCHITECTURAL EVALUATION
The agent performs a deep-scan of repository history to verify implementation proficiency across core architectural concepts.

1.1 ISA Implementation & Optimization
Instruction Set Depth: Evaluates the agent's ability to identify specific extensions and custom instruction implementations within open-source cores.

Privilege & Control Logic: Scans for sophisticated handling of system-level registers, custom CSRs, and privilege modes.

Performance Heuristics: Identifies work related to pipeline design, branch prediction, and execution unit optimization.

1.2 Hardware Construction & Verification
HDL Design Patterns: Audits SystemVerilog/Verilog for modularity, parameterization, and clock-domain crossing (CDC) management.

Modern Hardware Methodologies: Recognizes expertise in alternative hardware construction languages (Chisel, Bluespec, etc.).

Verification Rigor: Identifies the use of industry-standard frameworks (UVM) and modern Python-based verification environments.

1.3 System & Interconnect Infrastructure
Fabric & Bus Protocol: Assesses experience with high-performance interconnects and coherent hub interfaces.

Memory Subsystems: Evaluates expertise in cache hierarchy, memory management units (MMUs), and DMA controller design.

2. TECHNICAL FIDELITY SCORING (TFS)
The agent assigns a weighted score (1-10) based on the nature of contributions, moving beyond basic activity metrics:

Foundational: Assessment of repository engagement and basic peripheral integration.

Contributory: Evaluation of bug fixes, optimization of existing modules, and unit-level verification.

Architectural: Verification of original pipeline design, complex subsystem implementation, or out-of-order logic.

Core Maintainer: Recognition of leadership or primary maintainer status for widely-adopted industry cores and specifications.

3. TOOLCHAIN & LOW-LEVEL SOFTWARE
Compiler Engineering: Identifies contributions to backend optimizations, instruction selection, and custom target support.

Simulation & Modeling: Analyzes contributions to cycle-accurate simulators and hardware modeling environments.

4. CONTEXTUAL ENGAGEMENT GENERATOR
The agent utilizes the technical audit to draft a High-Context Thesis for each lead. This ensures outreach is grounded in actual engineering work:

Contribution-Led Hooks: Outreach is triggered by specific design choices identified during the repository scan.

Alignment Narrative: Maps a candidate’s specific technical challenges (e.g., hazard mitigation or vector processing) to the client’s current technical roadmap.
