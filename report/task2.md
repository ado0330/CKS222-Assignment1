[CKS222 Task 2- Requirements Quality & Agile User Stories (INVEST & GWT).md](https://github.com/user-attachments/files/35039217/CKS222.Task.2-.Requirements.Quality.Agile.User.Stories.INVEST.GWT.md)
# **Task 2: Requirements Quality & Agile User Stories (INVEST & GWT)**

## **2.1 Selected Feature Backlog Item**

The selected organisation is Prasarana Malaysia Berhad, and the application being audited is MyRapid PULSE. Prasarana describes PULSE as an application that helps public transport users plan their journeys.

The proposed major feature backlog item is:

Improve journey planning by allowing passengers to search for public transport routes and prioritise routes with fewer transfers.

This feature helps passengers identify how to reach their destination and choose a journey that matches their preferences. Some passengers may prioritise travel time, while others may prefer fewer service changes even if the journey takes longer.

Therefore, the feature is divided into two user stories:

* US1: Search for public transport routes.

* US2: Search for routes with fewer transfers.

The following requirements describe proposed behaviour for this assignment. They do not claim that these functions are currently missing from the PULSE application.

**2.2 Feature Scope and Business Rules**

To keep the stories manageable and testable, the proposed increment follows these rules:

| Item | Proposed rule |
| :---: | ----- |
| **Search inputs** | Passengers select an origin, destination and departure time. Locations must be recognised stops or stations within the supported network. |
| **Route information** | Each result shows the services used, boarding and alighting points, transfer locations, number of transfers and estimated total journey duration. |
| **Basic search order** | Routes are ordered by the shortest estimated total journey duration. If durations are equal, the route with fewer transfers appears first. |
| **Fewer-transfers order** | Routes are ordered by lowest transfer count. If transfer counts are equal, the shorter journey appears first. |
| **Transfer definition** | A transfer occurs when a passenger changes from one vehicle or rail service to another. Initial boarding and intermediate stops are excluded. |
| **Direct route** | A route requiring no service change has zero transfers. |
| **Number of results** | Display up to three distinct, feasible routes. |
| **Scope exclusions** | Live bus tracking, ticket purchasing, notifications and automatic rerouting are outside this increment. |

If two routes have the same duration and transfer count, a stable route identifier determines their order so that repeated searches against unchanged data produce consistent results.

## **2.3 Agile User Stories**

## **2.4 Evaluation against INVEST**

## **2.5 Given-When-Then (GWT) Acceptance Criteria**

### **2.5.1 US1 Basic Route Search**

### **2.5.2 US2 Fewer Transfer Search**

## **2.6 Definition of Done**

## **2.7 Control of Requirement Changes**

### 

