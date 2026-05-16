# 🌐 The RISC-V Monitoring & Observability Landscape

Many of my favorite memories in performance engineering, monitoring, and observability were formed during my years at New Relic and AppDynamics, watching developers hunt down complex bottlenecks across front-end systems and server code. More often than not, the true culprit wasn't a poorly written function—it was memory bandwidth saturation, cache thrashing, or interconnect contention happening quietly outside the CPU core. These hardware bottlenecks used to be incredibly difficult to diagnose until it was too late.

RISC-V's emerging **Uncore PMU (Performance Monitoring Unit)** proposal—originating from the team at Alibaba—tackles exactly this architectural blind spot. By standardizing performance monitoring for last-level caches, memory controllers, coherent interconnects, and I/O subsystems, it brings deep observability to the exact places where modern AI, HPC, and data center scale-out workloads live or die.

---

## 💡 Why This Layer Matters

| Target Audience | The Value Proposition |
| :--- | :--- |
| **🔧 For Developers** | Gain the exact uncore visibility Intel and ARM engineers already take for granted. Shift from blind scheduler tuning to data-driven layout optimization by exposing real-time memory bandwidth constraints. |
| **🐧 For Open-Source** | Establishes a unified standard integrated natively with Linux `perf`. This ensures RISC-V won't fragment into vendor-locked, proprietary monitoring silos. |
| **📈 For Business / GTM** | Uncore telemetry is non-negotiable table stakes for enterprise cloud adoption. When tier-1 customers ask, "Can we profile our custom workloads on your silicon?" this architecture gets the ecosystem to "yes." |

---

## 🗺️ Key Ecosystem Players (The Top 10)
*Organizations driving innovation across hardware telemetry, pre-silicon verification, and system-level event monitoring.*

### 🇨🇳 Alibaba (Hangzhou, China)
* **Category:** Uncore PMU / Observability
* **Focus:** Originator of the Zhou Song Uncore PMU proposal, defining standardized MMIO interfaces and discovery mechanisms for multi-chiplet systems.

### 🇮🇱 proteanTecs (Haifa, Israel)
* **Category:** Uncore PMU / Observability
* **Focus:** Hardware telemetry IP and cloud-based analytics targeting silicon health, power, and performance degradation across the entire device lifespan.

### 🇹🇼 Andes Technology (Hsinchu, Taiwan)
* **Category:** IP / Silicon
* **Focus:** Integrating commercial observability hooks directly into high-performance, vector-enabled commercial RISC-V cores via strategic ecosystem partnerships.

### 🇵🇱 Antmicro (Gdańsk, Poland)
* **Category:** Tooling / Integration
* **Focus:** Enabling practical pre-silicon performance observability through open-source tooling, verification frameworks, and advanced simulation spaces like Renode.

### 🇺🇸 SiFive (San Mateo, CA, USA)
* **Category:** IP / Silicon
* **Focus:** Setting the benchmark for RISC-V ecosystem maturity by implementing compliant performance monitoring across high-performance compute lines.

### 🇨🇳 StarFive (Shanghai, China)
* **Category:** Uncore PMU / Observability
* **Focus:** Actively deploying hardware-level event monitoring tools and platform telemetry inside shipping RISC-V SoC architectures.

### 🇺🇸 Synopsys (Sunnyvale, CA, USA)
* **Category:** Tooling / Integration
* **Focus:** Providing the essential system-level simulation, emulation, and verification stack required to analyze complex fabric and uncore interactions before tape-out.

### 🇺🇸 Qualcomm / Ventana Micro Systems (Cupertino, CA, USA)
* **Category:** IP / Silicon
* **Focus:** Enterprise data center-class vector/matrix chiplet designs paired with massive scale-out telemetry hooks.

### 🇺🇸 Akeana (San Jose, CA, USA)
* **Category:** Uncore PMU / Observability
* **Focus:** Configurable processor and fabric IP with native, in-field telemetry and reliability tracking arrays.

### 🇺🇸 Breker Verification Systems (San Jose, CA, USA)
* **Category:** Tooling / Integration
* **Focus:** Scenario-based test suite synthesis focusing on complex cache coherency validation and uncore fabric mapping.


### 🇺🇸 Tenstorrent (Austin, TX, USA / Toronto, Canada)
* **Category:** Core Hardware / AI Compute Consumers
* **Focus:** Scale-out AI processor architecture and massive RISC-V compute grids. They heavily consume uncore telemetry rather than authoring monitoring standards.

### 🇺🇸 Rivos Inc. (Mountain View, CA, USA)
* **Category:** Core Hardware / Server Silicon
* **Focus:** Ultra-high-performance, server-class RISC-V CPUs targeting data centers. Primary consumer of uncore tracking infrastructure for heavy workload profiling.

### 🇺🇸 NVIDIA (Santa Clara, CA, USA)
* **Category:** Proprietary Core Implementations
* **Focus:** Uses custom RISC-V microcontrollers embedded deeply across billions of GPUs for execution scheduling and internal telemetry, though handled via vendor-locked, proprietary paths.

### 🇺🇸 Google (Mountain View, CA, USA)
* **Category:** Operating System & Ecosystem Anchor
* **Focus:** Orchestrating Android architectural requirements and silicon target standards. They define ecosystem consumption requirements rather than creating hardware monitoring IP.

---

## 🏁 Summary
Modern performance bottlenecks are no longer contained within the core. As execution units scale, the battle for efficiency is won or lost on the fabric connecting them. RISC-V is finally making the uncore transparent—and these are the teams building that transparent future.

---

## 🤖 Connected Projects
This mapping project serves as an active data module for the **RISC-V Recruiting Agent**, an open-source, specialized AI intelligence agent designed to track talent, organizations, and architectural milestones across the global RISC-V semiconductor landscape.

👉 **Explore or contribute to the agent here:** [cve415/risc-v-recruiting-agent](https://github.com/cve415/risc-v-recruiting-agent)
