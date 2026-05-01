# SKILL: Technical & ISA Vetting (RISC-V Engineering)
**Version:** 1.2 (Optimized for Kimi K2.6)
**Target Roles:** Silicon Architect, RTL Engineer, Design Verification (DV), Compiler Engineer.

## 1. CORE ARCHITECTURAL SIGNALS
The agent must scan repositories for these specific implementation patterns rather than just "RISC-V" mentions.

### 1.1 Instruction Set Architecture (ISA) Depth
- **Extension Implementation:** Look for code-level evidence of `RV32`/`RV64` with:
  - `V` (Vector 1.0) - **Critical Signal**: Check for vector register file logic or ALU implementations.
  - `M` (Multiply), `A` (Atomic), `F/D` (Floating Point).
  - `K` (Scalar Cryptography) or `B` (Bit Manipulation).
- **Control & Status Registers (CSRs):** Look for custom CSR mapping or privilege mode handling (Machine, Supervisor, User).

### 1.2 Hardware Description & Verification (HDL)
- **RTL Quality:** Analyze SystemVerilog or Verilog for modularity. 
  - *Green Flag:* Use of parameterized modules and clean clock/reset strategies.
- **Verification Frameworks:** Search for `UVM` (Universal Verification Methodology) or `cocotb` (Python-based verification).
- **Alternative HDLs:** Evidence of modern hardware construction: `Chisel`, `Bluespec`, or `SpinalHDL`.

### 1.3 System-on-Chip (SoC) Infrastructure
- **Interconnects:** Implementation of `TileLink`, `AMBA AXI/AHB`, or `CHI` (Coherent Hub Interface).
- **Memory Hierarchy:** Cache controller design, TLB (Translation Lookaside Buffer) logic, or DMA controllers.

## 2. THE "QUALITY" HEURISTIC (1-10)
Assign a **Technical Fidelity Score** based on commit behavior:
- **Lvl 1-3 (Surface):** Forked popular repos (e.g., RocketChip) with no original commits or only doc changes.
- **Lvl 4-6 (Contributor):** Fixed bugs in existing cores; implemented peripheral controllers (SPI, UART, JTAG).
- **Lvl 7-9 (Architect):** Implemented a custom multi-stage pipeline, branch predictor, or out-of-order execution logic.
- **Lvl 10 (Master):** Maintainer of a major core (OpenTitan, VeeR, Ibex) or major contributor to RISC-V International specs.

## 3. COMPILER & TOOLCHAIN SIGNALS
*For Software/Firmware roles:*
- **LLVM/GCC:** Search for "Instruction Selection," "Peephole Optimizations," or "Custom Backend" work.
- **Simulators:** Contributions to `Spike`, `QEMU`, or `Renode`.

## 4. OUTREACH THESIS GENERATOR
When drafting the outreach, the agent must reference a **specific file or commit**:
- *Hook:* "I was reviewing your implementation of the [Feature] in [Repo Name]. Your approach to handling [Technical Challenge, e.g., pipeline hazards/vector chaining] was impressive and aligns with our current roadmap at [Client]."