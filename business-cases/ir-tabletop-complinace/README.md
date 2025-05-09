# Tabletop Incident Response & GDPR Drill

This directory contains all artifacts for a **ransomware tabletop exercise** focused on NIST CSF readiness and GDPR breach-notification workflows.  
Ideal for demonstrating your process, documentation rigor, and executive reporting to CISOs and security leadership.

---

## 📌 Project Overview

- **Objective:**  
  Simulate a ransomware attack on an EU-based customer database, exercise detection, containment, and GDPR-compliant notification (Art. 33–34).

- **Scope & Roles:**  
  - SOC Analyst  
  - Incident Response Lead  
  - Legal Counsel  
  - PR/Communications  
  - Business Owner  
  - CISO (Observer)

---

## 🗂️ Artifacts

### 1. Scenario & Injects
- [scenario/tabletop-script.md](scenario/tabletop-script.md) – Detailed timeline, IDS alerts, and periodic injects.  
- [scenario/injects-schedule.csv](scenario/injects-schedule.csv) – CSV of time-boxed injects for facilitator.

### 2. Templates
- [templates/gdpr-notification-template.docx](templates/gdpr-notification-template.docx) – Fill-in breach notification letter.  
- [templates/ir-ticket-template.xlsx](templates/ir-ticket-template.xlsx) – IR ticket fields aligned to NIST SP 800-61r2.  
- [templates/board-briefing-slide.pptx](templates/board-briefing-slide.pptx) – Executive summary slide.

### 3. After-Action Review (AAR)
- [aar/AAR-deck.pdf](aar/AAR-deck.pdf) – Slide deck with findings mapped to NIST CSF & GDPR.  
- [aar/POAM-dashboard.png](aar/POAM-dashboard.png) – Traffic-light POAM summary.

### 4. Detailed Walkthrough
- [docs/walkthrough.md](docs/walkthrough.md) – Step-by-step guide on running the drill, timing, and facilitation tips.

---

## 📊 Highlights & How to Use

1. **Review** the scenario script to understand the threat progression.  
2. **Assign** roles using `roles-and-RACI.md`.  
3. **Run** the exercise by following `injects-schedule.csv`—deliver each inject at the specified time.  
4. **Utilize** the templates to capture IR tickets, draft your GDPR notification, and brief the board.  
5. **Conduct** the After-Action Review (AAR) using the slide deck; update the POAM dashboard.  
6. **Share** this repo link with stakeholders to demonstrate your end-to-end process.

---
