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

### **Roles and deliverables**

\[To be written: five roles and six deliverables, to be confirmed with the group on 20 Nov.\]

### **Matrix**

\[To be added: the RACI table.\]

### **Constraint check and justification**

\[To be written: one Accountable and at least one Responsible per deliverable, with reasons for the allocations.\]