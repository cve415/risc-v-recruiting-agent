# SKILL: RISC-V Domain Validation & Artifact Verification
**Category:** Technical Screening & Sourcing Automation  
**Target Repository:** `riscv-recruiting-agent`

## 1. INSTRUCTION SET ARCHITECTURE (ISA) VERIFICATION
The agent possesses the ability to parse, identify, and validate source-code level evidence of specific RISC-V specifications and implementation depth rather than relying on surface-level keyword matching.

### 1.1 Base ISA & Extension Identification
The agent scans repository architectures, assembly configurations, and build manifests for valid extension usage:
* **`RV32` / `RV64` Base Configurations:** Identifies implementation boundaries (e.g., register width, integer base profiles).
* **`V` (Vector Extension 1.0):** Looks for vector configuration registers (`vsetvli`), vector ALU pipeline handling, or explicit vector execution logic.
* **Specialized Subsets:** Identifies code references mapping to `M` (Integer Multiplication/Division), `A` (Atomic Instructions), `F/D` (Single/Double Precision Floating-Point), `K` (Scalar Cryptography), and `B` (Bit Manipulation).

### 1.2 Low-Level Control Inspection
* **CSR (Control and Status Registers):** Evaluates whether code defines or interacts with standard custom CSR mapping or privilege mode boundaries (Machine, Supervisor, User modes).

---

## 2. HARDWARE DESIGN & SIMULATION CAPABILITIES
The agent analyzes repositories written in Hardware Description Languages (HDLs) to determine design complexity, modularity, and structural quality.

### 2.1 RTL Architecture Analysis
* **SystemVerilog / Verilog Engineering:** Quantifies parameterized design methodologies, modular grouping structures, and explicit clocking/reset domain protocols.
* **Modern Chisel / Bluespec / SpinalHDL Systems:** Maps non-traditional hardware description structures to verify high-level parameter generation.

### 2.2 Functional Verification Frameworks
* Sweeps file structures for active logic verification harnesses built on top of:
  * **`UVM`** (Universal Verification Methodology)
  * **`cocotb`** (Python-based coroutine verification environments)

### 2.3 System-on-Chip (SoC) Infrastructure Mapping
* **Bus & Interconnect Protocols:** Validates logic implementing standard infrastructure architectures: `TileLink`, `AMBA AXI/AHB`, or `CHI` (Coherent Hub Interface).
* **Memory Subsystems:** Detects design components dedicated to cache controllers, Translation Lookaside Buffers (TLB), or Direct Memory Access (DMA) units.

---

## 3. SYSTEM SOFTWARE & TOOLCHAIN DEPLOYMENT
For software-centric and firmware profiles, the agent assesses compiler, simulator, and runtime interface familiarity.

### 3.1 Compiler Backend Auditing
* **LLVM / GCC Implementations:** Identifies files containing architecture-specific modifications, custom target backend parameters, instruction selection passes, or custom peephole optimization flags.

### 3.2 Simulation & Architectural Modeling
* Detects integration hooks or code contributions targeted toward structural simulation utilities:
  * `Spike` (RISC-V ISA Simulator)
  * `QEMU` (System Emulation)
  * `Renode` (Multi-node Framework)

---

## 4. AUTOMATED OUTREACH THESIS GENERATION
Utilizing the structural indicators gathered from the skills above, the agent executes contextual synthesis routines:
* Maps specific technical implementations (e.g., pipeline hazard remediation, custom branch prediction, or vector chaining logic) to create precise, context-driven engagement summaries.