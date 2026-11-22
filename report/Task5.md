# **Task 5: Process Tailoring (Münch's 4 Ps) & Human Factors Governance** 

## **5.1 Tailoring with Münch's 4 Ps**

**5.1.1 Introduction**  
Software development methodologies should be selected according to the characteristics and requirements of a particular project rather than applying a single methodology universally. Münch's Process Tailoring framework provides a systematic approach to selecting and adapting software development processes based on four contextual factors: Problem, Project, People and Product.  
For this case study, the framework is applied to the MyRapid PULSE mobile application developed by Prasarana Malaysia Berhad. MyRapid PULSE provides public transportation-related services, including journey planning, live bus tracking, interactive rail maps, lifestyle information and promotional features. These functionalities aim to help commuters plan their journeys and access relevant transportation information conveniently.   
The application requires consideration of changing user requirements, integration of different functionalities, collaboration among relevant stakeholders and the delivery of reliable information. Therefore, this section evaluates the four contextual factors to determine an appropriate software development methodology for the continuous development and maintenance of MyRapid PULSE.

## **5.1.2 Problem**

The Problem factor examines the complexity, novelty and volatility of the constraints associated with the software problem being addressed. It considers how clearly the problem is understood, how frequently requirements may change and the uncertainties that developers must manage during development.

MyRapid PULSE aims to address the difficulties commuters encounter when accessing public transportation information and planning their journeys. Through its journey planner, live bus tracker and interactive rail map, the application provides information intended to help users make more informed travel decisions.

However, several challenges may arise when developing and improving the application as shown in Table 1\.

| Problem characteristic | Explanation |
| :---- | :---- |
| Changing user requirements | Commuters may request new functionalities or improvements based on their travelling experiences and expectations. |
| Real-time information accuracy | Users depend on accurate bus location and arrival-time information to plan their journeys effectively. |
| Diverse user requirements | Different users, such as daily commuters and occasional travellers, may have different expectations regarding navigation and accessibility. |
| Changing transportation information | Route information, schedules and service updates may require modifications to ensure that the information presented remains relevant. |

*Table 1: Possible Challenges When Developing MyRapid PULSE*

These challenges are supported by publicly available user feedback. For example, some Google Play reviewers have reported application crashes and inaccurate bus arrival estimates. 

*Figure 2 & Figure 3: Google Play Reviews Reporting Frequent Clash of MyRapid PULSE*

*Figure 4: Google Play Review Reporting Inaccurate Public Transportation Time of Arrival Prediction*

The developer has acknowledged these concerns and indicated that the feedback would be shared with the relevant team for investigation and improvement.

*Figure 5: Prasarana Malaysia Berhad’s Reply Regarding the Complaint in FIgure 3*

Such feedback demonstrates the importance of continuously identifying and addressing user requirements throughout the application's development lifecycle.

#### **5.1.2.1 Problem Factor’s Implications for Process Selection**

The characteristics of the Problem factor indicate that an iterative and flexible development approach is appropriate. Scrum is recommended because it allows development teams to continuously refine requirements based on user feedback and changing priorities.

For example, when users report inaccurate bus arrival information, the development team can carry out the following steps:

1. Collect and analyze the reported user feedback.  
2. Record the required improvements in the product backlog.  
3. Prioritize the improvements according to their importance.  
4. Develop the selected improvements within a sprint.  
5. Review the completed functionality and obtain further feedback.

This iterative approach allows MyRapid PULSE to be improved progressively without requiring the entire application to undergo a complete redevelopment whenever user requirements change.

Therefore, Scrum is considered suitable for addressing the complexity and volatility of the problems associated with the continuous improvement of MyRapid PULSE.

### **5.1.3 Project**

The Project factor examines the characteristics and constraints of the software development project, including team size, team distribution, budget, schedule and overall project complexity. These factors influence the resources required, the coordination of development activities and the level of process formality needed.

MyRapid PULSE is a mobile application that consists of several interconnected functionalities, including journey planning, live bus tracking, interactive rail maps, lifestyle information and promotional features. The development and maintenance of these functionalities involve different technical requirements and may require coordination between multiple software components.

Table 6 below describes the project characteristics of MyRapid PULSE.

| Project characteristic | Explanation |
| :---- | :---- |
| Multiple functionalities | The application contains different features that must operate consistently within a single mobile application. |
| Integration complexity | Journey planning and live bus tracking depend on the availability and coordination of relevant transportation information. |
| Continuous maintenance | Existing functionalities require ongoing bug fixes, performance improvements and compatibility updates. |
| Development scheduling | New features and improvements need to be prioritized and delivered within manageable development cycles. |
| Cross-platform considerations | The application is available on Android and iOS, requiring consideration of compatibility across supported mobile platforms. |

*Table 6: The Project Characteristics of MyRapid PULSE*

The presence of multiple functionalities increases the importance of coordination and testing. For example, improvements to the journey-planning functionality should not negatively affect other related features. Similarly, modifications to the bus-tracking functionality should be tested to ensure that the application continues to display transportation information correctly.

#### **5.1.3.1 Project Factor’s Implications for Process Selection**

A combination of Scrum and the V-Model is recommended to address the project's development and quality assurance requirements.

Scrum can be used to organize development activities into manageable sprints, allowing the team to prioritize different application functionalities and deliver improvements incrementally. Meanwhile, the V-Model can provide a structured approach to verification and validation by establishing corresponding testing activities throughout the development lifecycle.

This combination allows the project to maintain flexibility in feature development while ensuring that appropriate testing activities are performed before new improvements are released.

Therefore, Scrum supported by the V-Model is considered suitable for managing the multiple functionalities, integration requirements and continuous maintenance activities associated with MyRapid PULSE.

## **5.1.4 People**

The People factor examines the human characteristics of the software development team, particularly their technical skills, team cohesion, working culture and staff turnover. These characteristics influence how effectively individuals collaborate, communicate and perform their assigned development activities.

The development and maintenance of MyRapid PULSE requires collaboration among individuals with different technical skills, responsibilities and areas of expertise. As proposed in Task 1, the reorganised development team consists of five specialised roles, including Product Owner, Scrum Master, Tech Lead, Developer and QA Engineer. The Table 8 below shows the responsibilities of each role.

| Role | Responsibilities |
| :---- | :---- |
| **Product Owner** | Prioritises the product backlog, defines requirements and makes release decisions.  |
| **Scrum Master** | Facilitates Scrum activities, monitors sprint progress and removes obstacles.  |
| **Tech Lead** | Oversees technical standards, resolves technical disagreements and approves code merging.  |
| **Developer** | Implements application features, performs static analysis and reviews other developers' code.  |
| **QA Engineer** | Plans and conducts system and acceptance testing to ensure software quality.  |

*Table 8: The Responsibilities of Roles in Development Team*

#### **5.1.4.1 People Factor’s Implications for Process Selection**

A hybrid Scrum and V-Model approach is recommended because Scrum provides a collaborative working structure through sprint planning, regular progress discussions and sprint reviews. The Product Owner can communicate changing commuter requirements and prioritise the backlog, while the Scrum Master helps resolve development obstacles. Developers, the Tech Lead and QA Engineer can also communicate regularly to identify technical issues and testing requirements early.

Meanwhile, the V-Model provides a structured approach to verification and validation. The Tech Lead oversees technical reviews and merge approval, while the QA Engineer independently verifies and validates the application against its requirements. This helps prevent development decisions from being merely based on delivery speed and ensures that changes are evaluated before release.


## **5.1.4 Product**
