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
