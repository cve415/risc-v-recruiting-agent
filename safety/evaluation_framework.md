# Safety, Ethics & Compliance Framework

This AI Agent is governed by a strict **Safety-First** architecture. Recruitment is a high-stakes domain; therefore, this project prioritizes data integrity and platform compliance over total autonomy.

---

## 1. Anti-Hallucination Architecture
To eliminate "AI hallucinations" (invented skills or experiences), the agent operates under a **Zero-Inference Policy**:

* **Source Attribution:** Every candidate claim or qualification must cite a specific section of the source document (LinkedIn profile or Resume).
* **Confidence Thresholds:** All generated summaries undergo a secondary verification. Any output with a confidence score below **85%** is automatically quarantined for human review.
* **Factual Freeze:** Dates, company names, and job titles are treated as immutable. The agent is prohibited from "guessing" missing employment dates.

## 2. Platform Compliance (LinkedIn TOS)
This agent is engineered to protect your LinkedIn account longevity by respecting [LinkedIn’s User Agreement](https://www.linkedin.com/legal/user-agreement).

* **Subscription Tier Awareness:** The system adjusts activity (search depth and InMail volume) based on your specific tier (Basic, Premium, or Recruiter).
* **Anti-Scraping Safeguards:** We prioritize official integration pathways. The agent does not utilize prohibited browser automation (e.g., Selenium/Playwright) to bypass LinkedIn's technical measures.
* **Human-in-the-Loop (HITL):** All external actions (sending messages, connection requests) require a final human approval.

## 3. Ethics & Bias Mitigation
* **Protected Characteristics:** The agent is programmatically restricted from inferring or filtering candidates based on age, gender, ethnicity, or disability status.
* **Non-Automated Decisions:** This tool is a **Decision Support System**, not an Automated Decision-Making system. Final candidate selection is always performed by a human recruiter.

## 4. Security & Data Privacy
| Component | Protocol |
| :--- | :--- |
| **Data Encryption** | AES-256 for PII at rest; TLS 1.3 in transit |
| **Session Management** | Secure vaulting for tokens (No credentials in logs) |
| **Retention** | 90-day rolling purge for non-essential analysis logs |
| **Audit Trail** | Append-only logging of all agent-driven queries |

---

## 5. Failure Modes & Escalation
If the agent encounters data ambiguity or a potential TOS "Gray Area," it is trained to:
1.  **Halt** current execution.
2.  **Log** the discrepancy.
3.  **Alert** the human operator via the status channel.

Transparency Note: This framework is a subset of our internal Recruiting Agent Evaluation Framework. For the full technical specification and red-teaming protocols, please refer to our Standard Project Page.

-
