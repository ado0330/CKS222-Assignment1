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



## **2.4 Evaluation Against INVEST**

INVEST evaluates whether a user story is Independent, Negotiable, Valuable, Estimable, Small and Testable. 

Both stories provide user-facing outcomes. Neither is limited to a technical activity such as creating a database table or designing a screen.

Both stories are evaluated individually below.

### **2.4.1 INVEST Criterion for User Story 1 – Search for Public Transport Routes**

| INVEST criterion | US1 — Search for Public Transport Routes |
| :---: | ----- |
| **Independent** | Route searching works without the favourites function. It delivers a complete passenger outcome independently. |
| **Negotiable** | The arrangement of search controls and presentation of route details can be refined with passengers and the Product Owner. The goal remains finding suitable routes. |
| **Valuable** | Passengers can identify services and transfers needed in order to reach their destination and compare estimated journey durations. |
| **Estimable** | Supported locations, required inputs, output fields and failure cases define the work for validation, routing service integration, display and testing. Routing-service availability must be confirmed before estimation. |
| **Small** | The story covers a single search and its results within the pilot network. It excludes live tracking, ticketing and rerouting. Developers must confirm that it fits one sprint during planning. |
| **Testable** | Controlled route and timetable data can verify result accuracy, ordering, required information and handling of invalid inputs or unavailable services.  |

*Table 2.4.1 INVEST Criterion for US1– Search for Public Transport Routes*

### **2.4.2 INVEST Criterion for User Story 2 \- Save and Reuse a Favourite Journey**

| INVEST criterion | US2 — Save and Reuse a Favourite Journey |
| :---: | ----- |
| **Independent** | Passengers can save endpoints directly and retrieve them to prefill a form without first performing US1. Saving and retrieval can be implemented and tested separately from route calculation. |
| **Negotiable** | The save control, favourite-list layout and maximum number of favourites can be discussed during refinement. Agreed rules must be recorded before implementation and testing.  |
| **Valuable** | Regular passengers spend less time entering repeated journey details and reduce the risk of selecting the wrong endpoints. |
|    **Estimable** | The stored fields, account ownership, duplicate rule and ten-item limit define the work for saving, retrieving, prefilling and testing. Any uncertainty about account storage should be investigated first. |
| **Small** | The story covers saving endpoint pairs and selecting them for reuse. Editing, sharing, notifications and cross-device synchronisation are excluded. It should be split further if the estimate exceeds one sprint. |
| **Testable** | Stored records and displayed results can verify persistence, ownership, prefilling, duplicate prevention, storage failures and behaviour at the ten-item limit. |

*Table 2.4.2 INVEST Criterion for US2 \- Save and Reuse a Favourite Journey*

## **2.5 Given-When-Then (GWT) Acceptance Criteria**

### **2.5.1 US1 Basic Route Search**

### **2.5.2 US2 Fewer Transfer Search**

## **2.6 Definition of Done**

## **2.7 Control of Requirement Changes**

### 



