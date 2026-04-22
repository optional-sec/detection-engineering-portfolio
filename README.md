# optional-sec | Detection Engineering Portfolio

> *"Don't just respond to threats. Build the systems that find them first."*

---

## Who I Am

I'm **Samuel Ramon**, a Detection Engineer and SOC Analyst based in Santo Domingo, Dominican Republic. My career started in the trenches of a large MSSP — managing security operations across dozens of client environments simultaneously, handling everything from Tier 1 triage to full incident response under constant operational pressure. That foundation taught me how attacks actually unfold in the real world, not just in theory.

From there I moved into detection engineering, where the focus shifted from reacting to threats to building the logic that catches them before they escalate. Today I work across the full detection lifecycle — from raw log ingestion and parsing to rule design, gap analysis, and continuous tuning.

I hold a **CompTIA CySA+** certification and I'm currently deepening my expertise in YARA, Sigma, and Detection-as-Code practices.

- 📍 Santo Domingo, Dominican Republic
- 💼 SOC Analyst II & Detection Engineer @ Boomi
- 🎯 4+ years in Security Operations, Incident Response, and Detection Engineering
- 🏆 CompTIA CySA+

---

## Detection Philosophy

Detection engineering is not about writing rules — it's about understanding adversary behavior deeply enough to predict it.

My approach:

**1. Hypothesis first.** Every detection starts with a question: what would this attack look like in my logs? I map to MITRE ATT&CK before I write a single line of query logic.

**2. Data before detection.** A rule is only as good as the data behind it. Log source onboarding, normalization, parsing, and field extraction are not overhead — they are the foundation.

**3. Fidelity over volume.** One high-fidelity alert that fires accurately is worth more than fifty noisy rules that analysts learn to ignore. I optimize for signal, not coverage theater.

**4. Detection is never done.** Threats evolve. Rules decay. Weekly gap assessments, tuning case reports, and continuous validation are not optional — they are the job.

**5. Code-driven lifecycle.** Detections are code. They belong in version control, they need documentation, and they should be managed with the same discipline as any production system.

---

## Repository Structure

```
detection-engineering-portfolio/
│
├── sigma-rules/
│   ├── windows/          # Windows endpoint detections
│   ├── linux/            # Linux endpoint detections
│   └── cloud/            # AWS, Azure, GCP detections
│
├── yara-rules/
│   ├── malware-families/ # Rules targeting specific malware
│   └── techniques/       # Rules targeting ATT&CK techniques
│
├── sumo-logic/
│   ├── queries/          # Threat hunting and detection queries
│   └── parsers/          # Log source parsing logic
│
├── mitre-coverage/
│   ├── coverage-map.json # ATT&CK Navigator layer
│   └── gap-analysis.md   # Coverage gaps and remediation plan
│
├── detection-as-code/
│   ├── templates/        # Rule templates and standards
│   └── lifecycle-docs/   # Detection lifecycle documentation
│
└── docs/
    ├── detection-methodology.md  # End-to-end detection process
    └── tuning-case-template.md   # Tuning case report template
```

---

## Rule Standards

Every rule in this repository follows these standards:

**Sigma rules must have:**
- Title, status, description
- Correct logsource mapping
- MITRE ATT&CK tags (`attack.tXXXX`)
- False positive documentation
- Author, date, and reference

**YARA rules must have:**
- Meta block with author, date, description, MITRE technique, and reference
- Comments explaining non-obvious logic
- Tested against real samples or simulated activity

**No rule ships without:**
- A documented false positive rate
- A mapped MITRE technique
- Validation evidence

---

## Tools & Platforms

| Category | Tools |
|----------|-------|
| **SIEM / Detection** | Sumo Logic, Splunk, Elastic (ELK) Stack, Microsoft Sentinel, Azure Sentinel |
| **EDR / XDR** | CrowdStrike Falcon, SentinelOne, Carbon Black, Cylance Protect, Trend Micro Vision One, Microsoft Defender |
| **SOAR / Ticketing** | Palo Alto Cortex XSOAR, FortiSOAR, Torq.io, Splunk SIR, ServiceNow, OpsGenie, PagerDuty, Jira |
| **Email Security** | ProofPoint, PhishER (KnowBe4) |
| **Security Tools** | TruffleHog, Portal26, Astrix, Akamai Control Center, MDR Booli, Halo, Cisco AMP, Cisco ASA (Basic) |
| **Identity** | Azure AD, Entra ID |
| **Detection Languages** | Sigma, YARA, REGEX, Sumo Logic Query Language |
| **Scripting** | Python, PowerShell, Bash |
| **Collaboration** | Slack, Jira |
| **Frameworks** | MITRE ATT&CK, PICERL, Detection-as-Code |

---

## Connect

- 🔗 [LinkedIn](https://linkedin.com/in/samuel-ramon)
- 📧 samuelvalenzueela.04@gmail.com
- 🎮 CTF Player | Wargames Enthusiast | Chess

---

*This portfolio is continuously updated. All detections are built from real-world experience and validated against simulated or historical activity. No client or employer data is included.*
