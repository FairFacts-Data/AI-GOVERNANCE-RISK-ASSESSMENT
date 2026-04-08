# AI Governance Risk Assessment Template

**FairFacts Consulting LLC** | Privacy, AI Governance & Data Compliance  
*Chiemeka Okoronkwo — Founder & Principal Consultant*  
[fairfactsconsulting.com](https://www.fairfactsconsulting.com) · [LinkedIn](https://www.linkedin.com/in/chiemeka-okoronkwo) · [GitHub](https://github.com/fairfacts-data)

---

## Overview

This repository contains a reusable AI governance risk assessment framework designed for organizations deploying or evaluating AI systems. It is part of the FairFacts Consulting public portfolio, demonstrating applied skills in AI risk management, responsible AI governance, and regulatory compliance consulting.

The template covers **18 risk scenarios** across five governance domains, scored using a 5×5 likelihood-impact matrix. It is aligned to leading standards and regulations including NIST AI RMF, ISO/IEC 42001, the EU AI Act, GDPR, and CCPA.

---

## Repository Structure

```
AI-GOVERNANCE-RISK-ASSESSMENT/
│
├── README.md                          ← This file
├── ai_risk_register.csv               ← Full risk register (18 risks, scored & mitigated)
├── ai_risk_matrix_visualization.ipynb ← Python notebook: heat map + charts
└── methodology/
    └── framework_notes.md             ← Scoring methodology & regulatory alignment notes
```

---

## Risk Domains Covered

| Domain | Description |
|---|---|
| AI Model & Algorithm | Hallucination, bias, drift, explainability, adversarial inputs |
| Data Privacy & Governance | PII exposure, data subject rights, consent, cross-border transfers |
| Regulatory & Compliance | EU AI Act classification, audit readiness, shadow AI governance |
| Operational & Vendor | Third-party API risk, open-source model supply chain, system reliability |
| Ethical & Reputational | Discriminatory outputs, fairness testing, incident response |

---

## Scoring Methodology

Risk scores are calculated as:

```
Risk Score = Likelihood (1–5) × Impact (1–5)
```

| Score Range | Risk Level |
|---|---|
| 15–25 | 🔴 Critical |
| 8–12 | 🟠 High |
| 4–6 | 🟡 Medium |
| 1–3 | 🟢 Low |

**Residual risk** is calculated post-mitigation using an adjustment factor:
- Mitigated: ×0.4
- In progress: ×0.7
- Planned: ×1.0 (no reduction yet applied)

---

## Regulatory Alignment

This framework maps to the following standards and regulations:

- **NIST AI RMF 1.0** — Govern, Map, Measure, Manage core functions
- **ISO/IEC 42001:2023** — AI management system standard
- **EU AI Act (2024)** — High-risk AI system classification and conformity requirements
- **GDPR / CCPA** — Privacy-by-design, data subject rights, consent management
- **PMI Trustworthy AI Framework** — Accountability and transparency practices

---

## Risk Summary (Current Assessment)

- **Total risks identified:** 18  
- **Critical / High:** 5  
- **Mitigated or in progress:** 9  
- **Residual risk score:** 42 / 100  

---

## How to Use This Template

1. **Clone or download** this repository.
2. Open `ai_risk_register.csv` and adapt the risk items to your organization's AI systems and use cases.
3. Update likelihood and impact scores based on your internal context.
4. Assign owners from your team (e.g., Privacy, Legal, Engineering, Governance).
5. Run `ai_risk_matrix_visualization.ipynb` to regenerate the heat map and summary charts.
6. Review quarterly or upon any material change to AI systems, data flows, or regulatory requirements.

---

## Review Cadence

Risk registers should be reviewed:
- **Quarterly** as a standing governance cadence
- **Upon deployment** of any new AI system or model version
- **Upon regulatory change** (e.g., new guidance from EU AI Office, FTC, state privacy laws)
- **Following an incident** involving AI outputs, data exposure, or compliance finding

---

## About FairFacts Consulting

FairFacts Consulting LLC is a Bay Area-based consulting firm specializing in AI governance, data privacy, responsible AI practices, and program management. The firm serves organizations that are committed to building trustworthy, compliant, and ethically grounded AI systems.

**Services include:**
- AI & Data Governance program design
- Privacy Impact Assessments (DPIA/PIA)
- LLM evaluation, testing, and quality assessment
- Digital strategy & transformation
- Speaking, workshops, and executive coaching

> *"Responsible AI and privacy-forward design are not constraints — they are competitive advantages that build durable customer trust at scale."*  
> — Chiemeka Okoronkwo

**Contact:** [info@fairfactsconsulting.com](mailto:info@fairfactsconsulting.com)  
**Book a consultation:** [fairfactsconsulting.com](https://www.fairfactsconsulting.com)

---

*FairFacts Consulting LLC maintains professional liability and cyber insurance and adheres to strict confidentiality standards when working with client data.*

© 2026 FairFacts Consulting LLC. All rights reserved.
