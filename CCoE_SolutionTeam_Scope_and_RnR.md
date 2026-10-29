# CCoE Team Scope and Roles & Responsibilities (Draft v0.1)

**Team:** CCoE (formerly Migration Enablement): working name to be confirmed
**Assigned by:** Head of CCoE
**Status:** First draft for discussion
**Date:** 29 October 2026

---

## 1. Purpose

With migration projects on hold, the team is repositioned to help SCBX Group design and run cloud solutions well. It does this by advising and reviewing designs across the Group, owning solution design for internal SCBX projects, and governing the SCBX cloud environment.

**Mission statement (draft):**
> Help SCBX Group build secure, resilient, and cost-effective cloud solutions by reviewing designs against Group standards, owning solution architecture for SCBX projects, and governing the SCBX cloud environment.

---

## 2. Guiding Principles

1. **Apply standards; don't author them.** EA owns Group Standards and Reference Architectures. This team applies them in reviews and designs, and feeds gaps back to EA.
2. **Design and govern; don't operate.** IT Operations runs day-to-day operations. This team owns design decisions and approval guardrails, not execution or incident handling.
3. **Advise PortCos; own SCBX.** For subsidiaries (PortCos), the team consults and reviews, and the PortCo owns its design. For internal SCBX projects, the team owns the solution design.
4. **Independence of review.** The person who designs a solution should not be its TDS reviewer.
5. **Multi-cloud ready.** Scope covers Azure today and extends to AWS and GCP as the Group multi-cloud policy takes effect.

---

## 3. Scope Overview

| # | Service | Customer | Mode | One-line description |
|---|---|---|---|---|
| 1 | **Technical Design Surgery (TDS)** | All SCBX Group companies (PortCos) | Reactive / on request, voluntary | Consult on and review cloud solution designs against Group standards and policies |
| 2 | **Solution Architecture & Ownership** | Internal SCBX projects | Proactive, embedded | Own the end-to-end cloud solution design for SCBX projects |
| 3 | **Professional Services** *(to be confirmed, see §6)* | PortCos and SCBX teams | On request, time-boxed engagement | Hands-on expert help with a defined deliverable |
| 4 | **SCBX Cloud Environment Ownership** | SCBX cloud users and project teams | Ongoing governance | Own and approve usage of the SCBX cloud environment (firewall rules, IP allocation, etc.) |

---

## 4. Boundaries (Out of Scope)

| Area | Owner | How this team interacts |
|---|---|---|
| Group Standards and Policies (authoring and maintenance) | **EA** (with Cyber and Data for their domains) | Team applies them in TDS and SA work, and raises gaps or ambiguities to EA |
| Reference Architectures | **EA** | Team uses them as the starting point for designs and reviews, and proposes new patterns based on recurring review findings |
| IT Operations (run, monitor, incident, change execution, patching, backup operation) | **IT Operations team** | Team approves designs and guardrails; IT Ops implements and operates |
| Architecture decision authority for Group | **CADRB** | TDS output (Findings, Conditions, Sign-off) feeds CADRB; CADRB decides |
| Cyber security standards and security exceptions | **Cyber / ISO** | Cyber participates in TDS; security exceptions are approved by Cyber |
| Application-layer design | **Project / application teams** | Out of scope except where it affects cloud infrastructure design |

---

## 5. Detailed Roles & Responsibilities

### 5.1 Technical Design Surgery (TDS)

**Objective:** Act as consultant and solution reviewer for SCBX Group, helping PortCos meet Group standards early, before CADRB.

**Customers:** All SCBX Group subsidiaries (PortCos). Participation is voluntary per Group Policy.

**Responsibilities:**
- Run TDS as a consult-first service: kick-off, consult, session review, output artifact.
- Review cloud solution designs against Group standards and policies, including:
  - Cloud Architecture (Cloud Usage Guideline, Cloud Usage Policy, Group Cloud Architecture Standard)
  - Security (Group Cloud Security Standard, Group Information and Cybersecurity Policy)
  - Network (Group Network Security Standard)
  - Data and AI (Group Data Security and Encryption Standard, Group AI Policy)
  - IAM (Group IAM Standard)
  - Observability / Cyber Log (Group Logging and Auditing Standard)
  - Cloud Cost (advisory)
  - **New: ITDR (IT Disaster Recovery) Standard**, once launched
  - **New: Multi-cloud Policy**, once launched
- Maintain the TDS checklist so PortCos don't need to read every standard themselves. Update it when EA releases or changes a standard.
- Join PortCo-owned forums (e.g. AWG and Infra Day at SCB Bank, ARC at INVX, DAC at CardX) instead of running a duplicate review. Offer TDS as a forum-as-a-service to PortCos without their own forum.
- Produce the TDS output artifact (Findings, Conditions, Sign-off) for CADRB.
- Feed recurring findings back to EA as input for new or revised standards and reference architectures.

**Key deliverables:** TDS checklist, review reports, TDS output artifacts, quarterly findings summary to EA and CADRB.

**Suggested KPIs:** number of reviews completed; % of CADRB submissions with a TDS artifact; median turnaround time; PortCo satisfaction; recurring-finding trends.

**Preparing for the new standards:**

| New standard / policy | What the team needs to do |
|---|---|
| ITDR Standard | Add DR checklist items (RTO/RPO classification, DR pattern per tier, DR testing evidence). Build reviewer knowledge on DR patterns per CSP. |
| Multi-cloud Policy | Add CSP-selection and workload-placement checks, and cross-cloud network, identity, and logging checks. Build reviewer capability on AWS and GCP. |

---

### 5.2 Solution Architecture & Ownership (internal SCBX projects)

**Objective:** Proactively own the cloud solution design for internal SCBX projects, from early idea to design sign-off and hand-over to IT Operations.

**Customers:** SCBX internal business and technology project teams.

**Responsibilities:**
- Engage early in SCBX projects (demand intake, project kick-off) rather than waiting to be asked.
- Act as the accountable Solution Architect: requirements analysis, solution options, design, and design decisions.
- Produce and maintain solution design documents, architecture diagrams, and architecture decision records (ADRs).
- Ensure designs comply with Group standards and use EA reference architectures where available.
- Present designs to CADRB and own the response to CADRB conditions.
- Provide design assurance during implementation (design conformance, design change control).
- Produce hand-over documentation for IT Operations (operational design, DR design, monitoring requirements).

**Key deliverables:** solution design document, architecture diagrams, ADRs, CADRB submission, operational hand-over pack.

**Suggested KPIs:** % of SCBX projects with an assigned SA at kick-off; CADRB first-pass approval rate; number of post-go-live design issues.

---

### 5.3 Professional Services (to be confirmed)

See §6 for guidance on how this differs from Solution Architecture and the recommended options.

**Proposed objective (if adopted):** Provide time-boxed, hands-on expert engagements with a defined deliverable, on request, where a requester needs capability they don't have in-house.

**Example service catalog (illustrative):**
- Cloud readiness or migration assessment
- Landing zone / subscription or account design for a new PortCo or business unit
- Proof of concept or technical spike for a new cloud service
- Cost optimization assessment
- DR readiness assessment against the new ITDR Standard
- Multi-cloud onboarding assessment against the new Multi-cloud Policy

**Responsibilities (if adopted):**
- Publish a service catalog with entry criteria, scope, and typical effort.
- Agree a statement of work for each engagement (scope, deliverable, timeline, requester accountability).
- Deliver the agreed output and hand it over. The requester keeps ownership of the outcome.

---

### 5.4 SCBX Cloud Environment Ownership

**Objective:** Act as owner of the SCBX cloud environment. Manage and approve how it is used so it stays secure, well-structured, and cost-controlled.

**Customers:** All teams and projects consuming the SCBX cloud environment.

**Responsibilities:**
- Own the SCBX cloud environment structure (management groups / organizations, subscriptions / accounts / projects, naming and tagging conventions).
- **Approve** usage requests, including:
  - Firewall rule requests
  - IP address allocation (IPAM) and network/VNet/VPC requests
  - New subscription / account / project requests
  - Cloud policy and guardrail exceptions (in consultation with Cyber for security exceptions)
  - Requests for new cloud services to be enabled
- Define and maintain guardrails (policy-as-code, allowed services and regions, baseline configuration) in line with Group standards.
- Maintain the IP address plan and network topology records.
- Review cloud cost and usage trends and raise optimization actions with resource owners.
- Periodically recertify firewall rules, access, and environment hygiene (e.g. unused resources, stale rules).

**Boundary with IT Operations:**

| Activity | CCoE team | IT Operations |
|---|---|---|
| Define environment structure and guardrails | Owns | Consulted |
| Approve firewall rule / IP / subscription requests | Approves | Informed |
| Implement approved changes | Consulted (if design questions arise) | Implements |
| Monitor, respond to incidents, patch, back up | Not involved | Owns |
| Periodic rule and access recertification | Owns | Supports with data |

**Suggested KPIs:** request approval turnaround time (SLA); % of resources compliant with guardrails; number of stale firewall rules removed; cost trend vs. budget.

---

## 6. Guidance: Professional Services vs. Solution Architecture

The confusion is understandable: both roles use the same skills. The difference is **who owns the outcome**, **how work starts**, and **how long it lasts**.

| Dimension | TDS | Solution Architecture & Ownership | Professional Services |
|---|---|---|---|
| Core question | "Is this design good enough?" | "What should we build?" | "Can you do this piece of work for us?" |
| Who owns the design / outcome | Requester (PortCo) | **This team** | Requester |
| How work starts | Requester submits a design | Team engages proactively | Requester asks for a specific engagement |
| Customer | All Group companies | Internal SCBX projects | PortCos and SCBX teams |
| Duration | Short (sessions) | Full project lifecycle | Time-boxed, defined deliverable |
| Team's role | Reviewer / advisor | Accountable designer | Hands-on expert / doer |
| Output | Findings, Conditions, Sign-off | Solution design, ADRs, CADRB submission | Agreed deliverable (assessment, design, PoC) |

### Options for Professional Services

| Option | Description | Pros | Cons |
|---|---|---|---|
| **A. Drop as a separate service** | SA covers SCBX; TDS covers PortCos. Anything else is handled case by case. | Simplest; fits current capacity | PortCos needing hands-on help have no clear route |
| **B. Fold into SA as an engagement model** | SA can also take on PortCo projects on request, with the same ownership model | One role, clear skill set | Blurs "own SCBX, advise PortCos"; risks the team owning PortCo designs |
| **C. Define as a separate, catalog-based service** *(recommended to explore)* | Small catalog of time-boxed engagements for PortCos and SCBX teams; requester owns the outcome | Clear entry point for PortCos; complements TDS; creates reusable assets | Needs capacity and intake management; possible conflict of interest with TDS |

### Recommendation

1. **Start with Option C in a limited form:** publish two or three catalog items tied directly to the new standards (e.g. DR readiness assessment, multi-cloud onboarding assessment). These help PortCos prepare for TDS without the team taking design ownership.
2. **Keep ownership clear:** in Professional Services, the requester owns the outcome. The team only "owns" designs for internal SCBX projects.
3. **Protect TDS independence:** if a team member delivered a Professional Services engagement for a PortCo, a different team member should do that PortCo's TDS review.
4. **Revisit after six months:** if demand is low or capacity is too tight, fall back to Option A.

---

## 7. High-Level RACI

R = Responsible, A = Accountable, C = Consulted, I = Informed

| Activity | CCoE team | EA | Cyber / ISO | IT Ops | PortCo / Project owner | CADRB |
|---|---|---|---|---|---|---|
| Author Group Standards and Reference Architectures | C | **A/R** | C (security) | I | I | I |
| Maintain TDS checklist | **A/R** | C | C | — | I | I |
| TDS review of PortCo design | **R** | C | R (security) | — | **A** (owns design) | I |
| TDS output artifact | **A/R** | I | C | — | C | I |
| Solution design for SCBX project | **A/R** | C | C | C | C | I |
| Architecture decision | C | C | C | — | C | **A/R** |
| Professional Services engagement | **R** | — | C | — | **A** | — |
| Define cloud environment structure and guardrails | **A/R** | C | C | C | I | — |
| Approve firewall / IP / subscription requests | **A/R** | — | C (high risk) | I | I (requester) | — |
| Implement approved changes | C | — | — | **A/R** | I | — |
| Cloud operations and incident management | — | — | C | **A/R** | I | — |
| Security exception approval | C | — | **A/R** | — | I | — |

---

## 8. Engagement Model

| Service | Entry point | Channel |
|---|---|---|
| TDS | Request via TDS mail group, or via PortCo-owned forum | CWG announcement, mail group, per-PortCo group chat with named PIC |
| Solution Architecture | Assigned at SCBX project demand intake / kick-off | Project governance process |
| Professional Services | Request from service catalog | Same mail group as TDS (single front door), separate request type |
| Cloud Environment requests | Request form / ticket (firewall, IP, subscription, exception) | Ticketing system with approval workflow and SLA |

Using a single front door for TDS and Professional Services helps PortCos who are unsure which service they need. The team triages.

---

## 9. Capacity Considerations

Current capacity is **4 staff, plus 2 allocated to other teams**. Four services is a lot for this size, so prioritization matters:

| Priority | Service | Reason |
|---|---|---|
| 1 | Cloud Environment Ownership | Operational dependency; approvals block other teams if not handled |
| 2 | TDS (including ITDR and Multi-cloud readiness) | Group-wide mandate; new standards launching |
| 3 | Solution Architecture (SCBX) | Proactive but bounded to SCBX project pipeline |
| 4 | Professional Services | Demand-driven; start small or defer |

Suggested ways to stretch capacity:
- Automate routine cloud environment approvals (e.g. pre-approved firewall patterns, IPAM tooling, policy-as-code).
- Use the TDS checklist (and optionally the AI-assisted review tool explored earlier) to reduce manual review effort.
- Consider a rotation model (e.g. one person on environment approvals each week) so approvals don't interrupt design work.

---

## 10. Open Questions for Head of CCoE

1. **Professional Services:** which option (A, B, or C in §6) should we pursue? Is chargeback to PortCos expected?
2. **Team name:** should the team be renamed to reflect the new scope (e.g. "CCoE Cloud Architecture & Governance")?
3. **ITDR and Multi-cloud timing:** when will each be launched, and will EA provide the checklist inputs or should the team draft them?
4. **Cloud environment approval authority:** does approval authority for firewall rules and IP allocation formally move to this team? Is there an existing approver to hand over from?
5. **Approval SLAs:** what turnaround is expected for cloud environment requests?
6. **SA coverage:** should every SCBX project get an SA, or only projects above a size or risk threshold?
7. **Capacity:** can the 2 shared staff be brought back, or should scope be phased to fit 4 people?

---

## 11. Suggested Next Steps

1. Review this draft with Head of CCoE and confirm the Professional Services direction.
2. Validate boundaries with EA (standards and reference architecture) and IT Operations (cloud environment approval vs. implementation).
3. Agree the RACI with Cyber, EA, IT Ops, and CADRB.
4. Define the cloud environment request process and SLAs.
5. Plan TDS checklist updates for the ITDR Standard and Multi-cloud Policy.
6. Prioritize services against current capacity and publish the team's service catalog.
