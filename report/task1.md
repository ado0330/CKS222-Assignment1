# **Task 1: Process Definition and Modelling**

## **SPEM 2.0 Method Content: Code Review and Static Analysis**

### **Current practice**

MyRapid PULSE does not publish how code changes are checked, so we inferred the current practice from public evidence. Two App Store reviews report that a July 2026 update removed the daily bus schedule, departure times at bus stops and bus speed, and one reviewer asked whether the update had been tested at all (Figure 2). The developer's replies on 18 August 2026 apologised but described no change to how updates are checked.

*Figure 2: App Store reviews of MyRapid PULSE dated 23 and 30 July 2026, with developer responses dated 18 August 2026*

A second developer reading the code would be likely to question a change that removes features users depend on, so we infer that changes were not reviewed against existing features before release. Prasarana may have internal practices that are not public, so this is our interpretation of the evidence. Code review and static analysis will not catch every defect (testing is covered in Task 3), but they are the earliest point at which such a change can be stopped.

The activity is therefore defined below as reusable SPEM 2.0 method content: roles, work products, and tasks with steps, independent of any one project schedule.

### **Role definitions**

Table 1 defines the three roles. A role is a set of responsibilities and skills rather than a particular person, so one developer can be the Developer on one change and the Peer Reviewer on another.

*Table 1: SPEM 2.0 role definitions*

| Role | Responsibilities | Skills |
| :---- | :---- | :---- |
| Developer | Writes the code change for a user story. Runs static analysis on the change and fixes the issues it reports. Submits the change for review with a description of what changed and why. | Mobile app development. Working knowledge of the coding standard and the static analysis tool. |
| Peer Reviewer | Reads the change and checks it against the user story, the coding standard and the review checklist. Confirms that existing features, such as departure times at bus stops, still work. Records comments and a decision. | Familiar with the module being changed. Working knowledge of the coding standard. |
| Tech Lead | Maintains the coding standard and the static analysis rule set. Decides when the Developer and Peer Reviewer disagree. Gives final approval before the change is merged. | Senior development experience. Overview of the whole app and its release plan. |

### **Work product definitions**

\[To be written: three work products, each marked as input or output for each task.\]

### **Task definitions and steps**

\[To be written: two tasks, each broken into sequential steps.\]

### **Notion Electronic Process Guide**

\[To be added: Share Link, database screenshots and the updates panel screenshot.\]

## **RACI Responsibility Matrix**

The reorganised PULSE team has five roles: a Product Owner who owns the backlog and decides releases, a Scrum Master who runs sprints and removes blockers, a Tech Lead who owns the architecture, coding standard and merge approval, Developers who build and review features, and a QA Engineer who plans and runs system and acceptance testing.

Table 3 maps seven deliverables across the five SDLC stages (requirements, design, implementation, testing and maintenance) and project control to the five roles. R \= Responsible (does the work), A \= Accountable (signs it off), C \= Consulted, I \= Informed.

Table 3: RACI matrix for the PULSE development lifecycle

| Deliverable (stage) | Product Owner | Scrum Master | Tech Lead | Developer | QA Engineer |
| :---- | :---- | :---- | :---- | :---- | :---- |
| User stories and acceptance criteria (requirements) | R/A | I | C | C | C |
| Architecture and design specification (design) | C | I | A | R | C |
| Source code and Code Change Request (implementation) | I | I | A | R | I |
| Static Analysis Report and Review Record (implementation) | I | I | A | R | I |
| Test plan and test report (testing) | C | I | C | C | R/A |
| Release approval and app store update (maintenance) | A | I | R | I | C |
| Sprint progress report (project control) | I | R/A | I | I | I |

### **Constraint check and justification**

Every deliverable has exactly one A and at least one R, and every role holds at least one R or A, so no deliverable lacks a clear owner and no role exists only to be informed. R/A is used only where one owner can both produce and sign off the work.

The allocations target the weaknesses in the current practice. The Tech Lead is accountable for design, code and the review record, so one person owns the decision to merge, the control that was missing when the July update removed features. The Product Owner is accountable for each release and consults the QA Engineer first, so an update that changes what commuters see needs explicit sign-off. The QA Engineer owns testing independently of the developers, supporting the verification and validation process in Task 3, and the Scrum Master owns only the progress report, keeping process and product ownership separate. The Developer and Tech Lead match the SPEM roles, and the Peer Reviewer is a Developer acting as reviewer, so the review record is the Developer's responsibility.

