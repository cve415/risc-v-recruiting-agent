# AGENT SIGNAL: Academic Weighting & Course Code Heuristics
**Role:** Data Signal for Sourcing Swarm
**Confidential:** Internal Use Only - CVE Sourcing

## 1. HIGH-SIGNAL COURSE CODES (Automatic Tier-1)
If these specific courses or labs appear on a resume/transcript, the agent should flag the candidate as "Technically Vetted":

- **U-Michigan [EECS 470]:** High Signal for OoO (Out-of-Order) logic.
- **UPenn [CIS 5710]:** High Signal for RV32IM custom core design.
- **UT Arlington [CSE 4372]:** High Signal for FPGA-based processor testing.
- **Cornell [CS 3410]:** High Signal for Hardware/Software abstraction mastery.
- **Tufts [RV32I]:** Entry-level machine computing proficiency.

## 2. INSTITUTIONAL "PEDIGREE" WEIGHTING
Use these categories to bias search results in LinkedIn/GitHub X-Ray:

### A. The "Architect" Tier (Heavy R&D Focus)
- **UC Berkeley, MIT, Stanford, CMU, Georgia Tech.**
- *Agent Action:* Prioritize for Lead Architect and Principal RTL roles.

### B. The "Implementation" Tier (Hands-on RTL/FPGA)
- **UNLV, ASU, UT Arlington, Portland State, Rice.**
- *Agent Action:* Prioritize for Design Verification (DV) and SoC Integration roles.

### C. The "Security/Niche" Tier
- **Penn State (Radiation Hardened/Space), UCSD (Hardware Security).**
- *Agent Action:* Flag for Aerospace, Defense, or Secure Silicon requirements.

## 3. PROFESSIONAL PIVOT SIGNALS (Mid-Career)
If a candidate with 10+ years experience has these certs, treat as a "Successful Pivot":
- **LFD114 (Porting Software):** Flags a candidate capable of migrating legacy ARM/x86 codebases to RISC-V.
- **edX "Industrial Architecture":** Flags readiness for production-level SoC design.

## 4. AGENT SEARCH STRINGS
(Copy-paste for LinkedIn/GitHub Swarms):
- `(EECS 470 OR CIS 5710 OR CSE 4372 OR CS 3410) AND "RISC-V"`
- `"RVfpga" AND (UNLV OR "Arizona State" OR "UT Arlington")`
- `("LFD110" OR "LFD114") AND "Engineer"`
