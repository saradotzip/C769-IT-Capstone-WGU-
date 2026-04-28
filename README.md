
# C769 – IT Capstone (WGU)

**Student:** Sara E. Goodie  
**Course:** C769 – IT Capstone  
**Program:** Western Governors University  
**Project Title:** Implementation of a Security Information and Event Management (SIEM) Solution for a Mid-Sized Retail Business

---

## Repository Contents

| File | Description |
|------|-------------|
| `IT_Capstone_Proposal_SaraGoodie_task2.pdf` | **Task 2** – IT Capstone Proposal (problem, solution, methodology, goals, timeline) |
| `Post-Implementation_Report_Sg_task3.pdf` | **Task 3** – Post-Implementation Report (results, scope creep, project success metrics) |

---

## Project Overview

### The Problem
A mid-sized retail business (~200 employees, physical + online sales) experienced a phishing incident that compromised an employee account. Investigation revealed the root cause: logs from firewalls, servers, endpoints, authentication systems, POS terminals, and cloud services were all stored and reviewed in complete isolation. Early warning signs — repeated failed authentication attempts, suspicious IP geolocations, and privilege escalations — went undetected because no centralized monitoring existed.

### The Solution
Implement **Microsoft Sentinel** (cloud-native SIEM) as the primary security monitoring platform. Sentinel centralizes all log sources into a single Log Analytics workspace, applies normalization schemas (ASIM models), and uses analytics rules to automatically detect and alert on threats in real time.

---

## Task 2 – IT Capstone Proposal

### Proposal Structure

| Section | Summary |
|---------|---------|
| **Problem Summary** | Phishing incident exposed fragmented, siloed log management with no centralized visibility or automated alerting |
| **IT Solution** | Microsoft Sentinel SIEM: unified log ingestion, real-time analytics rules, Workbook dashboards, automated response playbooks via Azure Logic Apps |
| **Implementation Plan** | 7-phase structured plan (Planning → Test Deployment → Log Integration → Config/Use-Case Dev → Testing → Training → Production Rollout) |
| **Project Rationale** | PCI-DSS compliance requirements, business growth scaling, customer trust, financial risk reduction |
| **Current Environment** | Mixed on-prem/cloud; Microsoft 365, POS terminals, Windows servers, firewalls; all operating in silos with no correlation layer |
| **Methodology** | Agile (5 sprints); iterative refinement of alert rules, dashboards, and log integrations |
| **Goals & Objectives** | 3 goals, 5 supporting objectives, 6 deliverables |
| **Project Timeline** | December 1–30, 2025 (30 days total) |
| **Outcomes** | Centralized log collection, accurate threat detection, staff SIEM proficiency |

### 7-Phase Implementation Plan

| Phase | Owner | Key Actions |
|-------|-------|-------------|
| 1. Planning | IT Director & Security Lead | Define scope, select SIEM platform, identify log sources, set retention policy per PCI-DSS |
| 2. Test Deployment | System Administrators | Deploy Sentinel in sandbox; configure Log Analytics workspace, ingestion pipelines, access roles |
| 3. Log Source Integration | Security Engineers | Connect AD, M365, POS, firewalls, endpoints, cloud apps; monitor ingestion health |
| 4. Config & Use-Case Dev | Security Team | Build analytics rules (phishing, credential abuse, lateral movement), dashboards, automated playbooks |
| 5. Testing & Validation | IT & Security Teams | Controlled simulations; validate alert accuracy; document and tune false positives |
| 6. Training | Security Lead & HR | Workshops on dashboard navigation, alert triage, incident response playbooks |
| 7. Production Rollout | All IT Teams | Switch to live environment; begin continuous monitoring; monthly reviews |

### Agile Sprint Breakdown

| Sprint | Focus |
|--------|-------|
| Sprint 1 | Deployment and Initial Configuration |
| Sprint 2 | Log Source Integration and Normalization |
| Sprint 3 | Alert Creation, Dashboard Development, Use-Case Testing |
| Sprint 4 | Training, Documentation, Incident Workflow Development |
| Sprint 5 | Production Rollout and Continuous Improvement |

### Project Goals, Objectives & Deliverables

| Goal | Objectives | Deliverables |
|------|-----------|-------------|
| **1. Centralize Security Monitoring** | Connect all log sources; normalize and correlate data | Fully deployed SIEM with configured connectors; functional SIEM with normalized logs and correlation logic |
| **2. Improve Threat Detection & Incident Response** | Develop detection rules and dashboards; validate via simulated attacks | Customized dashboards and alert rules; test report from simulated attacks |
| **3. Prepare IT Staff** | Structured training; workshops and staff evaluation | User guides, training materials, incident response playbooks; staff evaluation records and workshop completion |

### Proposed Project Timeline

| Milestone | Duration | Start | End |
|-----------|----------|-------|-----|
| Install SIEM in test environment | 3 days | Dec 1, 2025 | Dec 3, 2025 |
| Collect log sources | 5 days | Dec 4, 2025 | Dec 9, 2025 |
| Configure dashboards and alerts | 7 days | Dec 10, 2025 | Dec 17, 2025 |
| Testing and feedback | 4 days | Dec 18, 2025 | Dec 21, 2025 |
| Staff training | 3 days | Dec 22, 2025 | Dec 24, 2025 |
| Production rollout | 5 days | Dec 25, 2025 | Dec 30, 2025 |

### Literature Review (4 Works)

| Source | Key Contribution |
|--------|----------------|
| **NIST SP 800-137** (2011) | Federal standard for Information Security Continuous Monitoring (ISCM); automated correlation, log standardization, and enterprise visibility are core SIEM requirements |
| **Verizon DBIR** (2023) | Phishing and credential theft are top breach vectors; SIEM enables faster automated detection; organizations slow to detect face disproportionate financial damage |
| **IBM Cost of a Data Breach Report** (2023) | Organizations using SIEM/SOAR reduce breach costs by ~30%; measured via Mean Time to Detect (MTTD) and Mean Time to Contain (MTTC) |
| **Splunk Security Analytics Whitepaper** (2022) | SIEM correlation rules detect multi-step attacks; machine learning anomaly detection; customizable dashboards and automated response capabilities |

---

## Task 3 – Post-Implementation Report

### Project Outcome: Complete Success ✅

All three goals were met. All prioritized log sources were centralized in Sentinel, analytics rules successfully detected threats during simulated testing, dashboards provided real-time visibility, and IT staff demonstrated proficiency operating the platform.

### Agile Sprint Execution Results

| Sprint | Deliverables | Result |
|--------|-------------|--------|
| **Sprint 1** – Deployment & Initial Config | SIEM workspace deployed; ingestion pipelines active; agents deployed | ✅ On time |
| **Sprint 2** – Log Source Integration | All 6 log source categories onboarded; ASIM normalization applied | ✅ On time |
| **Sprint 3** – Alerts, Dashboards, Use-Case Testing | Detection rules built; dashboards configured; simulated attack testing conducted | ✅ 1 day early |
| **Sprint 4** – Training & Documentation | Workshops held; user guides and playbooks delivered to staff | ✅ On time |
| **Sprint 5** – Production Rollout | Live monitoring activated; continuous improvement ongoing | ✅ 1 day early |

### Actual vs. Planned Timeline

| Milestone | Planned | Actual | Status |
|-----------|---------|--------|--------|
| Install SIEM in test environment | Dec 1–3 | Dec 3, 2025 | ✅ On time |
| Collect log sources | Dec 4–9 | Dec 9, 2025 | ✅ On time |
| Configure dashboards and alerts | Dec 10–17 | Dec 16, 2025 | ✅ 1 day early |
| Testing and feedback | Dec 18–21 | Dec 22, 2025 | ⚠️ 1-day delay (alert tuning required) |
| Staff training | Dec 22–24 | Dec 24, 2025 | ✅ On time |
| Production rollout | Dec 25–30 | Dec 29, 2025 | ✅ 1 day early |

### Log Source Onboarding Summary (Appendix A)

| Log Source | Status | Ingestion Date | Events/Day | Notes |
|-----------|--------|---------------|-----------|-------|
| Azure AD Sign-In Logs | ✅ Connected | 12/22/2025 | 14,200 | Identity logs; highest volume source |
| Windows Security Events | ✅ Connected | 12/22/2025 | 8,950 | Server and endpoint logs |
| Defender for Endpoint | ✅ Connected | 12/22/2025 | 1,120 | Malware alerts ingested |
| Firewall Logs | ✅ Connected | 12/22/2025 | 5,830 | Network logs normalized |
| POS Logs | ✅ Connected | 12/22/2025 | 2,415 | POS device activity collected |
| VPN Logs | ✅ Connected | 12/22/2025 | 980 | Required custom parser (see Scope Creep) |

### Unanticipated Scope Creep
VPN logs were not formatted to Sentinel's expected ASIM schema on initial onboarding — fields including source IP, connection status, and username were either mapped incorrectly or missing entirely. This prevented Sentinel from correlating VPN authentication events with other log sources. Resolution required building a custom parser and applying a Sentinel transformation rule. Resolved within the same sprint with no long-term schedule impact; the fix actually improved overall log quality and detection accuracy.

### Project Success Metrics

| Metric | Measurement Method | Result |
|--------|-------------------|--------|
| **Detection Accuracy** | Controlled simulations: phishing, credential stuffing, malicious PowerShell, lateral movement | All scenarios triggered alerts; one authentication rule required threshold/time-window tuning; post-tuning alerts were accurate and consistent ✅ |
| **Log Coverage** | Data Connectors dashboard showing active ingestion pipelines | All 6 critical log source categories connected, verified active, and normalized via ASIM ✅ |
| **Staff Readiness** | Structured workshops; KQL query exercises; simulated alert response | Staff demonstrated independent alert investigation, dashboard navigation, and incident escalation; no significant knowledge gaps identified ✅ |

### Environmental Changes Post-Implementation

| Before SIEM | After SIEM |
|-------------|-----------|
| Logs stored in isolated silos per system | All logs centralized in Microsoft Sentinel |
| Reactive monitoring; incidents discovered after damage occurred | Proactive, automated detection with real-time alerts |
| Inconsistent alert handling across staff members | Standardized incident investigation using Sentinel entity timelines and event graphs |
| Security reviews occasional and manual | Daily Workbook reviews embedded in IT operational routine |
| No formal log retention, access management, or documentation standards | Formal policies implemented for log retention, access management, and documentation |
| Leadership lacked visibility into risk patterns | Sentinel dashboards enable data-driven security decision-making at the leadership level |

### Literature Review (3 Works — Task 3)

| Source | Influence on Implementation |
|--------|---------------------------|
| **Microsoft Sentinel Deployment & Best Practices Guide** (2023) | Guided log source prioritization (identity first), KQL ingestion validation, ASIM schema mapping, analytics rule management (scheduled vs. behavioral), and Azure Logic Apps automation design |
| **SANS Institute — Improving SOC Operations Through Centralized Log Management** (2022) | Informed Sentinel Workbook design for authentication/endpoint/firewall monitoring; motivated Sprint 4 tuning process to reduce alert fatigue; supported SOC maturity transition from reactive log review to proactive detection |
| **Splunk — Designing Effective Correlation Searches for Real-Time Threat Detection** (2021) | Applied platform-neutral event chaining and time-window correlation concepts to Sentinel analytics rule development; inspired brute-force and password spray detection logic; provided guidance on threshold settings to minimize false positives |

---

## Technologies & Platforms

| Technology | Role in Project |
|-----------|----------------|
| **Microsoft Sentinel** | Primary SIEM platform — log ingestion, analytics rules, dashboards (Workbooks), incident management |
| **Azure Log Analytics Workspace** | Backend data store for all ingested security logs |
| **ASIM (Advanced Security Information Model)** | Sentinel's normalization schema ensuring consistent event structure across heterogeneous log sources |
| **KQL (Kusto Query Language)** | Used to validate ingestion pipelines and build analytics/detection rules |
| **Microsoft Defender for Endpoint** | Endpoint telemetry and malware alert ingestion |
| **Azure Active Directory** | Identity log source; sign-in logs and audit logs |
| **Azure Logic Apps** | Automated response playbooks (e.g., disable compromised accounts, block malicious IPs) |
| **UEBA (User and Entity Behavior Analytics)** | Behavioral anomaly detection within Sentinel |

---

## Compliance & Standards

| Standard | Relevance to Project |
|---------|---------------------|
| **PCI-DSS** | Requires centralized logging, log retention, and continuous monitoring for payment card systems; SIEM directly resolves pre-existing compliance gaps |
| **NIST SP 800-137** | Federal ISCM framework; automated correlation and enterprise-wide visibility requirements align directly with SIEM capabilities |

---

## References

- IBM Security. (2023). *Cost of a data breach report 2023.* https://www.ibm.com/security/data-breach
- Microsoft. (2023). *Sentinel deployment and best practices guide.* https://learn.microsoft.com/en-us/azure/sentinel/
- National Institute of Standards and Technology. (2011). *NIST SP 800-137: Information security continuous monitoring (ISCM) for federal information systems and organizations.* https://doi.org/10.6028/NIST.SP.800-137
- SANS Institute. (2022). *Improving SOC operations through centralized log management.* https://www.sans.org/white-papers/
- Splunk. (2021). *Designing effective correlation searches for real-time threat detection.* https://www.splunk.com/en_us/resources.html
- Splunk. (2022). *Security analytics and SIEM: Whitepaper on modern security operations.* https://www.splunk.com
- Verizon. (2023). *2023 data breach investigations report.* https://www.verizon.com/business/resources/reports/dbir/

---

*All work is original and based on WGU C769 IT Capstone course requirements.*
