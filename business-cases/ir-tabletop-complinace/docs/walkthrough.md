# Tabletop Drill Walkthrough

This guide explains how to run the “Ransomware Incident Drill” from start to finish. It assumes you have completed the **scenario**, **roles & RACI**, and **injects** files, and have your **templates** (IR ticket, GDPR letter, board slide) and **AAR artifacts** ready.

---

## 1. Prerequisites

- **Artifacts in place**  
  - `scenario/tabletop-script.md`  
  - `scenario/injects-schedule.csv`  
  - `scenario/roles-and-RACI.md`  
  - `templates/ir-ticket-template.xlsx`  
  - `templates/gdpr-notification-template.docx`  
  - `templates/board-briefing-slide.pptx`  
- **AAR folder** with `aar/AAR-deck.pdf` and `aar/POAM-dashboard.png`  
- **Facilitator** identified and deck of slides to show injects (optional)  
- **Timekeeper** with access to a clock or timer  
- **Participants** briefed and given copies of the IR playbook and GDPR checklist  

---

## 2. Kick-Off (T=0)

1. **Gather everyone** (in person or virtual).  
2. **Explain objectives & rules** (5–10 min):  
   - We’re simulating a ransomware incident on an EU database.  
   - No real changes to production.  
   - Time-boxed injects will drive the discussion.  
   - Document all decisions in the IR ticket and board slide.  
3. **Assign roles** by reviewing `roles-and-RACI.md`.  
4. **Show the exercise timeline** (brief slide or whiteboard).  

---

## 3. Exercise Execution

### A. Initial Detection & Triage (T+0 → T+1 hr)  
- **Deliver Inject G0** from `injects-schedule.csv`:  
  - Read: “IDS alert: multiple SMB connections… database slow.”  
- **SOC Analyst** logs the alert in the IR ticket (sheet: “Date/Time Detected,” “Initial Triage”).  
- **Group Discussion** (10 min):  
  - What’s your hypothesis? Do you escalate to IR? Where do you look next?  
- **Document** the decision in the ticket under “Containment Actions.”

### B. Containment & Malware Analysis (T+1 → T+8 hrs)  
- At **T+1 hr**, deliver Inject G1: “Backup monitoring alert: unusual file renames…”  
- **IR Lead** and **SOC Analyst** debate containment options (isolate server vs. block IP).  
- At **T+2 hrs**, deliver Inject G2: “Ransom note on DB-FR-01…”  
  - Record “Eradication Actions” (e.g. snapshot for forensics, isolate shares).  
- Continue discussion until **T+8 hrs**; update ticket and begin drafting the board slide.

### C. Impact Assessment & Notification (T+8 → T+48 hrs)  
- At **T+8 hrs**, deliver G3: “External intel—variant targeting EU finance.”  
  - **Legal Counsel** consulted: review GDPR trigger.  
- At **T+24 hrs**, deliver G4: “10k EU records exfiltrated.”  
  - **SOC Analyst** updates “Severity” and “Affected Systems.”  
  - **Legal Counsel** begins filling `gdpr-notification-template.docx`.  
- Between **T+24–T+48 hrs**:  
  - Team populates board slide (summary metrics & timeline).  
  - Finalize draft GDPR letter by **T+48 hrs**.

### D. Regulator Interaction & Wrap (T+48 → T+72 hrs)  
- At **T+48 hrs**, deliver G5: “Regulator requests clarifications.”  
  - Update GDPR letter and board slide with “Additional Measures” section.  
- By **T+72 hrs**, ensure the notification is “sent” (mock-send in template) and slide is complete.

---

## 4. After-Action Review

1. **Distribute** the completed IR ticket, GDPR letter, and board slide.  
2. **Present** the AAR deck (`aar/AAR-deck.pdf`) to participants.  
3. **Discuss** each “Key Finding” slide, confirm accuracy.  
4. **Review** the POAM snapshot (`aar/POAM-dashboard.png`):  
   - Are owners assigned?  
   - Are due dates realistic?  
   - Are statuses updated?  
5. **Capture** any new gaps or lessons learned.

---

## 5. Facilitation Tips

- **Keep time**: gently remind participants of the timeline.  
- **Encourage participation**: ask quieter roles for input (“Legal, how would you phrase the notification?”).  
- **Stay in scope**: if side-topics emerge, note them for later but redirect back to the inject.  
- **Use visuals**: show swimlane or timeline slide when moving phases.  
- **Document decisions live**: have the IR ticket open and visible to all.

---

## 6. Next Steps

- Finalize and version-control all artifacts in the repo.  
- Share the link with stakeholders.  
- Solicit feedback and schedule a full-scale (technical) drill if resources allow.  
- Repeat the exercise quarterly, updating injects and templates as regulations evolve.  
