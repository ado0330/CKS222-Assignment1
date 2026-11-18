**Task 3: Symmetrical Verification & Validation (V-Model Design)**

**3.0 Introduction**

   MyRapid PULSE, developed by Pasarana Malaysia Berhad, is a mobile application that provides public transport information and journey planning services. Its Journey Planner helps passengers plan their daily trips using public transport services.

   For this task, the selected feature is Journey Planning, focusing on two functions: normal route search and a fewer-transfer option. Normal route search allows passengers to search for available journeys between their starting point and destination. The fewer-transfer option provides an alternative that prioritizes journeys requiring fewer changes between transport services.

   This feature is treated as a core database-related feature because its route-planning functions depend on accessing and processing transport information, such as station stops, routes, services and schedules. A customized symmetrical V-model is proposed to guide its development and testing.

   The V-model establishes a relationship between each development phase and its corresponding testing phase. This ensures that verification and validation activities are considered throughout the development activities.

**3.1 Justification for Selecting the V-model**

   The Journey planning feature involves processing passenger’s search requests and retrieving suitable route information based on their selected starting point and destination. It also needs to consider the connections between transport services when generating alternative journeys with fewer transfers.

   The feature therefore requires accurate route information, consistent database records and efficient search processing. Incorrect route information or unsuitable transfer combinations may result in passengers receiving misleading journey recommendations.

  The V-Model is suitable because it provides a structural development approach in which testing activities are planned alongside requirements and design activities. Each constructive phase has a corresponding analytical phase, allowing the development team to identify potential problems and evaluate the completed feature systematically.

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

