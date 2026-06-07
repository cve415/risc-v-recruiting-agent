# RISC-V Academic Ecosystem — India

**Compiled By:** Christopher Velasco, RISC-V International Academia & Training SIG member  
**Source:** IIT course catalogs, NPTEL module records, SHAKTI program documentation, faculty Lattes/Google Scholar profiles.

India has the most concentrated academic RISC-V momentum outside the United States. Three overlapping forces: IIT Madras's **SHAKTI processor program** (government-funded domestic RISC-V silicon), **MeitY's national RISC-V push**, and the **NPTEL** open courseware platform distributing IIT-produced architecture content to millions of students nationally.

---

## Tier 1 — Confirmed Named Programs or Production Tapeouts

### IIT Madras — Chennai, Tamil Nadu
**Anchor of Indian RISC-V academia.** SHAKTI Processor Program: multiple production tapeouts (C-class through E-class RISC-V cores) funded by MeitY + NaMPET. RISE Lab leads the work. CS6600 and Computer Architecture courses use RISC-V. NPTEL courses produced here use RISC-V as primary ISA — multiplied to thousands of affiliated colleges nationally. SHAKTI cores open-sourced on GitHub.
- **Role routing:** Role 1 (Silicon Architecture — deepest microarchitecture output in India), Role 2 (DV/Verification)
- **GitHub signals:** shaktiproject org, SHAKTI-SDK, c-class/e-class RISC-V repos, Bluespec BSV RISC-V implementations
- **Sourcing thesis:** IIT Madras SHAKTI contributor = strongest Lane A signal in India; equivalent to US Tier 1 in terms of silicon depth

### IIT Bombay — Mumbai, Maharashtra
CS 683 (Advanced Computer Architecture) and related courses use RISC-V. Faculty publications include RISC-V microarchitecture and memory hierarchy research. Strong NPTEL contribution.
- **Role routing:** Role 1, Role 2
- **GitHub signals:** RISC-V pipeline simulators, memory hierarchy research repos, CS683 lab materials

### IIT Kanpur — Kanpur, Uttar Pradesh
CS422 uses *Patterson & Hennessy RISC-V Edition* as primary text — one of the earliest IITs to formally adopt it. Graduate research covers processor design and RISC-V compiler backends.
- **Role routing:** Role 1, Role 4 (Toolchain/Software)
- **GitHub signals:** RISC-V assembler/simulator student projects, LLVM backend patches

### IIT Delhi — New Delhi
COL216 (Computer Architecture) and COL718 (Advanced) use RISC-V for pipeline design and hazard analysis. Public course materials include RISC-V assembly exercises.
- **Role routing:** Role 1, Role 2
- **GitHub signals:** RISC-V pipeline lab repos, COL216 simulation frameworks

### IIT Kharagpur — Kharagpur, West Bengal
NPTEL courses on Computer Organisation and Architecture produced by IIT Kharagpur faculty use RISC-V. One of the original IITs with large ECE/CS output; adoption here propagates nationally.
- **Role routing:** Role 1, Role 2
- **GitHub signals:** RISC-V coursework repos, digital design FPGA projects

### Indian Institute of Science (IISc) — Bangalore, Karnataka
India's premier research university. CSA and ECE departments produce RISC-V microarchitecture, hardware security, and VLSI research. Graduate architecture courses use RISC-V as reference ISA. Proximity to Bangalore's semiconductor cluster (Qualcomm, Intel, Arm India) accelerates research-to-industry transfer.
- **Role routing:** Role 1, Role 8 (Security)
- **GitHub signals:** RISC-V accelerator research repos, hardware security extensions, custom ISA work
- **Sourcing thesis:** IISc PhD/MTech = India's strongest academic research signal; treat as equivalent to US research university Tier 1

### IIT Hyderabad — Hyderabad, Telangana
Published research on RISC-V accelerators and custom ISA extensions. Computer Architecture coursework uses RISC-V. Collaboration with Hyderabad's semiconductor cluster (Qualcomm, Intel, TSMC design centers).
- **Role routing:** Role 1, Role 3 (AI/ML Acceleration)
- **GitHub signals:** RISC-V custom extension repos, accelerator design projects

---

## Tier 2 — Active Teaching Materials or Project-Based Use

### IIT Roorkee — Roorkee, Uttarakhand
ECE/CS architecture sequences moving toward RISC-V via P&H textbook transition. Embedded systems and digital design research. Role 1 pipeline.

### IIT BHU (IIT Varanasi) — Varanasi, Uttar Pradesh
Electronics Engineering with computer architecture coursework. VLSI design research supports Tier 2 placement. Role 1.

### IIT Guwahati — Guwahati, Assam
CS and ECE in Northeast India's flagship institution. Architecture faculty with RISC-V alignment. Role 1.

### IIIT Hyderabad — Hyderabad, Telangana
Center for VLSI and Embedded Systems Technology (CVEST): RISC-V publications and student projects. Graduate architecture courses reference RISC-V. Role 1/2.
- **GitHub signals:** CVEST org, RISC-V accelerator and verification repos

### BITS Pilani — Rajasthan (+ Goa, Hyderabad campuses)
India's top private technical university. Strong undergraduate research culture; documented RISC-V processor implementations and FPGA projects on GitHub. Role 1/4.

### NIT Tiruchirappalli (NIT Trichy) — Tiruchirappalli, Tamil Nadu
Top-ranked NIT. ECE architecture courses adopted RISC-V edition textbooks. Role 1.

### NIT Calicut — Kozhikode, Kerala
Strong ECE/CS programs; Kerala's open-source culture reinforces adoption. Computer architecture moving to RISC-V. Role 1.

### IIIT Bangalore — Bangalore, Karnataka
Research-focused IIIT with Bangalore chip design industry ties. VLSI, embedded systems, and architecture capstone projects include RISC-V core implementations. Role 1/2.

### Jadavpur University — Kolkata, West Bengal
One of India's oldest state engineering universities. ECE and CS VLSI/digital design research groups. Role 1.

### Anna University — Chennai, Tamil Nadu
Apex university for Tamil Nadu, affiliating hundreds of colleges. Close to IIT Madras and SHAKTI ecosystem; faculty collaboration drives RISC-V exposure in affiliated programs. Role 1.

---

## India Sourcing Context

- **MeitY policy pull:** India's Ministry of Electronics and IT explicitly backs domestic RISC-V chip development — RISC-V university adoption is partly policy-driven, accelerating pipeline formation.
- **NPTEL multiplier:** IIT-produced NPTEL RISC-V content reaches millions of students at affiliated colleges — any IIT Tier 1 entry effectively propagates to hundreds of downstream institutions. A candidate citing NPTEL course completion is a valid signal.
- **India Semiconductor Mission (₹76,000 crore):** Semiconductor incentive program is creating upstream pressure on universities to formalize RISC-V coursework — expect Tier 2 promotions over 2025–2027.
- **Bangalore cluster:** IISc + IIIT Bangalore + Jadavpur alumni heavily populate Bangalore's chip design centers (Qualcomm, Intel, Arm, Marvell India). RISC-V exposure from these schools maps directly to transition candidate (Lane B) pipeline.
- **Verification path:** Cross-reference faculty Lattes CVs or Google Scholar for RISC-V publications. SHAKTI GitHub org activity is the strongest signal for IIT Madras origin.
