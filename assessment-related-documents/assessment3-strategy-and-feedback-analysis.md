# Phase 1: Assessment 3 Strategy & Feedback Analysis

## 1. The Scope Adjustments (Addressing Maneerat's Feedback)
To elevate this from an 83% (Distinction) to an 85%+ (High Distinction), we must modify the scope of the report and the UI to explicitly address the assessor's notes.

* **Competitor Analysis Expansion:** In the "Recap of Your Idea" section, we will explicitly add a paragraph comparing ResConnect to generic tools like Slack and Teams. We will emphasize that Slack requires heavy manual channel management and lacks built-in pastoral care workflows, making ResConnect superior for residential life.
* **Persona Deep Dive:** We will inject more realism into the personas to show deep empathy for the users. 
    * *Reece:* We will highlight the specific friction of balancing heavy 3rd-year IT units and part-time work alongside the cognitive load of tracking duty handovers manually.
    * *Kunihiro:* We will emphasize the isolation of navigating a new country and the specific anxiety of deciding whether a dripping tap warrants bothering an RL.
* **UI Adjustments for Clarity:** * **Event Kanban:** The HTML/CSS design will feature explicit visual separation and clear headers to address the "Would be better if you could explain e.g, A... B..." comment.
    * **Resident Feed:** We will ensure the Floating Action Button (FAB) for the maintenance report is highly intuitive, using standard iconography and a tooltip.

## 2. Alternative Paths Plan (Scenario Edge Cases)
Maneerat explicitly asked to "consider different paths the user might take and describe alternative scenarios" to show system robustness.

* **Scenario 1 (Duty Report) - Offline Edge Case:** The system detects no connection, saves the report locally to the device cache, displays a "Saved as Draft - Offline" banner, and auto-submits when connectivity returns.
* **Scenario 2 (Event Kanban) - Rejection Edge Case:** If the RLC rejects the risk assessment, the Kanban status turns red ("Revision Required"), unlocks the PDF upload button, and opens a mandatory comment box showing the RLC's feedback.
* **Scenario 3 (Resident Feed) - Duplicate Issue Edge Case:** When Kunihiro selects a location, a dynamic prompt appears: *"1 known issue already reported here. Is it the shower head?"* allowing him to upvote instead of duplicating.

## 3. Targeted Fixes for Assessment 2 Mark Deductions
Based on the specific grading breakdown, we will over-deliver in the following Assessment 3 sections:
* **HCI Principle Reflection (Lost 2.5/5.0):** This was the biggest deduction. In Assessment 3, the "Design Decisions" section will be exhaustive. We will not just mention Cialdini or Wickens; we will explicitly state *how* the HTML/CSS Grid layout reduces cognitive load, *how* the specific use of CQUniversity Lime Green draws the eye to the FAB, and *how* the typography hierarchy satisfies Nielsen's heuristics.
* **LoFi Wireframes/Prototyping (Lost 1.5/7.5):** The high-fidelity prototype will leave nothing to the imagination. The UI will be self-documenting, and our report will explain every single container, button state, and hover effect.
* **Scenarios & HTA (Lost 1.0/10.0):** We will include visual flowcharts (using Mermaid.js or standard diagrams) in the report instead of just text lists.
* **Personas (Lost 0.5/5.0) & Introduction (Lost 0.25/2.5):** Fixed via the Scope Adjustments in Section 1.

## 4. The Assessment 3 HD Checklist
Mapped directly to the Assessment 3 High Distinction Rubric:

### Report Component (~45% of total grade)
* [ ] **Recap (10%):** Concise summary (~250 words) explicitly detailing the scope changes (competitor analysis and persona depth).
* [ ] **Usability Study Results (20%):** Comprehensive 2-page report detailing tests on 3 users, including deep analysis of errors, completion times, and redesign recommendations.
* [ ] **Design Decisions (10%):** Thorough articulation (~500 words) mapping UI elements directly to established HCI principles to recover the lost marks from A2.
* [ ] **Limitations (10%):** Insightful, highly critical look at the prototype's shortcomings and future potential.
* [ ] **Presentation (10%):** Flawless organization, clear headings, and perfect IEEE/Harvard referencing.

### Prototype Component (40% of total grade)
* [ ] **Framework-Free:** Custom HTML5 and CSS3 (No Bootstrap/Tailwind).
* [ ] **Responsive Grid:** Content organized using CSS Grid.
* [ ] **Breakpoints:** Explicit media queries defined for Mobile and Tablet.
* [ ] **Mobile Layout:** Single-column layout on mobile devices with a hamburger menu.
* [ ] **Visual Evidence:** High-quality screenshots of the main page and all 3 scenarios.