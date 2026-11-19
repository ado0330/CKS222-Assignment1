**Task 3: Symmetrical Verification & Validation (V-Model Design)**

**3.0 Introduction**

  The V-Model (Verification and Validation Model) is selected to guide the development and testing of the proposed Journey Planning feature for MyRapid PULSE. This model is suitable because it connects each development phase with a corresponding testing phase, ensuring that requirements and design specifications are properly checked throughout the development process.

  For the Journey Planning feature, the V-Model focuses on ensuring that the route search function retrieves accurate journey information, calculates the number of transfers correctly and provides results within the expected response time. By planning testing activities alongside development activities, potential errors can be identified earlier, improving the overall quality and reliability of the proposed feature.

**3.1 Selected Feature and Technical Scope**
   The selected feature is Journey Planning in MyRapid PULSE, an application provided by Prasarana Malaysia Berhad to help public transport users plan their journeys.

   The proposed improvement focuses on two main user stories:
* US1: Basic Route Search - Allows passengers to search for available routes between their selected origin and destionation.
* US2: Fewer-Transfer Search - Allows passengers to find routes with the lowest number of transfer.

   For this audit, the technical scope focuses on the Core Route Database Retrieval and Processing behind the Journey Planning feature. This includes retrieving relevant route, station, stop and service information from the database, calculating the number of transfers, estimating journey duration and sorting the available results according to the selected search option.

   The proposed system should display up to three distinct feasible routes, including the services used, boarding and alighting points, transfer locations, number of transfers and estimated journey duration.

   This scope provides a clear basis for applying the V-Model because both the database operations and route-processing logic can be examined through specific development and testing activities.


**3.2 Customized Symmetrical V-Model**

The customized V-Model contains of two main sides:

* Constructive phases (left side): Focus on identifying requirements, defining specifications and designing the system before implementation.  
* Analytical phase (right side): Focus on verifying and validating the implemented system through different levels of testing.

The proposed phase mapping is as follows: 

| Constructive Phase | Corresponding Analytical Phase |
| :---: | :---: |
| User Requirements Analysis | Acceptance Testing |
| System Requirements Specification | System Testing |
| System Architecture Design | Integration Testing |
| Module/ Detailed Design | Unit Testing |
| Coding/ Implementation | Bottom of the V-Model |

The corresponding phases are aligned horizontally to demonstrate the relationship between development activities and their planned testing activities.

**3.3 Explanation of the Development and Testing Phases**

3.3.1 User Requirements Analysis

During this phase, the development team identifies the needs and expectations of passengers who use the Journey Planning feature.

The main user requirements include:

* Passengers can enter their starting point and destination to search for available public transport journeys.  
* The system provides suitable route options for the selected journey.  
* Passengers can choose a fewer-transfer option to prioritize journeys involving fewer changes between transport services.

Corresponding analytical phase: Acceptance Testing

Acceptance testing evaluates whether the completed Journey Planning feature meets passenger’s expectations and intended needs.

For example, passengers can test whether they can successfully search for a journey and identify an alternative route with fewer transfers. The results help determine whether the feature is suitable for its intended users.

3.3.2 System Requirements Specification

Corresponding analytical phase: System Testing

3.3.3 System Architecture Design

Corresponding analytical phase: Integration Testing

3.3.4 Module/ Detailed Design

Corresponding analytical phase: Unit testing

3.3.5 Coding/ Implementation

**3.4 Verification and Validation**

Verification and validation are two important quality assurance activities in the V-Model. Although they are related, they have different purposes.

| Aspect | Verification | Validation |
| ----- | ----- | ----- |
| Main question | Are we building the product right? | Are we building the right product? |
| Main focus | Technical specifications and implementation correctness | User needs and intended purposes |
| Activities  | Requirements reviews, design inspections and technical testing | User evaluation and acceptance testing |
| Expected outcome | Evidence that the feature follows its expectations  | Evidence that the feature meets passenger’s needs |

For the Journey Planning feature, verification ensures that route-search and transfer evaluation functions follow their defined technical specifications. Validation determines whether the generated journey options are useful and suitable for passengers’ travel needs.

**3.5 Non-Functional Requirement: Performance**

Selected quality attribute: Performance Efficiency \- Time Behaviour

