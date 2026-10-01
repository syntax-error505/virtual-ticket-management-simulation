# Incident Log: INC-1005

## Metadata
* **Ticket ID:** INC-1005
* **Reporter:** Finance Department Lead
* **Category:** Desktop Application / OS Compatibility
* **Priority:** P3 - Medium
* **Status:** Escalated (Tier 2 - Application Support)
* **Assigned To:** Desktop Engineering

---

## 1. Issue Description
Custom legacy ERP software crashes instantly upon startup with error code `0xC0000005 (Access Violation)` following a Windows 11 cumulative update.

## 2. Impact Analysis
* **User Impact:** Medium (Finance team member cannot generate weekly invoices).
* **Business Impact:** Moderate administrative delay.

## 3. Tier 1 Preliminary Troubleshooting Attempted
- [x] Executed app as Administrator (Failed).
- [x] Verified application compatibility mode settings (Windows 10/8 mode failed).
- [x] Reinstalled application package from IT deployment share (Failed).

## 4. Escalation Justification & Decision
* **Action:** Escalated to Tier 2 Application / Desktop Engineering.
* **Justification:** Core issue relates to DLL conflict caused by latest OS patch. Tier 2 needs to evaluate rolling back the Windows patch via Endpoint Manager or pushing a compatibility registry patch.