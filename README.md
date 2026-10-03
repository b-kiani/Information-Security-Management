# Management of Information Security

Course materials for an undergraduate course on the **management side of information security**: governance, policy, risk, programs, people and planning. Each week has a lecture deck with full speaker notes and hands-on lab handouts. Students learn to think about security the way a manager or CISO does, not only the way a technician does.

The course follows the structure of *Management of Information Security*, 6th edition, by Michael E. Whitman and Herbert J. Mattord (Cengage). All slides, diagrams, labs and case studies in this repository are original material. They contain no publisher slides or figures.

> **Instructor:** Behnam Kiani ·  **Term:** _Fall 2026_

---

## Contents

- [Repository structure](#repository-structure)
- [Week 1: Introduction to the Management of Information Security](#week-1-introduction-to-the-management-of-information-security)
- [Course roadmap](#course-roadmap)
- [How to use these materials](#how-to-use-these-materials)
- [Requirements](#requirements)
- [Design conventions](#design-conventions)
- [Academic integrity and lab safety](#academic-integrity-and-lab-safety)
- [Sources](#sources)
- [Contributing](#contributing)
- [License](#license)

---

## Repository structure

```
.
├── README.md
├── LICENSE
├── .gitignore
└── week-01-introduction/
    ├── lecture/
    │   └── Week1_Lecture_Intro_to_Mgmt_of_InfoSec.pptx
    └── labs/
        ├── Lab1_Asset_Inventory_CIA.docx
        ├── Lab2_Integrity_Authentication_Passwords.docx
        └── Lab3_Threat_Analysis_Six_Ps.docx
```

Each new week gets its own folder with the same `lecture/` and `labs/` layout (`week-02-…`, `week-03-…`).

> **Answer keys are not published here.** Instructor answer keys (for example `Week1_Labs_Instructor_Answer_Key.docx`) are kept in a private repository or excluded with `.gitignore`. See [Academic integrity](#academic-integrity-and-lab-safety).

---

## Week 1: Introduction to the Management of Information Security

### Learning objectives

By the end of the week, students should be able to:

1. List and discuss the key characteristics of information security.
2. List and describe the dominant categories of threats to information security.
3. Discuss the key characteristics of leadership and management.
4. Describe the importance of the manager's role in securing an organization's information assets.
5. Differentiate information security management from general business management.

### Lecture deck (78 slides)

The deck is `lecture/Week1_Lecture_Intro_to_Mgmt_of_InfoSec.pptx`. Every slide has detailed speaker notes with explanations, discussion prompts and suggested timing.

| Part | Topics |
|---|---|
| **1. Foundations** | Information as an asset, the three communities of interest, what security is, specialized areas of security, the CNSS (McCumber) cube, the C.I.A. triad, privacy, identification, authentication, authorization, accountability |
| **2. Threats and attacks** | Vocabulary of risk, anatomy of an attack, the 12 categories of threats, password attacks, social engineering, the WannaCry case, DDoS and man-in-the-middle, MTBF/MTTR, OWASP Top 10:2025, technological obsolescence |
| **3. Management and leadership** | Management roles, leadership vs. management, POLC vs. POSDC, planning levels, the control process, governance (incl. NIST CSF 2.0 *Govern*), five-step problem solving, feasibility analyses |
| **4. The six Ps of InfoSec management** | Planning, policy (EISP / ISSP / SysSP), programs, protection, people, projects; security as a process vs. a project |
| **Wrap-up** | Two summary slides, key terms, eight review questions (answers in the notes), labs overview, references |

The deck also includes two in-class knowledge checks, three linked videos (IBM Technology and BBC News), and statistics from the IBM *Cost of a Data Breach Report 2025* and the Verizon *2025 DBIR*.

### Labs

All labs are done in pairs. Each handout has objectives, background, step-by-step tasks, fill-in tables, analysis questions, deliverables and a 100-point rubric.

| Lab | Title | Time | Objectives | What students do |
|---|---|---|---|---|
| 1 | Information Asset Inventory & CIA Classification | 60–75 min | 1, 4 | Inventory the assets of a fictional logistics company, assign owners and custodians, rate C/I/A impact, classify assets using the high-water mark, map controls to the McCumber cube, and check vendor end-of-support dates |
| 2 | Integrity, Authentication & Password Strength | 60–75 min | 1 | Use SHA-256 hashes to detect tampering and observe the avalanche effect, verify a download, calculate password keyspace and brute-force time, audit identification, authentication, authorization and accountability on one of their own accounts, and calculate allowed downtime from availability targets |
| 3 | Threat Analysis Case Study & Six Ps Plan | 75–90 min | 2, 3, 5 | Analyze a fictional clinic ransomware incident: classify events into the 12 threat categories, trace attack chains, apply five-step problem solving with feasibility scoring, and write a one-page six Ps plan (optional board briefing) |

**Before Lab 2:** post a small file and its published SHA-256 checksum on the course page for Part A3 (download verification).

---

## Course roadmap

This roadmap follows the chapter order of the 6th edition. Adjust it to your own syllabus.

- [x] **Week 1:** Introduction to the Management of Information Security
- [ ] **Week 2:** Compliance: Law and Ethics
- [ ] **Week 3:** Governance and Strategic Planning for Security
- [ ] **Week 4:** Information Security Policy
- [ ] **Week 5:** Developing the Security Program
- [ ] **Week 6:** Risk Management: Assessing Risk
- [ ] **Week 7:** Risk Management: Treating Risk
- [ ] **Week 8:** Security Management Models
- [ ] **Week 9:** Security Management Practices
- [ ] **Week 10:** Planning for Contingencies
- [ ] **Week 11:** Security Maintenance
- [ ] **Week 12:** Protection Mechanisms

---

## How to use these materials

### For instructors

1. **Download** the week folder, or clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. **Read the speaker notes** (View → Notes in PowerPoint). They are written to be teachable as-is and include discussion questions and model answers.
3. **Animations:** the parts of each slide fade in automatically, one after another. To advance them yourself, open *Animations → Animation Pane*, select the effects and change *Start* to **On Click**.
4. **Videos** are clickable panels that open in a browser. To embed a video instead, use *Insert → Video → Online Video* and paste the link from the slide.
5. **Printing:** the labs are A4 Word files designed for black-and-white printing. Students can also fill them in digitally and submit them as PDF.

### For students

- Download the lab handouts from the week's `labs/` folder before class.
- Submit each lab as a PDF named `LabN_Surname1_Surname2.pdf`. Follow the submission instructions in each handout.
- Review the key terms and review questions at the end of the lecture deck before the next class.

---

## Requirements

| Material | Software |
|---|---|
| Lecture decks (`.pptx`) | Microsoft PowerPoint 2016 or later (recommended), LibreOffice Impress, or Google Slides (animations may differ) |
| Lab handouts (`.docx`) | Microsoft Word, LibreOffice Writer, or Google Docs |
| Lab 2 | Any computer with a terminal: PowerShell / Command Prompt (Windows), Terminal (macOS), or a Linux shell |

No special software, virtual machines or paid tools are needed for Week 1.

---

## Design conventions

- **Monochrome:** black, white and grays only, so everything prints well on standard printers and works for color-blind readers.
- **Typography:** Cambria for headings, Calibri for body text.
- **Original visuals:** every diagram (C.I.A. triangle, McCumber cube, attack chains, control-process flowchart, six Ps) is redrawn from scratch. Icons come from the open-source Font Awesome set.
- **Fictional case studies:** all organizations in the labs (Silk Road Logistics LLC, Oasis Medical Clinics) are invented composites.

---

## Academic integrity and lab safety

- **Do not commit answer keys** to a public repository. Add them to `.gitignore`:
  ```gitignore
  # Instructor-only material
  *Answer_Key*
  answer-keys/
  ```
- Labs use **fictional organizations** and the **student's own files and accounts** only.
- Students must never enter real passwords into online "strength checkers", share credentials, or record secrets (passwords, MFA codes, recovery codes) in submissions.
- Attempting to access systems or accounts without authorization is a crime in most countries. All attack material in this course is taught for defense and management purposes.

---

## Sources

- Whitman, M. E., & Mattord, H. J. *Management of Information Security* (6th ed.). Cengage.
- IBM Security. *Cost of a Data Breach Report 2025.*
- Verizon. *2025 Data Breach Investigations Report.*
- OWASP Foundation. *OWASP Top 10:2025.* https://owasp.org/Top10/
- NIST. *Cybersecurity Framework (CSF) 2.0*, 2024.
- McCumber, J. (1991). *Information Systems Security: A Comprehensive Model.*
- Microsoft Security Bulletin MS17-010 (March 2017).

**Videos used in Week 1**
- IBM Technology: [What is the CIA Triad?](https://www.youtube.com/watch?v=kPPFNrlN3zo)
- IBM Technology: [Phishing Explained](https://www.ibm.com/think/videos/phishing)
- BBC News: [Cyber-attack: Ransomware causing chaos globally](https://www.youtube.com/watch?v=5v5gtycGTps)

---

## Contributing

Corrections and improvements are welcome, especially updated statistics, broken video links and clarifications to lab instructions.

1. Open an **issue** describing the problem or suggestion.
2. For changes, fork the repository, create a branch (`fix/week1-lab2-typo`) and open a **pull request**.
3. Keep the black-and-white design and do not add copyrighted publisher material.

---

## License

Unless otherwise noted, the original materials in this repository are licensed under
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) (CC BY-NC-SA 4.0).

You may share and adapt the materials for non-commercial teaching with attribution. The textbook, the linked videos and third-party trademarks belong to their respective owners and are not covered by this license.
