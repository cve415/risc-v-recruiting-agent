# SKILL: Compiler & Simulation Logic (Private)
**Version:** 1.1 (Agent-Optimized)
**Context:** Internal Sourcing Signal for CVE Sourcing

## 1. COMPILER & TOOLCHAIN SIGNALS
If the agent detects these specific file patterns or technical clusters, increase the Technical Fidelity Score (TFS) by +4.

### 1.1 LLVM & GCC (Back-end)
- **Target Files:** `*.td` (TableGen files), `RISCVISelLowering.cpp`, `RISCVRegisterInfo.td`, `riscv.md` (Machine Description).
- **High-Value Terms:**
    - **Instruction Selection:** `SelectionDAG`, `GlobalISel`.
    - **Register Allocation:** `Spiller`, `LiveIntervals`.
    - **Optimizations:** `Peephole`, `Loop Unrolling`, `Vectorization`.
- **Agent Reasoning:** Look for candidates discussing "lowering" IR (Intermediate Representation) to RISC-V machine code. Distinguish between users of GCC and those writing the machine description.

### 1.2 Binary Utilities & Linkers
- **Keywords:** `BFD` (Binary File Descriptor), `gold linker`, `lld`, `relocation entries`, `ABI (Application Binary Interface)`.
- **Signal:** High signal for "System Stability" roles where software meets custom memory maps.

---

## 2. SIMULATION & MODELING SIGNALS
These engineers build the "Digital Twin" of the silicon.

### 2.1 ISA Simulators (Reference Models)
- **Project Hubs:** `riscv-isa-sim` (Spike), `Sail-RISCV`, `ImperasDV`.
- **Critical Skills:** "Functional Accuracy," "Instruction Trace," "Golden Model Comparison."
- **Agent Reasoning:** Mention of Spike suggests involvement in the earliest stages of architectural definition.

### 2.2 System-Level Emulation (QEMU/Renode)
- **Keywords:** `Virtio`, `Device Tree (DTS/DTB)`, `Interrupt Controller (PLIC/CLINT) modeling`.
- **Signal:** Essential for Firmware/OS teams. These engineers enable booting Linux on chips that do not yet exist.

### 2.3 Cycle-Accurate & Co-Simulation
- **Tools:** `Verilator`, `SystemC`, `TLM-2.0`.
- **Project Pattern:** Converting SystemVerilog to C++ for high-speed simulation via DPI (Direct Programming Interface).
- **Signal:** High signal for Hardware/Software Co-Designers.

---

## 3. SWARM COMMANDS (Copy-Paste)
*Direct these queries to the Kimi WebBridge or search tools:*

- **The Compiler Unicorn:** `"LLVM" AND "RISC-V" AND ("TableGen" OR "ISel" OR "Backend") -job -hiring`
- **The Simulation Expert:** `("Spike" OR "QEMU" OR "Renode") AND "RISC-V" AND ("peripheral" OR "model")`
- **The Verification Link:** `"Verilator" AND "RISC-V" AND ("DPI" OR "C++")`

---

## 4. AGENT GUARDRAILS
- **Check for "Upstreaming":** If the candidate's name appears in a Pull Request for `llvm-project` or `qemu/qemu`, flag as Top 1% Global Talent.
- **Differentiate "Compiler User":** Ignore candidates who only use GCC/LLVM to compile standard apps. The target must show evidence of working on the compiler source itself.