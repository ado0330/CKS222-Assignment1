**Task 3: Symmetrical Verification & Validation (V-Model Design)**

**3.0 Introduction**

   The V-Model  (Verification and Validation Model) is selected to guide the development and testing of the proposed Journey Planning feature for MyRapid PULSE. This model is suitable because it connects each development phase with a corresponding testing phase, ensuring that requirements and design specifications are properly checked throughout the development process.

   For this feature, the V-Model focuses on ensuring that passengers can successfully search for routes between their selected origin and destination and save frequently used origin-destination pairs as favourites for future use. It also ensures that the system retrieves accurate journey information and stores favourite routes correctly. By planning testing activities alongside development activities, potential errors can be identified earlier, improving the overall quality and reliability of the proposed feature.

## **3.1 Selected Feature and Technical Scope**

   The selected feature for this audit is **Journey Planning** in MyRapid PULSE, an application provided by Prasarana Malaysia Berhad to help public transport users plan their journeys.

The proposed improvement focuses on two main user stories:

* **US1: Basic Route Search** – Allows passengers to search for available routes between their selected origin and destination.  
* **US2: Save Favourite Route** – Allows passengers to save an origin-destination pair as a favourite for future use.

   For this audit, the technical scope focuses on the **Core Route Database Retrieval and Favourite Route Management** behind the Journey Planning feature. This includes retrieving relevant route, station, stop and service information from the database, saving selected origin-destination pairs as favourites and retrieving saved favourites for future use.

    The proposed system should display available journey information based on the passenger’s selected origin and destination. It should also allow passengers to have frequently used origin-destination pairs and access them later without having to enter the same locations again.

    This scope provides a clear basis for applying the V-Model because the database operations and route-processing functions can be examined through specific development and testing activities.

**3.3 Overview of the V-Model**

   The V-Model (Verification and Validation Model) is a software development model that extends the traditional Waterfall approach by linking each development phase with a corresponding testing phase. It follows a V-shaped structure, where the left side focuses on requirements analysis and system design, the bottom represents implementation, and the right side focuses on testing and validation.

    Each development phase has a corresponding testing phase to ensure that the system is developed according to its requirements and design specifications. Testing activities are planned early during development rather than waiting until implementation is completed. This helps identify potential issues earlier and ensures that the final system meets both technical requirements and user expectations.

    In this customised V-Model, the development activities on the left side are matched with their corresponding testing activities on the right side. The implementation phase is positioned at the bottom of the V.

**3.4 Customised V-Model for Journey Planning**

The following V-Model is customised for the proposed Core Route Database Retrieval and Favourite Route Management feature in MyRapid PULSE.

| Development Phase (left side) | Corresponding Testing Phase (right side) |
| ----- | ----- |
| User Requirements Analysis \- Identify passenger needs for searching routes and saving favourite origin-destination pairs. | Acceptance Testing \- Confirm that passengers can successfully search for routes and save and reuse their favourite origin-destination pairs. |
| System Requirements Specification \- Define functional requirements for route retrieval, favourite saving and retrieval, together with NFRs and database constraints. | System Testing \- Test the complete feature, including route searching and favourite route management, against the specified requirements.  |
| System Architecture Design \- Design the database structure and relationships between passengers, routes, stations, stops and saved favourites. | Integration Testing \- Check whether the database and route-processing components work correctly together, including saving and retrieving favourites. |
| Detailed Design \- Specify the processing logic for route retrieval, saving favourite pairs, checking existing favourites and retrieving saved pairs. | Unit Testing \- Test individual functions, such as route retrieval, saving favourites and retrieval, saving favourites and retrieving favourite pairs. |
| Coding/ Implementation \- Develop the database operations and processing functions based on the approved design. | Coding/ Implementation \- Located at the bottom of the V-Model, where the planned feature is implemented before the corresponding testing activities are carried out. |

## 

## **3.3 Explanation of the Development and Testing Phases**

### **3.3.1 User Requirements Analysis**

During this phase, the development team identifies the needs and expectations of passengers who use the Journey Planning feature.

The main user requirements include:

* Passengers can enter their origin and destination to search for available public transport routes.  
* The system provides suitable route options based on the selected origin and destination.  
* Passengers can save an origin-destination pair as a favourite for future use.  
* Passengers can access their previously saved favourite origin-destination pairs without entering the same locations again.

**Corresponding analytical phase: Acceptance Testing**

Acceptance testing evaluates whether the completed Journey Planning feature meets passengers' expectations and intended needs.

For example, passengers can test whether they can successfully search for routes between their selected locations, save an origin-destination pair as a favourite and access the saved favourite later. The results help determine whether the feature is suitable for its intended users.

### **3.3.2 System Requirements Specification**

In this phase, the identified user requirements are translated into detailed functional and non-functional requirements.

Examples of functional requirements include:

* The system must receive the selected origin and destination from the passenger.  
* The system must retrieve and display suitable route information based on the selected locations.  
* The system must allow passengers to save an origin-destination pair as a favourite.  
* The system must retrieve previously saved favourite pairs associated with the passenger's account.

A non-functional requirement may specify that route search results and saved favourite origin-destination pairs should be retrieved within 2 seconds under normal operating conditions.

**Corresponding phase: System Testing**

System testing evaluates the complete feature against its specified requirements. For example, testers verify whether passengers can search for routes, save favourite origin-destination pairs and retrieve their saved favourites correctly. They also examine whether the system handles invalid or incomplete inputs appropriately and meets the specified response-time requirement.

### **3.3.3 System Architecture Design**

During this phase, the development team defines the overall architecture and the interactions between the relevant components.

For this proposed feature, the architecture may include the passenger interface, backend processing component and database. The database design should support the storage and retrieval of route information and favourite origin-destination pairs.

The design also defines the relationships between passenger accounts, origin and destination records, and saved favourite records to ensure that each favourite is associated with the correct passenger.

**Corresponding phase: Integration Testing**

Integration testing checks whether the connected components communicate and exchange information correctly.

For example, testers verify whether the passenger interface can send search requests to the backend, whether the backend retrieves the correct route information from the database and whether favourite origin-destination pairs can be saved and retrieved successfully.

### **3.3.4 Detailed Design**

This phase focuses on the detailed design of individual modules and database structures. It specifies the attributes and relationships required to support the Journey Planning feature.

For example, a favourite route record may contain a unique favourite ID, passenger ID, origin ID and destination ID. The design also specifies the processing logic for retrieving available routes, saving favourite pairs, checking for duplicate favourites and retrieving previously saved favourites.

These details help ensure that the feature follows a consistent structure before implementation.

**Corresponding phase: Unit Testing**

Unit testing checks individual modules and functions independently.

For example, the development team can test the route retrieval function to ensure that it returns the appropriate route information for the selected locations. The favourite-saving function can also be tested to ensure that it stores the correct origin-destination pair, while the favourite retrieval function should return the saved records associated with the correct passenger.

### **3.3.5 Coding / Implementation**

During this phase, developers translate the approved designs and specifications into executable code. The route-search logic, database operations and favourite route management functions are implemented according to the established requirements.

The implementation includes developing functions to retrieve route information, save favourite origin-destination pairs and retrieve previously saved favourites.

After implementation, the feature proceeds through the planned testing activities, including unit testing, integration testing, system testing and acceptance testing, to ensure that it meets the specified requirements and passenger expectations.

**3.4 Verification and Validation Activities** 

    Verification and validation are important activities in the V-Model because they ensure that the proposed feature is developed correctly and meets user expectations.

   **Verification** checks whether the system is being developed according to its specified requirements and design. It focuses on reviewing development outputs and checking whether they satisfy the stated specifications.

    **Validation** checks whether the completed system meets the actual needs and expectations of its intended users. It focuses on whether the feature provides the expected functionality and useful results.

For the Journey Planning feature, the activities can be applied as follows: 

| Aspect | Verification | Validation |
| :---: | ----- | ----- |
| Route Retrieval | Review the database queries and check whether the retrieval logic follows the specified requirements. | Confirm that passengers receive relevant routes for their selected origin and destination. |
| Favourite Saving | Review the saving logic and check whether favourite records are stored with the correct passenger, origin and destination identifiers. | Confirm that passengers can save their frequently used origin-destination pairs successfully. |
| Favourite Retrieval | Check whether the retrieval logic follows the specified database relationships and passenger identification rules. | Confirm that passengers can access their previously saved favourites for future journey planning. |
| Duplicate Prevention | Review and test the database constraints or application logic used to prevent duplicate favourite records. | Confirm that passengers do not encounter repeated entries for the same saved origin-destination pairs. |

These activities ensure that the proposed feature follows its technical specifications while also providing the expected outcome for passengers.

**3.5 Verification and Validation of the Selected NFR and Technical Constraint**

    Apart from functional requirements, the proposed feature must also satisfy a non-functional requirement (NFR) and a technical constraint to ensure its performance and data reliability.

**3.5.1 Non-Functional Requirement (NFR): Response Time**

**Proposed Requirement:** The Journey Planning feature should return route search results and retrieve saved favourite-origin-destination pairs within 2 seconds under normal operating conditions.

This requirement is important because passengers expect to receive journey information and access their saved favourites without unnecessary delays.

* **Verification:** Conduct performance testing to measure the response time of route searching and favourite retrieval. Review the test results to determine whether both operations meet the specified 2-second response-time requirement.  
* **Validation:** Evaluate whether passengers can obtain route search results and access their saved favourites within an acceptable waiting time.

**3.5.2 Technical Constraint: Database Referential Integrity**

**Proposed Constraint:** The database must maintain valid relationships between passenger accounts and their saved favourite origin-destination pairs through appropriate primary key and foreign key constraints.

This constraint ensures that each favourite record is associated with a valid passenger account and valid origin and destination records.

* **Verification:** Review the database design and conduct database integrity tests to ensure that primary key and foreign key constraints are correctly defined and enforced. Test whether invalid references are rejected.  
* **Validation:** Test the favourite-saving and retrieval functions to confirm that passengers can save and access their own favourite origin-destination pairs correctly.

   

