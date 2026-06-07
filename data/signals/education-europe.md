# RISC-V Academic Ecosystem — Europe

**Compiled By:** Christopher Velasco, RISC-V International Academia & Training SIG member  
**Source:** RISC-V Europe Summit 2023/2025/2026 presenter affiliations; Horizon Europe project records.

Europe is one of three global centers of RISC-V academic gravity. Key structural advantages: **PULP Platform** (ETH/Bologna — most-forked open RISC-V IP globally), **European Processor Initiative (EPI)**, and **BSC Barcelona** anchoring safety-critical research. Talent here skews toward silicon architecture, security/PQC, and HPC — strong Lane A supply.

---

## Tier 1 — Confirmed Named Programs or Production Tapeouts

### ETH Zurich — Zurich, Switzerland
Origin of the PULP Platform (CVA6/Ariane, Ibex, Snitch). Prof. Luca Benini's IIS lab is the most productive source of open RISC-V IP in Europe. Multiple tapeouts confirmed at IHP 130nm open PDK (Croc SoC, MLEM, HyperCroc). Computer architecture courses use RISC-V as primary ISA. RISC-V Europe 2025 keynote + 2026 papers confirm ongoing leadership in physical AI, confidential computing (CAGE-V), and open toolchain (Loom).
- **Role routing:** Role 1 (Silicon Architecture), Role 2 (DV/Formal), Role 8 (Security/Confidential)
- **GitHub signals:** CVA6/ariane forks, PULP SDK, Snitch repos, IIS-ETH org, Loom, X-HEEP (EPFL joint)
- **Sourcing thesis:** Any contributor to CVA6, Ibex, or Snitch is a Tier-1 Lane A signal regardless of current employer

### University of Bologna — Bologna, Italy
Co-originator of PULP Platform with ETH Zurich. Dual appointment of Prof. Benini. Produces graduates who enter GreenWaves, SiFive, and OEM edge-AI roles. 2026 Astral project (RISC-V for space AI). 5G NTN space comms paper confirms RVV vector extension as strategic research direction.
- **Role routing:** Role 1 (Silicon Architecture), Role 3 (AI/ML Acceleration)
- **GitHub signals:** PULP Platform org, GAP8-SDK, Hero-PULP, RedMulE, Spatz (RVV), MAGIA-V
- **Sourcing thesis:** Bologna Laurea Magistrale = US MS equivalent (Bologna Process); do not discount

### Barcelona Supercomputing Center (BSC) / UPC — Barcelona, Spain
Europe's strongest RISC-V safety-critical research. Produces NOEL-V processor (SafeLS lockstep), Sargantana RV64GBV, post-quantum crypto (HQC on RISC-V). RISC-V Educator of the Year 2019 (Dr. Leonidas Kosmidis). Active on FRACTAL, NimbleAI, METASAT, AERO Horizon Europe projects. 2026: PQC for EU passports (PQC4eMRTD), vector cache design (Bicameral+).
- **Role routing:** Role 1 (HPC/Safety-Critical), Role 7 (FuSa — NOEL-V lockstep), Role 8 (Security/PQC)
- **GitHub signals:** bsc-caos org, NOEL-V repos, Sargantana, RAVE profiling tool, BSC-HPC
- **Sourcing thesis:** BSC candidates typically have dual strength in HPC + safety; route FuSa evaluator if lockstep/ASIL keywords present

### Technical University of Munich (TUM) — Munich, Germany
Prof. Georg Sigl's security group: three RISC-V ASIC tapeouts for post-quantum crypto (UMC 65nm, GF 22nm). Participant in Scale4Edge. Computer architecture and embedded systems courses reference RISC-V.
- **Role routing:** Role 8 (Security), Role 1 (Silicon Architecture)
- **GitHub signals:** TUM-LIS org, RISC-V PQC ASIC repos, Scale4Edge project repos
- **Talent thesis:** TUM PQC ASIC work = strongest European signal for Role 8 hardware security

### University of Cambridge — Cambridge, United Kingdom
Home of **CHERI-RISC-V** (with lowRISC and SRI International). Authors of the frozen RV64Y (CHERI) RISC-V extension spec. Prof. Simon Moore (hardware), Prof. Robert Watson (CHERI project lead). 2026: RVY ratification infrastructure (formal golden model, fuzz testing via Sail, FPGA at scale).
- **Role routing:** Role 8 (Security/Confidential Computing)
- **GitHub signals:** CTSRD-CHERI org, cheriot-ibex, sail-cheri-riscv, temporal-safety repos
- **Sourcing thesis:** Cambridge CHERI contributors are the highest-signal Role 8 candidates in Europe

### Politecnico di Torino — Turin, Italy
Most concentrated PQC ISA extension work in Europe (CIRCE, HORCRUX, CHIMERA at 65nm ASIC ~26.3 kGE). Prof. Matteo Sonza Reorda: RISC-V Self-Test Libraries for safety-critical. Side-channel + fault injection research (Flush+Reload on gem5, InjectV framework).
- **Role routing:** Role 8 (Security/PQC), Role 7 (FuSa — STL work)
- **GitHub signals:** VLSI-EDA-PoliTo org, InjectV, ML-KEM accelerator repos, CV32E40P extensions

### CEA (Leti + List) — Grenoble / Paris-Saclay, France
France's primary RISC-V institution. CVA6-based SoC platform (ALPES), Flying V (ECC-hardened HPDcache), Fault-Tolerant CVA6 (DCLS + SEU, targeting 18nm AI SoC), ANSSI IPECC side-channel-resistant ECC accelerator. Active in EPI.
- **Role routing:** Role 1 (Silicon Architecture/Space), Role 7 (FuSa — DCLS/SEU), Role 8 (Security)
- **GitHub signals:** CEA-LIST org, CVA6 forks with ECC, HPDcache, ALPES platform
- **Sourcing thesis:** CEA candidates at Leti/List typically have silicon depth + Horizon Europe collab history

---

## Tier 2 — Active Research or Project-Based RISC-V Use

### Germany
- **RPTU Kaiserslautern-Landau** — transient-execution side-channel detection in OoO RISC-V (SonicBOOM); Scale4Edge participant. Role 2/8.
- **University of Bremen / DFKI** — formal verification of RISC-V (Prof. Drechsler). Role 2.
- **Forschungszentrum Jülich** — RVV BLIS kernel generation; EUPILOT HPC project. Role 3.
- **IHP Microelectronics (Leibniz)** — fault injection on Ibex, TETRISC quad-core RISC-V SoC. Operates the IHP 130nm open PDK used by ETH/EPFL for academic tapeouts. Role 1/2.

### France
- **University of Rennes / IRISA / INRIA** — dual-core lockstep RISC-V via HLS for real-time safety. Role 7.
- **Mines Saint-Étienne (IMT)** — CEA Leti PhD co-supervision; microelectronics / security. Role 8.
- **Université Grenoble Alpes / TIMA Lab** — high-performance RISC-V microarchitecture (Arthur Perais). Role 1.

### Switzerland
- **EPFL — Lausanne** — X-HEEP open RISC-V SoC platform (Pasquale Schiavone); first silicon at IHP 130nm. Joint ETH/EPFL tapeout flow. Role 1. GitHub: epfl-iis/x-heep.

### United Kingdom
- **University of Manchester (APT Group)** — TornadoVM RISC-V, AERO project. Role 3.
- **University of Edinburgh / EPCC** — RISC-V in HPC emerging architecture evaluation. Role 3.
- **lowRISC CIC (Cambridge/Bristol)** — maintains Ibex and OpenTitan; key node connecting ETH open-source IP to production. Role 1/8.

### Spain
- **Universidad de Cantabria** — RISC-V educational HW lab curriculum development. Role 1 pipeline.
- **IMSE-CNM / Universidad de Sevilla** — Root-of-Trust (RO-PUF/TRNG) for RISC-V SoCs. Role 8.
- **UPV Valencia** — TinyML matrix mul on multicore RISC-V (GAP8). Role 3.

### Italy
- **Sapienza University of Rome** — Dynamic TMR on RISC-V microarchitecture. Role 7 (fault tolerance).
- **University of Pisa** — HW-SW interface for RAS on RISC-V. Role 1.
- **University of Torino** — distributed workflows on RISC-V HPC. Role 3.

### Belgium
- **KU Leuven / imec-DistriNet** — RISC-V hardware security (Prof. Frank Piessens). Role 8.

### Netherlands
- **University of Twente** — SmallSat RISC-V payload platform (space). Role 1 (space/rad-hard track).

### Austria
- **Johannes Kepler University Linz** — DSL for RISC-V pipeline visualization; toolchain/verification. Role 2.
- **TU Wien** — Philipp Tomsich (VRULL; RISC-V TSC Vice-Chair) spent decade here; matrix extension (IME/VME) contributor. Role 1/3.

### Portugal
- **Universidade do Minho** — CROSSCON IoT security stack with RISC-V (Prof. Sandro Pinto). Role 8.

### Greece
- **University of Athens** — Vitamin-V Horizon Europe project (RISC-V cloud stack: QEMU, gem5, OpenStack, Kubernetes); CTVS cache timing vulnerability scoring on RISC-V. Role 3/8.
- **ICS-FORTH (Crete)** — RISER project: all-European RISC-V cloud server prototypes (EPAC1.5 vector processor). Role 3.

### Albania *(Emerging — national policy initiative)*
- **University of Tirana** — Digital Valley Albania EDIH; explicit national strategy to embed RISC-V in CS education. No Tier 1 coursework yet; monitor Kushtrim Shala (Co-Founder, Digital Valley Albania) as key contact.

---

## European Sourcing Context

- **PULP affiliation** is the strongest single Lane A signal in Europe — treat any contributor to CVA6, Ibex, Snitch, or Spatz as Tier 1 regardless of institutional affiliation.
- **Horizon Europe project participant** (FRACTAL, NimbleAI, METASAT, AERO, CROSSCON, Scale4Edge, Vitamin-V, RISER) = confirmed RISC-V research exposure; route for deeper evaluation.
- **IHP 130nm open PDK tapeouts** = silicon-level proof of RISC-V competency; strongest possible signal for Role 1 or Role 2 from European candidates.
- **PQC wave (2026):** Seven+ European institutions are publishing RISC-V PQC ISA extension papers; this cohort will enter industry 2026–2028. Role 8 pipeline building now.
- **Degree equivalency:** Bologna Process 3+2 (Laurea Triennale + Laurea Magistrale) = US BS + MS. Do not discount.
- **Language of repos:** European contributors often mix English/native-language READMEs. Do not penalize.
