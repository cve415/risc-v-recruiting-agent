# RISC-V Academic Ecosystem — China

**Compiled By:** Christopher Velasco, RISC-V International Academia & Training SIG member  
**Source:** CNKI/GitHub cross-reference, national CPU design competition records, 一生一芯 program institutional enrollment.

China is the most consequential RISC-V ecosystem outside the United States. US export controls on advanced semiconductors have made open-ISA RISC-V a national strategic priority. Key anchors: **XiangShan** (ICT/CAS — open-source OoO RISC-V at 14nm), **T-Head/Alibaba XuanTie** (ZJU cluster), and the **一生一芯 (One Life One Chip)** national tapeout program.

---

## ⚠️ COMPLIANCE NOTE
**Mandatory review required before routing Chinese institution candidates to roles involving US export-controlled technology.** This includes: EAR-controlled EDA tools, advanced process nodes below 14nm, space/radiation-hardened applications, and military/defense adjacency. Route to compliance review before Stage 2 evaluation for candidates from institutions with PLA/defense adjacency (NUDT, BUAA, BUIT). Standard commercial RISC-V roles (firmware, toolchain, open-source Linux) do not require special review. When in doubt, flag for human review.

---

## Tier 1 — Confirmed Named Programs or Production Tapeouts

### ICT/CAS (Institute of Computing Technology, Chinese Academy of Sciences) — Beijing
**Most impactful RISC-V research institution in China.** Origin of **XiangShan (香山)** — open-source, high-performance OoO RISC-V processor. Tapeouts: Yanqihu (28nm), Nanhu (14nm), performance comparable to ARM Cortex-A75/A76. Fully open-source on GitHub (OpenXiangShan). Graduate architecture courses use RISC-V as primary design target. XiangShan is the reference design studied and forked by universities across China.
- **Role routing:** Role 1 (Silicon Architecture — deepest microarchitecture signal in China), Role 2 (DV)
- **GitHub signals:** OpenXiangShan org, XiangShan repo forks, NEMU (reference simulator), difftest framework
- **Sourcing thesis:** ICT/CAS XiangShan contributor = China's strongest Lane A signal; deepest OoO microarchitecture knowledge outside Arm/Intel/AMD

### Zhejiang University (ZJU, 浙江大学) — Hangzhou, Zhejiang
Geographic anchor of China's RISC-V industry cluster. ZJU sits at the center of Hangzhou's tech ecosystem — home to Alibaba's DAMO Academy and T-Head Semiconductor (XuanTie C906/C910/C920 open-source RISC-V cores). ZJU–Alibaba joint research programs create direct pipeline from student RISC-V work to production chip deployment. Uncore PMU proposal to RISC-V ISA spec originated from T-Head at Hangzhou.
- **Role routing:** Role 1, Role 4 (Toolchain/Software — XuanTie ecosystem)
- **GitHub signals:** T-Head-Semi org, xuantie repos, ZJU CS architecture projects, Alibaba DAMO RISC-V repos

### Tsinghua University (清华大学) — Beijing
China's top-ranked university overall. Department of Computer Science and Technology + Institute of Microelectronics both produce RISC-V research. P&H RISC-V Edition as primary textbook. Faculty publications: RISC-V microarchitecture, hardware security, compiler backends. Student teams in national RISC-V design competitions.
- **Role routing:** Role 1, Role 8 (Security — hardware security research)
- **GitHub signals:** Tsinghua RISC-V design competition repos, hardware security extension projects

### Shanghai Jiao Tong University (SJTU, 上海交通大学) — Shanghai
CS359 (Computer Architecture) and graduate courses use RISC-V as design ISA. Published research: RISC-V accelerators, vector extensions, FPGA prototyping. National RISC-V competition participant. Located in Shanghai's semiconductor design hub.
- **Role routing:** Role 1, Role 3 (AI/ML — accelerator research)
- **GitHub signals:** SJTU CS RISC-V accelerator repos, vector extension projects

### Peking University (PKU, 北京大学) — Beijing
Intro to Computer Systems and Architecture courses adopt RISC-V as instructional ISA. Institute of Software contributes to open-source RISC-V toolchain. Students participate in national RISC-V CPU design contests. 一生一芯 program participant.
- **Role routing:** Role 1, Role 4 (Toolchain/Software — ISCAS/PLCT Lab affiliation common)
- **GitHub signals:** PKU RISC-V course repos, toolchain contribution history

### USTC (University of Science and Technology of China, 中国科学技术大学) — Hefei, Anhui
School of Computer Science and Technology: RISC-V in lab assignments (pipeline implementation). Students have won national RISC-V design competitions. Research: RISC-V reconfigurable computing and domain-specific accelerators. Founded by CAS — strong connection to ICT/CAS ecosystem. 一生一芯 participant.
- **Role routing:** Role 1, Role 3
- **GitHub signals:** USTC RISC-V tapeout repos, reconfigurable compute projects

### HUST (Huazhong University of Science and Technology, 华中科技大学) — Wuhan, Hubei
One of China's most structured RISC-V programs. Public lab materials include RISC-V pipeline design exercises. Faculty research: RISC-V IoT processors, security extensions, formal verification. Participant in **一生一芯 (One Life One Chip)** — students design and tape out a complete RISC-V SoC.
- **Role routing:** Role 1, Role 7/8 (security extensions)
- **GitHub signals:** HUST CS RISC-V pipeline labs, 一生一芯 tapeout project repos

### 一生一芯 (One Life One Chip) Program — National, led by ICT/CAS
Students design, verify, and tape out a complete RISC-V SoC from scratch — one chip per student lifecycle. **Participating universities (automatic Tier 1):** ICT/CAS, Peking University, Zhejiang University, HUST, Nanjing University, USTC. Any candidate citing 一生一芯 participation = highest-signal Role 1 or Role 2 indicator in China.
- **GitHub signals:** ysyx-workbench repos, 一生一芯 org, student SoC tapeout branches

### Southeast University (SEU, 东南大学) — Nanjing, Jiangsu
School of Electronic Science and Engineering: one of China's strongest microelectronics programs. RISC-V in digital IC design and computer architecture courses. Faculty research: RISC-V SoC design, VLSI, low-power embedded. Strong industry ties to Nanjing's chip design cluster (NXP China, Huawei Nanjing).
- **Role routing:** Role 1, Role 2
- **GitHub signals:** SEU ECE RISC-V SoC repos, VLSI design projects

### NUDT (National University of Defense Technology, 国防科技大学) — Changsha, Hunan
⚠️ **Compliance flag: defense-affiliated institution.** Tianhe supercomputer series origin. College of Computer: advanced processor design program. Graduate courses use RISC-V for HPC and reliable computing research. NUDT's influence on national computing standards gives RISC-V research policy relevance.
- **Role routing:** Role 1, Role 3 — **flag for compliance review before any US export-controlled role**
- **GitHub signals:** RISC-V HPC project repos (public), custom ISA extension work

---

## Tier 2 — Active Teaching Materials or Project-Based Use

- **Fudan University (Shanghai)** — School of Microelectronics; RISC-V in graduate chip design coursework and student tapeouts. Shanghai semiconductor cluster. Role 1/2.
- **Nanjing University (NJU)** — 一生一芯 participant (on cusp of Tier 1); computer science P&H RISC-V adoption. Role 1.
- **UESTC (Chengdu)** — China's most electronics-specialized university; RISC-V in digital systems and SoC design; Chengdu chip design hub. Role 1.
- **Harbin Institute of Technology (HIT)** — Top engineering university in Northeast China; national RISC-V competition participants. Role 1.
- **Beihang University (BUAA)** — ⚠️ Aerospace/defense-oriented. Computer architecture and embedded systems referencing RISC-V; fault-tolerant and real-time systems research. **Compliance review required for US export-controlled roles.**
- **Xi'an Jiaotong University (XJTU)** — One of China's original Jiaotong universities; ECE architecture coursework with RISC-V edition materials. Role 1.
- **Sun Yat-sen University (SYSU, Guangzhou)** — Pearl River Delta region; Huawei HQ proximity creates industry pull. CS/ECE architecture with RISC-V. Role 1.
- **SCUT (Guangzhou)** — South China engineering programs; ECE/CS tracking RISC-V textbook transition; embedded IoT research. Role 1.
- **Wuhan University** — CS/ECE near HUST cluster; cross-institutional RISC-V influence. Role 1.
- **BIT (Beijing Institute of Technology)** — ⚠️ Defense-adjacent. Safety-critical systems research with RISC-V alignment. **Compliance review required.**
- **ISCAS/PLCT Lab (Beijing)** — Not degree-granting, but China's most important RISC-V toolchain contributor: GCC, LLVM, QEMU for RISC-V. Graduate students from top Chinese universities; output underpins RISC-V education nationally.
  - **GitHub signals:** plctlab org, PLCT-RISC-V repos, QEMU-RISCV patches, LLVM RISC-V backend PRs
  - **Role routing:** Role 4 (Toolchain/Software) — one of the strongest global signals for this role

---

## China Sourcing Context

- **Export control accelerant:** US restrictions on advanced chip tech (EDA, advanced nodes) have made RISC-V a national strategic priority — university adoption is partially policy-driven, creating a large and fast-growing talent pool.
- **National CPU design competitions:** China holds annual national RISC-V processor design competitions — school participation is a reliable Tier 1 or Tier 2 signal.
- **一生一芯 signal:** Any candidate citing 一生一芯 participation has designed and taped out a real RISC-V chip as part of their degree — the most direct academic RISC-V integration anywhere in the world.
- **T-Head/XuanTie multiplier:** Alibaba's open-source RISC-V cores (C906, C910, C920) are widely used in Chinese university labs — particularly ZJU and partner institutions in the Hangzhou–Shanghai corridor.
- **PLCT Lab:** China's equivalent of India's NPTEL for toolchain — PLCT propagates RISC-V capability to universities without independent infrastructure.
- **Verification path:** Cross-reference CNKI and GitHub for RISC-V publications and student repositories. National CPU design competition leaderboards are a direct institutional engagement signal.
