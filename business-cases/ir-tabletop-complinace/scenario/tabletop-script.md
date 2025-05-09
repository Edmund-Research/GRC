# Tabletop Exercise Script
**Project:** Ransomware Incident Drill (NIST CSF + GDPR)  
**Facilitator:** [Name]  
**Date & Time:** [Date], T=0 to T+72 hrs

---

## 1. Overview & Objectives
- **Purpose:** Validate IR playbook against NIST CSF Detection & Response functions and GDPR notification requirements (Art. 33–34).  
- **Scenario Summary:** Simulate a ransomware attack on an EU-hosted customer database that encrypts data and exfiltrates PII.  
- **Goals:**  
  1. Test detection & escalation workflows.  
  2. Exercise containment & eradication decisions.  
  3. Draft timely GDPR breach notification.  
  4. Produce board-level briefing within 72 hrs.

---

## 2. Roles & Instructions
| Role                   | Name / Team        | Responsibility                             |
|------------------------|--------------------|--------------------------------------------|
| SOC Analyst            | [Name]             | Triage alerts, initial investigation       |
| Incident Response Lead | [Name]             | Orchestrate containment, assign tasks      |
| Legal Counsel          | [Name]             | Assess GDPR trigger, draft notification    |
| PR / Communications    | [Name]             | Prepare external/internal messaging        |
| Business Owner         | [Name]             | Provide business context, approve actions  |
| CISO Observer          | [Name]             | Oversight, decision escalation             |

---

## 3. Initial Conditions (T=0)
> **Inject #0** (9:15 UTC):  
> - IDS alert: “Multiple SMB connections from DB-FR-01 to unknown external IP.”  
> - User report: “Database UI slow and unresponsive.”  
> - SIEM log excerpt attached in `logs/initial-ids.txt`.

**Facilitator Prompt:**  
> “SOC Analyst, what’s your first step? Do you escalate to IR team?”

---

## 4. Inject Schedule & Script

| **Time**   | **Inject**                                                                    | **Facilitator Notes**                           |
|------------|-------------------------------------------------------------------------------|-------------------------------------------------|
| T+1 hr     | “Backup monitoring alert: Unusual file rename operations in backup share.”    | Guide discussion to containment options.        |
| T+2 hrs    | “Ransom note found on DB-FR-01: ‘Your files are encrypted… contact x@y.com.’” | Trigger eradication planning.                   |
| T+8 hrs    | “External threat intel: Similar variant targeting EU financial services.”     | Assess need for external notification.          |
| T+24 hrs   | “Forensics report: ~10k EU customer PII encrypted & exfiltrated.”             | Legal: Draft GDPR notification (Art. 33).       |
| T+48 hrs   | “Regulator questions received: Need clarifications on ‘measures taken.’”      | PR/Legal: Finalize notification; board memo.    |

---

## 5. Discussion Questions
- How do you validate the integrity of backups before restore?  
- What logs or evidence do you collect for the GDPR notification?  
- If the ransomware authors demand payment, how does that affect your risk appetite and legal obligations?

---

## 6. Expected Deliverables
1. **IR Ticket** in `templates/ir-ticket-template.xlsx` with timeline & actions.  
2. **GDPR Notification Draft** using `templates/gdpr-notification-template.docx`.  
3. **Board Briefing Slide**: populate `templates/board-briefing-slide.pptx`.  
4. **AAR Findings** mapped to NIST CSF & GDPR, to be captured in `aar/AAR-deck.pdf`.  

---

## 7. After-Action Wrap-Up
- Remind participants to complete the **POAM** in `aar/POAM-dashboard.png`.  
- Schedule a 1-hour AAR meeting to capture lessons learned and assign owners.
