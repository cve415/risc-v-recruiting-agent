performance-monitoring-riscv.MD

# Performance Monitoring and Observability in RISC-V

Eight companies across five countries shaping the RISC-V observability stack

* **Alibaba (Hangzhou, China)** — Strongest signal for the Uncore PMU conversation; Zhou Song's proposal (defining MMIO interfaces and discovery mechanisms for multi-chiplet SoCs) originates here. Alibaba ranks among the top RISC-V tech companies globally.
* **Andes Technology (Hsinchu, Taiwan)** — Major RISC-V IP supplier; already partnered with proteanTecs to integrate on-chip health and performance monitoring into the AndesCore™ AX45MPV and other high-performance cores.
* **proteanTecs (Haifa, Israel)** — The clearest "observability" play; hardware IP monitoring and analytics explicitly focused on visibility, power, performance, and reliability across the device lifecycle using deep data analytics.
* **Antmicro (Gdańsk, Poland)** — Deep in open hardware/software integration and RISC-V ecosystem tooling; their Renode simulator and "Trace-Based Model" (TBM) make pre-silicon performance observability practical.
* **SiFive (San Mateo, CA, USA)** — The most recognized RISC-V processor IP brand and a benchmark for ecosystem maturity, driving standard-compliant performance monitoring across their Essential, Performance, and Intelligence lines.
* **StarFive (Shanghai, China)** — Already shipped RISC-V performance tooling for hardware event monitoring (e.g., in the JH-7110 and JH-B100 BMC chips), mapping directly to the observability theme in data centers.
* **Synopsys (Sunnyvale, CA, USA)** — Their verification and system-level tooling (like ZeBu and Platform Architect) are part of the "make RISC-V production-ready" stack, moving observability from simple core-tracing to complex uncore analysis.

---

RISC-V's new Uncore PMU proposal (shoutout to Zhou Song and the team at Alibaba, Hangzhou, China) tackles exactly this blind spot. It standardizes performance monitoring for last-level cache, memory controllers, coherent interconnects, and I/O subsystems—the places where modern AI, HPC, and data center workloads actually live or die.
Why this matters for three different audiences:
🔧 For developers: You'll get the same uncore visibility Intel and ARM engineers already take for granted. No more assuming 40% CPU utilization means headroom, when your memory bandwidth is actually maxed out and your LLC is thrashing. The fix shifts from "tune the scheduler" to "fix the data layout"—but only if you can see it.
🐧 For open-source advocates: This isn't a vendor-specific hook. It's a shared standard integrated with Linux perf and existing tooling, meaning RISC-V implementations won't fragment into proprietary monitoring silos. Ecosystem cohesion beats ecosystem lock-in.
📈 For business/GTM: This is infrastructure-level table stakes for cloud and HPC adoption. Customers evaluating RISC-V against x86 or ARM will ask: "Can your platform debug the bottlenecks that actually matter?" 
