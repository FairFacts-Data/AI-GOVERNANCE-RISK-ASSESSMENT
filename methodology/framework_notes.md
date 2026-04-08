# AI Governance Risk Assessment — Framework & Methodology Notes

**FairFacts Consulting LLC**  
Author: Chiemeka Okoronkwo, Founder & Principal Consultant  
Last updated: April 2026

---

## 1. Purpose

This document describes the methodology, scoring logic, regulatory alignment, and governance principles underlying the FairFacts AI Governance Risk Assessment Template. It is intended to accompany the risk register (`ai_risk_register.csv`) and visualization notebook.

---

## 2. Scoring Methodology

### 2.1 Inherent Risk Score

Risk scores are calculated before mitigations are applied:

```
Inherent Risk Score = Likelihood (1–5) × Impact (1–5)
```

**Likelihood scale:**

| Score | Label | Description |
|---|---|---|
| 1 | Rare | May occur only in exceptional circumstances |
| 2 | Unlikely | Could occur at some time but not expected |
| 3 | Possible | Might occur at some time |
| 4 | Likely | Will probably occur in most circumstances |
| 5 | Almost Certain | Expected to occur in most circumstances |

**Impact scale:**

| Score | Label | Description |
|---|---|---|
| 1 | Negligible | Minimal disruption; no regulatory exposure |
| 2 | Minor | Limited impact; manageable with standard controls |
| 3 | Moderate | Noticeable harm; some regulatory or reputational exposure |
| 4 | Major | Significant harm; regulatory findings or litigation risk |
| 5 | Severe | Catastrophic harm; enforcement action, major data breach, or loss of public trust |

**Risk level thresholds:**

| Score | Level | Response Priority |
|---|---|---|
| 15–25 | 🔴 Critical | Immediate action required; executive escalation |
| 8–12 | 🟠 High | Priority mitigation; assigned owner with deadline |
| 4–6 | 🟡 Medium | Monitor and mitigate within standard cycle |
| 1–3 | 🟢 Low | Accept or monitor; review annually |

---

### 2.2 Residual Risk Score

Residual risk reflects the risk remaining after mitigations are applied. An adjustment factor is applied based on mitigation status:

| Status | Adjustment Factor | Meaning |
|---|---|---|
| Mitigated | × 0.4 | Controls in place and verified; 60% risk reduction |
| In Progress | × 0.7 | Controls partially implemented; 30% risk reduction |
| Planned | × 1.0 | No reduction yet — mitigation not yet implemented |

```
Residual Score = Inherent Risk Score × Adjustment Factor
```

Adjustment factors should be revisited based on control testing results. A "Mitigated" status should only be assigned when controls have been tested, not merely documented.

---

## 3. Risk Domains

| Domain | Scope |
|---|---|
| AI Model & Algorithm | Hallucination, bias, drift, explainability, adversarial inputs, model versioning |
| Data Privacy & Governance | PII exposure, data subject rights, consent, cross-border data transfers, data minimization |
| Regulatory & Compliance | EU AI Act classification, audit readiness, shadow AI, board accountability |
| Operational & Vendor | Third-party API dependencies, open-source model supply chain, system availability |
| Ethical & Reputational | Discriminatory outputs, fairness testing, stakeholder trust, incident response |

---

## 4. Regulatory Alignment

### 4.1 NIST AI Risk Management Framework (AI RMF 1.0)

The four core functions of the NIST AI RMF are mapped throughout this register:

- **Govern** — accountability structures, policies, review cadence (R-09, R-18)
- **Map** — AI inventory, use case classification, stakeholder impact (R-10, R-02, R-15)
- **Measure** — bias audits, drift monitoring, explainability metrics (R-02, R-03, R-04)
- **Manage** — mitigation actions, incident response, vendor management (R-05, R-12, R-16)

### 4.2 ISO/IEC 42001:2023

This standard establishes requirements for an AI management system (AIMS). Key clauses referenced:

- **Clause 5** — Leadership and accountability (R-18)
- **Clause 7.3** — AI awareness and competence (R-09)
- **Clause 8.4** — AI supply chain controls (R-12, R-13)
- **Clause 9** — Performance evaluation and monitoring (R-03, R-11)

### 4.3 EU AI Act (2024)

The EU AI Act introduces binding obligations for high-risk AI systems. Key articles referenced:

- **Article 4** — AI literacy requirements (R-09)
- **Article 10** — Data governance requirements (R-06, R-15)
- **Article 12** — Record-keeping and logging (R-11)
- **Article 13** — Transparency and explainability (R-04)
- **Title III** — High-risk AI system classification (R-10)
- **Article 73** — Incident reporting obligations (R-16)

### 4.4 GDPR / CCPA

- **GDPR Articles 15–22** — Data subject rights (R-07)
- **GDPR Articles 25 & 32** — Privacy by design and security (R-06)
- **GDPR Chapter V** — Cross-border data transfers (R-08)
- **CCPA §1798.100–120** — Consumer rights and opt-out (R-07, R-17)

---

## 5. Review Cadence & Governance

### 5.1 Scheduled reviews

| Trigger | Review Type |
|---|---|
| Quarterly | Standing risk register review with all domain owners |
| New AI system deployment | Full risk re-assessment before go-live |
| Regulatory change | Targeted review of affected risk items |
| Post-incident | Root cause analysis + register update within 30 days |
| Annual | Full framework review including scoring thresholds |

### 5.2 Ownership model

Each risk has a designated owner responsible for:
- Implementing and maintaining mitigation controls
- Reporting status at quarterly reviews
- Escalating to Governance Lead or Exec Sponsor when risk level increases

### 5.3 Escalation thresholds

| Scenario | Escalation |
|---|---|
| Any Critical risk without mitigation in progress | Immediate exec escalation |
| Residual score increases from prior quarter | Governance Lead review within 2 weeks |
| Regulatory deadline within 60 days | Legal + Exec briefing |

---

## 6. Assumptions & Limitations

- Likelihood and impact scores reflect the assessor's professional judgment at time of review and should be validated with domain subject matter experts.
- Adjustment factors for residual risk are estimates. Organizations should conduct control testing to validate actual risk reduction.
- This template is designed as a starting framework. It should be adapted to the specific AI systems, business context, and regulatory obligations of each organization.
- This register does not constitute legal advice. Organizations should engage qualified legal counsel for regulatory compliance matters.

---

## 7. About FairFacts Consulting

FairFacts Consulting LLC helps organizations build responsible, trustworthy AI systems through expert consulting in AI governance, data privacy, program management, and digital strategy.

**Contact:** info@fairfactsconsulting.com  
**Website:** [fairfactsconsulting.com](https://www.fairfactsconsulting.com)  
**LinkedIn:** [linkedin.com/in/chiemeka-okoronkwo](https://www.linkedin.com/in/chiemeka-okoronkwo)

---

*© 2026 FairFacts Consulting LLC. All rights reserved.*
