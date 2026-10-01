# Incident Log: INC-1003

## Metadata
* **Ticket ID:** INC-1003
* **Reporter:** Security Information & Event Management (SIEM)
* **Category:** Cybersecurity / Identity Access
* **Priority:** P2 - High
* **Status:** Escalated (Tier 2 - Security Operations)
* **Assigned To:** SecOps / Identity Team

---

## 1. Issue Description
Automated SIEM alert triggered for user `j.doe@company.com`. Successful login detected from an unrecognized IP address in foreign jurisdiction 10 minutes after a login from the office IP.

## 2. Impact Analysis
* **User Impact:** Medium (Specific account isolated).
* **Business Impact:** High risk of unauthorized data access or credential compromise.

## 3. Tier 1 Preliminary Troubleshooting Attempted
- [x] Initiated immediate account lock in Active Directory/Entra ID.
- [x] Revoked all active SSO session tokens.
- [x] Contacted user via registered mobile number (User confirmed they are in the office and did not initiate foreign login).

## 4. Escalation Justification & Decision
* **Action:** Escalated to Tier 2 Security Operations (SecOps).
* **Justification:** Account isolation completed per playbook. Full forensic audit of access logs, endpoints, and potentially compromised data requires SecOps tools and authority.