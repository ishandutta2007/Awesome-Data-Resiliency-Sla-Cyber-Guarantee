# Awesome-Data-Resiliency-Sla-Cyber-Guarantee

## Top Data Resiliency SLA & Cyber Guarantee Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Financially-Backed SLAs, Ransomware Warranties & Recovery Guarantees*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Data Resiliency SLA & Cyber Guarantee**. These offerings provide financially-backed commitments from vendors—covering data immutability, recoverability, availability, and ransomware recovery—giving organizations contractual leverage and potential reimbursement if recovery fails.

**Examples** include Druva Data Resiliency Guarantee, Rubrik Ransomware Recovery Warranty, Veeam Ransomware Warranty, Cohesity Ransomware Guarantee, Acronis Anti-Ransomware Warranty, Sophos Breach Protection Warranty, and SentinelOne Ransomware Warranty (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted SLA monitoring, open-source recovery drill automation, and community-driven resilience verification—ideal for organizations seeking to *prove* recoverability rather than rely on vendor promises. Note that **financially-backed guarantees are inherently commercial constructs**—no open-source project offers a warranty. The open-source path focuses on verification: automated drills, canary testing, and evidence generation that demonstrates your recovery actually works.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Druva Data Resiliency Guarantee](https://www.druva.com/products/resiliency-guarantee)** | **The most comprehensive financially-backed guarantee in the category: up to $10M coverage across five risk categories** (Cyber, Human, Application, Operational, Environmental). Backed by five SLAs: **100% Confidentiality**, **100% Immutability** (last successful backup recoverable after ransomware), **99% Reliability**, **99.999% Durability**, and **99.5% Availability**. Available at **no additional charge** for qualifying customers who purchase the Security Posture & Observability license, meet annual spend minimums, contract length, and pass a Health Check. Payout tiers scale from $100K (for $25K–$49K annual spend) to $10M (for $1M+ spend) . | **Included at no extra charge** with qualifying Druva subscription (requires Security Posture & Observability license + spend minimum)  | No standalone free tier; guarantee bundled with Druva subscription |
| **[Rubrik Ransomware Recovery Warranty](https://www.rubrik.com/warranty)** | **Up to $10M in coverage** for Rubrik Enterprise Edition and Rubrik Cloud Vault customers. Covers recovery costs if Rubrik cannot restore protected data after a ransomware incident. Requires: working with a Customer Experience Manager (CEM), passing health checks (initial, monthly, and upon incident), enabling Radar/Sonar, implementing MFA, retention lock, and notifying Rubrik within **12 hours** of discovery. Reimbursement request must be submitted within **1 year** of confirmed Recovery Incident . | Included with Rubrik Enterprise Edition (quote-only) | No free tier; warranty bundled with Enterprise Edition subscription |
| **[Veeam Ransomware Recovery Warranty](https://www.veeam.com/legal/ransomware-warranty-agreement.html)** | **Up to $5M in recovery coverage** for verified ransomware incidents on Veeam Data Platform (Advanced and Premium editions) and Veeam Kasten. Requires: current TAM services, passing quarterly security assessments, running latest software version, and notifying Veeam within **12 hours** of discovery. Reimbursement request must be submitted within **6 months** of confirmed Recovery Incident . | Included with Veeam Data Platform Advanced/Premium (quote-only) | No free tier; warranty bundled with eligible subscriptions |
| **[Cohesity Ransomware Guarantee](https://www.cohesity.com/)** | **Industry-unique "200% payout" offer**: Cohesity will match any competitor's published warranty and **double the dollar cap**. Requires equivalent terms adapted to Cohesity products. Notably, Cohesity itself publicly states that "these warranties are intentionally designed to never pay out" and lists **11 common ways vendors avoid payment**—including preexisting conditions, non-compliance with every recommendation, late notification, and customer-introduced malware. The 200% offer is essentially a competitive statement rather than a standard program . | Quote-only (match competitor terms + double cap) | No free tier; competitive offer via sales |
| **[Acronis Anti-Ransomware Warranty](https://care.acronis.com/s/article/Acronis-Cyber-Protect-Anti-ransomware-warranty)** | **Up to $1M or 12 months of fees** (whichever is less) for eligible recovery costs. Covers **endpoints only** (disk, volume, file backups) stored in **Acronis-hosted cloud storage**. Requires: 2FA enabled, immutable storage in Compliance mode, and backup validation via checksum, screenshot, or heartbeat. Enabled by default for qualifying customers . | Included with Acronis Cyber Protect Cloud (qualifying configurations) | No free tier; warranty bundled with eligible subscriptions |
| **[Sophos Breach Protection Warranty](https://www.sophos.com/en-us/legal/mdr-warranty)** | **Up to $1M in response expenses** for Sophos MDR Complete customers at **no additional cost**. Covers up to **$1,000 per affected endpoint**, up to **$100,000 for ransom payments** (as part of per-device limit), plus breach notification, PR, legal, and compliance expenses. No warranty tiers, no minimum contract term, no additional purchase requirements. Excludes VDI environments, SAN/NAS storage, and incidents caused by customer negligence . | **Included at no extra charge** with Sophos MDR Complete subscription  | No free tier; warranty bundled with MDR Complete |
| **[SentinelOne Ransomware Warranty](https://www.sentinelone.com/legal/ransomware-warranty/)** | Warranty for SentinelOne Control or Complete SKU customers. Requires extensive configuration: Protection Mode set to Protect, all detection engines ON, Anti-Tamper ON, Snapshots ON, latest GA agent version, 2FA on Management Console, VSS enabled with 10% disk allocation, and **notification within 24 hours** of discovery. Customer must blacklist the threat within 1 hour and take remediation/rollback action within 1 hour . | Quote-only (bundled with eligible SKU) | No free tier; warranty requires specific SKU and configuration |
| **[CrowdStrike Falcon Complete Limited Warranty](https://www.crowdstrike.com/)** | Limited warranty for Falcon Complete MDR customers. Explicitly **not a contract of insurance**; void in jurisdictions where deemed insurance. Liability capped at Customer's cap as set forth in the agreement. CrowdStrike reserves the right to modify warranty terms at any time with notice . | Quote-only (bundled with Falcon Complete) | No free tier; warranty bundled with Falcon Complete subscription |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[FireDrill](https://github.com/kirilurbonas/FireDrill)** | [![Stars](https://img.shields.io/github/stars/kirilurbonas/FireDrill?style=social&color=white)](https://github.com/kirilurbonas/FireDrill/stargazers) | **The most complete open-source recovery drill and SLA evidence platform.** Automated disaster recovery drills that **prove** backups actually restore. Features: **ransomware canary** (plant a sentinel value in production, prove every drill restores it byte-exact—catches encrypted-at-source or silently corrupted backups that row counts miss); **RTO/RPO measurement** per drill with trend history; **compliance-control export** (drills declare controls they evidence, `firedrill controls` aggregates into auditor-ready matrix with ISO27001-A.8.13, SOC2-A1.2 mappings); **Kubernetes operator** for scheduled drills via CRD; **Velero integration** for namespace-level restore verification. Go binary, Apache 2.0 . |
| **[Pulse](https://github.com/Erchoc/pulse)** | [![Stars](https://img.shields.io/github/stars/Erchoc/pulse?style=social&color=white)](https://github.com/Erchoc/pulse/stargazers) | **Lightweight self-hosted SLA monitoring platform with global probes.** Multi-protocol monitoring (HTTP, TCP, WebSocket, DNS, ICMP, heartbeat) with probes deployable across CN, HK, SEA, EU, US regions. **Real-time SLA dashboard** with availability %, latency percentiles (p50/p95/p99), incident timeline, and **service-level SLA targets** with configurable reporting windows (7D–365D). Maintenance windows exclude planned downtime from SLA calculations. Webhook alerts to Slack, DingTalk, Feishu. Single Go binary, Apache 2.0 . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[PulseOps](https://www.npmjs.com/package/pulseops)** | — | CLI companion to Pulse (or similar SLA monitoring backends). Provides **30-day SLA summaries**, uptime/latency percentiles (all-time, 24h, 30d), incident history, and heartbeat sending. Useful for teams wanting terminal-based SLA reporting without a full dashboard . |

**Frameworks for building custom systems**: The open-source path to **verifiable** resilience (not legal guarantees) is **prove it works**. Use **FireDrill** for automated recovery drills with ransomware canaries and compliance-control evidence export—this is what auditors actually want to see, not vendor warranty documents. Use **Pulse** for continuous SLA monitoring of your own services with configurable targets and incident tracking. **No open-source project offers a financially-backed warranty**; the open-source advantage is transparency and proof, not reimbursement.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cyber warranties are **contractual instruments**, not insurance. They contain extensive eligibility requirements, exclusions, and notification deadlines that can void coverage. **Cohesity itself publicly states that these warranties are "intentionally designed to never pay out"** and lists 11 common vendor escape clauses . Do not treat a warranty as a substitute for a working backup and recovery program.
- **Key distinctions across offerings**: Druva offers the broadest coverage (5 risk categories, $10M) and is **free with qualifying subscription** . Rubrik covers up to $10M but requires Enterprise Edition and CEM engagement . Veeam covers up to $5M with quarterly assessments . Acronis caps at **$1M or 12 months of fees** and covers **endpoints only** . Sophos offers **$1M with no extra cost** for MDR Complete customers . SentinelOne and CrowdStrike have extensive configuration requirements and notification windows (24h and 12h respectively). **Open-source tools like FireDrill provide the evidence** that your recovery actually works—which is what auditors and insurers care about more than any vendor warranty document.

---

**Made for SREs, backup administrators, compliance officers, and organizations building verifiable cyber resilience.**  
Let's make data resiliency SLAs and guarantees more transparent, measurable, and provable.
