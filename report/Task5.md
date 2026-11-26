# **Task 5: Process Tailoring (Münch's 4 Ps) & Human Factors Governance** 

## **5.1 Tailoring with Münch's 4 Ps**

## **5.1.1 Problem**

The Problem factor examines the complexity, novelty and volatility of the constraints associated with the software problem being addressed. 

Problem characteristic | Explanation |
| :---- | :---- |
| Changing user requirements | Commuters may request new functionalities or improvements based on their travelling experiences and expectations. |
| Real-time information accuracy | Users depend on accurate bus location and arrival-time information to plan their journeys effectively. |
| Changing transportation information | Route information, schedules and service updates may require modifications to ensure that the information presented remains relevant. |

*Table 1: Possible Challenges When Developing MyRapid PULSE*

These challenges are supported by publicly available user feedback. For example, some Google Play reviewers have reported application crashes and inaccurate bus arrival estimates. 

*Figure 2-4: Selected Google Play Feedback*

*Figure 5: Prasarana Malaysia Berhad’s Response*

#### **5.1.1.1 Problem Factor’s Implications on Process Selection**

The Problem factor indicates that an iterative and flexible development approach is appropriate. Therefore, Scrum is recommended because it allows development teams to continuously refine requirements based on user feedback and changing priorities. This iterative approach allows MyRapid PULSE to be improved progressively without requiring the entire application to undergo a complete redevelopment whenever user requirements change.
For example, when users report inaccurate bus arrival information, the development team can carry out the following steps:

### **5.1.2 Project**

The Project factor considers team size, schedule, complexity, resources and coordination. 

| Project characteristic | Explanation |
| :---- | :---- |
| Multiple functionalities | Journey planning, bus tracking, rail maps and other features must work consistently together. |
| Integration complexity | Journey planning and live tracking depend on relevant transportation data being available and coordinated. |
| Continuous maintenance | Existing functionalities require ongoing bug fixes, performance improvements and compatibility updates. |
| Development scheduling | New features and improvements need to be prioritized and delivered within manageable development cycles. |
| Cross-platform considerations | The application is available on Android and iOS, requiring consideration of compatibility across supported mobile platforms. |

*Table 6: The Project Characteristics of MyRapid PULSE*

#### **5.1.2.1 Project Factor’s Implications for Process Selection**

A combination of Scrum and the V-Model is recommended. Scrum can be used to organize development activities into manageable sprints, allowing the team to prioritize different application functionalities and deliver improvements incrementally. Meanwhile, the V-Model can provide a structured approach to verification and validation by establishing corresponding testing activities throughout the development lifecycle. This combination allows the project to maintain flexibility in feature development while ensuring that appropriate testing activities are performed before new improvements are released.

## **5.1.3 People**

The People factor examines the human characteristics of the software development team, particularly their technical skills, team cohesion, working culture and staff turnover. The proposed five-role structure from Task 1 distributes responsibilities across product management, process facilitation, technical leadership, development and quality assurance.

| Role | Responsibilities |
| :---- | :---- |
| **Product Owner** | Prioritises the product backlog, defines requirements and makes release decisions.  |
| **Scrum Master** | Facilitates Scrum activities, monitors sprint progress and removes obstacles.  |
| **Tech Lead** | Oversees technical standards, resolves technical disagreements and approves code merging.  |
| **Developer** | Implements application features, performs static analysis and reviews other developers' code.  |
| **QA Engineer** | Plans and conducts system and acceptance testing to ensure software quality.  |

*Table 8: The Responsibilities of Roles in Development Team*

#### **5.1.3.1 People Factor’s Implications on Process Selection**

A hybrid Scrum and V-Model approach is recommended because Scrum provides a collaborative working structure through sprint planning, regular progress discussions and sprint reviews. The Product Owner can communicate changing commuter requirements and prioritise the backlog, while the Scrum Master helps resolve development obstacles. Developers, the Tech Lead and QA Engineer can also communicate regularly to identify technical issues and testing requirements early. Meanwhile, the V-Model provides a structured approach to verification and validation. The Tech Lead oversees technical reviews and merge approval, while the QA Engineer independently verifies and validates the application against its requirements. This helps prevent development decisions from being merely based on delivery speed and ensures that changes are evaluated before release.

## **5.1.4 Product**
The Product factor examines the characteristics and quality requirements of the software being developed including product criticality, reliability, lifespan and security requirements.
 Quality attribute | Importance to MyRapid PULSE |
| :---- | :---- |
| Reliability | The application should operate consistently without frequent crashes or unexpected failures. |
| Accuracy | Bus locations, arrival estimates and journey information should be accurate to support users' travel decisions. |
| Performance | Features such as journey planning and live bus tracking should respond within an acceptable time.

*Table 9: Important Quality Attributes of MyRapid PULSE*

#### **5.1.4.1 Product Factor’s Implications on Process Selection**

The V-Model is recommended because it emphasizes systematic verification and validation throughout the software development lifecycle. It helps ensure that product requirements are translated into corresponding testing activities. This allows potential defects to be identified earlier and reduces the likelihood of unresolved problems reaching users.

### **5.1.5 Proposed Hybrid Software Development Methodology**

Based on the four factors, a hybrid methodology combining Scrum and the V-Model is proposed. Scrum provides iterative development and responsiveness to changing commuter requirements, while the V-Model contributes structured verification and validation.

#### **5.1.5.1 Scrum**

Development activities are organized into short sprints. Requirements and improvement requests are maintained in a product backlog and prioritized according to their importance. For example, if users report problems with the Live Bus Tracker, the development team can prioritize the required improvements and implement them during upcoming sprints. Scrum addresses the Problem and People factors by allowing requirements to evolve through feedback while encouraging communication and collaboration among development team members. 

#### **5.1.5.2 V-Model**

The V-Model is proposed to strengthen the quality assurance process of MyRapid PULSE. Unlike an approach that postpones testing until development is completed, the V-Model establishes corresponding testing activities alongside the development and specification phases. For example, when improving the Journey Planner, the development team should establish the expected functionality and corresponding testing requirements before implementation. For example, unit testing, integration testing, system testing and acceptance testing should be carried out. The V-Model addresses the Project and Product factors by providing systematic testing activities for the application's interconnected functionalities and quality requirements.

## **5.2 Tuckman's Team Dynamics and Fist-of-Five Governance**
### **5.2.1 Current Stage of Team Development**

Based on the group's progress, its current development stage is assessed as Storming. At this stage, members may have different opinions and interpretations of the assignment requirements. These differences can create disagreements when making decisions. For example, when considering the proposed Scrum and V-Model hybrid methodology, a member was concerned about the complexity of combining two different approaches. 

### **5.2.2 Fist-of-Five Consensus**

To establish agreement on the proposed hybrid methodology for the MyRapid PULSE application, our group adopts the Fist-of-Five consensus method.

#### **5.2.2.1 Consensus discussion and conflict resolution**

During the vote, Cecilia Se assigned a score of 2 out of 5 because she was concerned that combining Scrum and the V-Model might complicate the development process because the two methodologies have different approaches to managing development activities. She also questioned whether the group could coordinate sprint activities while maintaining the corresponding testing activities.

In response, the group clarified that the two methodologies would serve complementary purposes rather than operate as two separate development lifecycles. Scrum would be used as the main framework for managing development activities, while relevant V-Model verification and validation practices would be incorporated into the development and testing process. For instance, testing requirements for a particular feature could be considered during its planning and implementation rather than being postponed until the end of development. The member then indicated that the explanation addressed the concern and revised the vote from 2 to 4. This discussion allowed the group to clarify the intended implementation of the hybrid approach and consider the potential difficulties before reaching a decision.

*Figures 10-12: WhatsApp discussion showing the initial concern, clarification and member confirmation*

#### **5.2.2.2 Fist-of-Five Voting Results**

Group member | Initial vote  | Final vote |
| :---: | :---: | :---: |
| Khaw Zhi Xin | 5 | 5 |
| Seah Xin Yi | 4 | 4 |
| Lim Zhi Ying | 5 | 5 |
| Cecilia Se | 2 | 4 |
| Kung Ker Mian | 5 | 5 |

*Table 13: Fist-of-Five voting results*  

#### **5.2.2.3 Final decision**
Based on the actual voting results and subsequent discussion, the group agreed on adopting the Scrum and V-Model hybrid methodology for the MyRapid PULSE application. The discussion demonstrates the importance of considering individual concerns before finalising a group decision. The unedited WhatsApp group chat screenshot showing all five members' votes and the discussion resolving any votes below 3 is attached as evidence of the Fist-of-Five consensus process.

*Figure 14: Initial Vote in WhatsApp ·		     Figure 15: Final Vote in WhatsApp*  
