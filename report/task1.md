# **Task 1: Process Definition and Modelling**

## **1.1 SPEM 2.0 Method Content: Code Review and Static Analysis**

### **1.1.1 Current Practice**

MyRapid PULSE does not publish how code changes are checked, so we inferred the current practice from public evidence. Two App Store reviews report that a July 2026 update removed the daily bus schedule, departure times at bus stops and bus speed, and one reviewer asked whether the update had been tested at all (Figure 1.1). The developer's replies on 18 August 2026 apologised but described no change to how updates are checked.

*Figure 1.1: App Store reviews of MyRapid PULSE dated 23 and 30 July 2026, with developer responses dated 18 August 2026*

A second developer would likely have questioned a change that removes features users depend on, so we infer that changes were not reviewed against existing features before release, although Prasarana may have internal practices that are not public. Code review and static analysis cannot catch every defect (testing is covered in Task 3), but they are the earliest point at which such a change can be stopped, so they are defined below as reusable SPEM 2.0 method content.

### **1.1.2 Role Definitions**

Table 1.1 defines the three roles. A role is a set of responsibilities and skills, not a person, so one developer can be the Developer on one change and the Peer Reviewer on another.

*Table 1.1: SPEM 2.0 role definitions*

| Role | Responsibilities | Skills |
| :---- | :---- | :---- |
| Developer | Writes the code change for a user story. Runs static analysis on the change and fixes the issues it reports. Submits the change for review with a description of what changed and why. | Mobile app development. Working knowledge of the coding standard and the static analysis tool. |
| Peer Reviewer | Reads the change and checks it against the user story, the coding standard and the review checklist. Confirms that existing features, such as departure times at bus stops, still work. Records comments and a decision. | Familiar with the module being changed. Working knowledge of the coding standard. |
| Tech Lead | Maintains the coding standard and the static analysis rule set. Decides when the Developer and Peer Reviewer disagree. Gives final approval before the change is merged. | Senior development experience. Overview of the whole app and its release plan. |

### **1.1.3 Work Product Definitions**

Table 1.2 defines the three work products and their access mode in each task: input (read), output (produced) or input/output (read and then updated).

Table 1.2: SPEM 2.0 work products and access modes

| Work product | Description | Run Static Analysis | Conduct Peer Code Review |
| :---- | :---- | :---- | :---- |
| Code Change Request | The pull request: the code change, what changed and why, and a link to the user story it implements. | Input/output | Input |
| Static Analysis Report | Warnings and errors found by the tool, each with its location and severity. An unresolved high-severity issue blocks the change from review. | Output | Input |
| Review Record | The reviewer's comments, the completed checklist, and the decision to approve or request changes. | Not used | Output |

Every work product is produced or used by at least one task, so there are no orphan entities, and the report flows only from the first task to the second, so there is no dependency cycle. The coding standard and review checklist are modelled as SPEM guidance.

### **1.1.4 Task Definitions and Steps**

#### **1.1.4.1 Run Static Analysis**

Performed by the Developer. Input/output: Code Change Request. Output: Static Analysis Report. Guidance: coding standard and static analysis rule set.

1. Commit the code change to a feature branch and open a Code Change Request linked to its user story.  
2. Run the static analysis tool on the changed files using the team's rule set.  
3. Read the Static Analysis Report and sort the issues by severity.  
4. Fix every high-severity issue, and fix or justify each remaining warning in the Code Change Request.  
5. Run the tool again until no high-severity issue remains, then attach the final report and submit the Code Change Request for review.

#### **1.1.4.2 Conduct Peer Code Review**

Performed by the Peer Reviewer, assisted by the Tech Lead. Inputs: Code Change Request and Static Analysis Report. Output: Review Record. Guidance: review checklist.

1. Read the linked user story and its acceptance criteria.  
2. Confirm from the Static Analysis Report that no high-severity issue remains.  
3. Read the code change against the review checklist, including whether any existing feature, such as departure times at bus stops, has been removed or changed.  
4. Record comments and the completed checklist in the Review Record.  
5. Approve the change or request changes. If changes are requested, the Developer updates the Code Change Request and Run Static Analysis is repeated.  
6. The Tech Lead checks the Review Record, gives final approval and merges the change.

### **1.1.5 Notion Electronic Process Guide**

The method content is published as a Notion Electronic Process Guide at [https\://app.notion.com/p/CKS222-Assignment-41a66e96893880678791e0b127e31dce?source=copy\_link](https://app.notion.com/p/CKS222-Assignment-41a66e96893880678791e0b127e31dce?source=copy_link), using four linked databases: Roles, Work Products, Tasks and Steps. Each task links to its role, work products and steps.

## **1.2 RACI Responsibility Matrix**

The reorganised PULSE team has five roles: Product Owner (backlog and releases), Scrum Master (sprints and blockers), Tech Lead (architecture, coding standard and merges), Developers (building and reviewing features) and QA Engineer (system and acceptance testing).

Table 1.3 maps seven deliverables across the five SDLC stages and project control to the five roles: R \= Responsible, A \= Accountable, C \= Consulted, I \= Informed.

Table 1.3: RACI matrix for the PULSE development lifecycle

| Deliverable (stage) | Product Owner | Scrum Master | Tech Lead | Developer | QA Engineer |
| :---- | :---- | :---- | :---- | :---- | :---- |
| User stories and acceptance criteria (requirements) | R/A | I | C | C | C |
| Architecture and design specification (design) | C | I | A | R | C |
| Source code and Code Change Request (implementation) | I | I | A | R | I |
| Static Analysis Report and Review Record (implementation) | I | I | A | R | I |
| Test plan and test report (testing) | C | I | C | C | R/A |
| Release approval and app store update (maintenance) | A | I | R | I | C |
| Sprint progress report (project control) | I | R/A | I | I | I |

### **1.2.1 Constraint Check and Justification**

Every deliverable has exactly one A and at least one R, and every role holds at least one R or A, so every deliverable has a clear owner and no role is only informed.

The Tech Lead is accountable for design, code and the review record, so one person owns the merge decision, the control that was missing when the July update removed features. The Product Owner is accountable for each release and consults the QA Engineer first, so user-facing changes need sign-off. The QA Engineer tests independently of the developers, and the Scrum Master owns only the progress report, keeping process and product ownership separate. The Peer Reviewer is a Developer, so the review record is the Developer's responsibility.