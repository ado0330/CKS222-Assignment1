[CKS222 Task 2- Requirements Quality & Agile User Stories (INVEST & GWT) (2).md](https://github.com/user-attachments/files/35172239/CKS222.Task.2-.Requirements.Quality.Agile.User.Stories.INVEST.GWT.2.md)
[CKS222 Task 2- Requirements Quality & Agile User Stories (INVEST & GWT).md](https://github.com/user-attachments/files/35039217/CKS222.Task.2-.Requirements.Quality.Agile.User.Stories.INVEST.GWT.md)

# **Task 2: Requirements Quality & Agile User Stories (INVEST & GWT)**

## **2.1 Selected Feature Backlog Item**

The selected organisation is Prasarana Malaysia Berhad, and the application being audited is MyRapid PULSE. Prasarana describes PULSE as an application that helps public transport users plan their journeys.

The proposed major feature backlog item is:

Improve journey planning by enabling passengers to search for public transport routes and save frequently used journeys for future searches.

This feature addresses two passenger needs. Passengers need to identify routes to their destinations, while regular passengers need a convenient way to reuse the frequently entered journey details.

Therefore, the feature is divided into two distinct user stories:

* US1: Search for public transport routes.

* US2: Save and reuse a favourite journey.

These stories represent proposed requirements for the audit. They do not establish that the functions are currently absent from the PULSE application.

## **2.2 Scope and Proposed Business Rules**

The first increment is limited to an agreed pilot network. Live tracking, ticket purchasing, journey sharing and automatic rerouting are outside of the scope.

| Area | Proposed business rule |
| :---: | ----- |
| **Search inputs** | Passengers select an origin, destination and departure time.  |
| **Valid endpoints** | The origin and destination must refer to different recognised stops or stations. |
| **Search results** | Display up to three distinct, feasible routes, ordered by estimated total journey duration. |
| **Route details** | Each result shows the services used, boarding and alighting points, transfer locations and estimated total journey duration. |
| **Favourite contents** | A favourite stores an origin-destination pair under the signed-in passenger’s account.  |
| **Saving a favourite** | Passengers can save selected endpoints directly without first completing a route search. |
| **Duplicate rule** | The same ordered pair cannot be saved twice under one account. A-to-B and B-to-A are treated as different journeys. |
| **Favourite limit** | Each account can store a maximum of ten favourite journeys. |
| **Reusing a favourite** | Selecting a favourite prefills the origin and destination. The passenger selects or confirms the departure time before searching. |
| **Saved information** | Favourites store endpoints rather than previous routes or timetable results. Each new search uses the available journey information at that time. |

The ten favourites limit is a proposed boundary for this increment and should be confirmed during backlog refinement.

## **2.3 Agile User Stories**

**User Story 1 \- Search for Public Transport Routes**

**As a public transport passenger, I want to search for routes between my selected origin and destination so that I can plan how to reach my destination.**

The passenger selects journey details and receives feasible route options. The results provide enough information to compare journeys and identify the required services and transfers.

This story does not require the passenger to save a favourite.

**User Story 2 \- Save and Reuse a Favourite Journey**

**As a regular public transport passenger, I want to save an origin-destination pair as a favourite journey so that I can reuse it without entering the same locations again.**

The passenger saves frequently used endpoints and later selects them to prefill the journey-planning form. This reduces repeated input for journeys such as travelling between home and university. 

Saving is available directly from endpoint selection. It does not depend on a successful route search. Account authentication is a prerequisite provided by the existing account service while developing registration and login is outside this user story. 

## 

## 

## 

## **2.4 Evaluation Against INVEST**

INVEST evaluates whether a user story is Independent, Negotiable, Valuable, Estimable, Small and Testable. The following evaluation applies these criteria to both stories.

### **2.4.1 INVEST Criterion for Basic Route Search**

| INVEST criterion | US1 — Basic Route Search |
| :---: | ----- |
| **Independent** |  |
| **Negotiable** |  |
| **Valuable** |  |
| **Estimable** |  |
| **Small** |  |
| **Testable** |  |

*Table 2.4.1 INVEST Criterion for* 

### **2.4.2 INVEST Criterion for Fewer-Transfer Search**

| INVEST criterion | US2 — Fewer-Transfer Search |
| :---: | ----- |
| **Independent** |  |
| **Negotiable** |  |
| **Valuable** |  |
|    **Estimable** |  |
| **Small** |  |
| **Testable** |  |

*Table 2.4.2 INVEST Criterion for* 

## **2.5 Given-When-Then (GWT) Acceptance Criteria**

### **2.5.1 US1 Basic Route Search**

### **2.5.2 US2 Fewer Transfer Search**

## **2.6 Definition of Done**

## **2.7 Control of Requirement Changes**

### 



