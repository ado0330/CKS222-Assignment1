# **Task 4: Lean Waste Auditing & Extreme Programming (XP) Practice Alignment**

# **4.0 Introduction**

For task 4, we chose the CCA103 Student Consultation and Appointment Booking System as our case study because it was developed by a group that included three of our current members during Semester II, 2025/2026. The system allows students to schedule consultation sessions with lecturers or academic advisors based on available time slots. It improves communication and reduces scheduling conflicts by providing a structured platform for managing appointments, notifications and feedback. In fact, we are able to understand and analyze the development of the system based on the generated report, rather than the MyRapid Pulse application that provides limited resources and evidence to the public. In this section, we will figure out the four potential lean wastes and three Extreme Programming (XP) alignment accordingly.

## **4.1 Lean Waste Audit & Remedies**

Lean Software Development is based on maximizing customer value by eliminating waste and optimizing process flow. It is crucial to ensure a structured and cost-effective development process. For the CCA103 Student Consultation and Appointment Booking System, four potential Lean wastes are identified based on the project’s design and proposed development activities. Each waste comes with a brief description, a specific example and a proposed process remedy.

### **4.1.1 Lean Waste 1: Waiting**

Waiting occurs when team members cannot proceed with their work because they are waiting for related information or completed tasks from others. This often happens when there are dependencies across modules. As a result, the member may remain inactive while others are still completing their work, slowing down the development process and creating pressure especially when deadlines are approaching.

In the CCA103 project, the Booking and Appointment Module depends on the Lecturer Availability and Slot Management Module, as an appointment booking requires available consultation slots. For example, the developer responsible for the Appointment Booking Module needs information such as lecturer’s available dates, time slots and booking status before confirming a student’s booking. So in this case, if the Lecturer Availability Module fails to finalize those details on time, the booking developer may not be able to complete its function that displays available slots to students. This could also delay the Notification and Feedback Module because appointment confirmation messages always depend on successful bookings.

To reduce waiting, the team can use GitHub Projects to track tasks and set deadlines. Members should also agree on module interfaces early and use sample data while waiting for other modules to be completed. This allows development to continue without unnecessary delays.

### **4.1.2 Lean Waste 2: Defects**

Defects refer to errors or bugs that escape early detection and cause the system to work incorrectly. These errors may be the result from unclear requirements, incorrect logic or insufficient testing. When defects are discovered late, developers may need extra time to fix and retest the system, increasing the workload, cost and delaying development.

In the CCA103 project, a possible defect would be an overlapping slots booking between two students. For example, Student A and Student B both try to book an appointment with Lecturer C at the same time slot. If the system fails to check and update slots availability, both bookings may be accepted. As a result, the lecturer would have two appointments scheduled at the same time, causing confusion and requiring students to rearrange their appointments. The development team would also need to correct the booking logic and repeat the testing process.

To prevent defects, the team should introduce automated testing to check important booking functions such as preventing duplicate bookings and rejecting unavailable slots. These tests should run whenever the booking function is updated, helping the developers to detect errors early and reduce the need of repeated manual testing.

### **4.1.3 Lean Waste 3: Overproduction (Gold Plating)**

Overproduction occurs when developers create unnecessary features or functionality that customers never requested or actually need. In software development, this is also known as Gold Plating. Other than wasting development time, this wastes also increase non-essential cost and makes the system more complicated to maintain.  
In the CCA103 project, overproduction could occur if developers added an AI-based lecturer recommendation feature even though the original requirements focused mainly on lecturer availability and appointment booking. Developing this additional feature would require extra coding, testing and maintenance effort without providing any essential value to the system’s main purpose. As a result, the team might spend time on this unnecessary feature instead of improving the core booking functions which directly affect our users' experience.

To prevent overproduction, the team can maintain a prioritised backlog so the developers can focus on implementing essential functions that meet user requirements. In addition, requiring approval before developing additional features can prevent unnecessary work and help the team to use its time and  resources more efficiently. For example, any proposed feature should be reviewed by stakeholders based on its necessity and value to users before development begins.

### **4.1.4 Lean Waste 4: Handoffs**

Handoffs occur when work or information is transferred from one team member to another. They become wasteful when important details are missing, unclear or misunderstood during the transfer. In software projects, this happens when different developers work on connected modules but lack effective communication. Poor handoffs can lead to incorrect assumptions and integration problems when combining different modules into a working system.

For example, in our CCA103 system, the Booking Module needs to pass appointment information to Notification Module when a student successfully books a consultation slot. This includes the correct student and appointment details such as student ID, lecturer ID, appointment date, time and booking status. But if the developers do not agree on the required information, the Notification Module may receive incomplete or incorrect data. As a result, students may receive incorrect confirmation messages and affect the lecturer’s schedule. The team would then need to review the connections between modules and correct the integration errors.

To reduce handoff problems, the team should prepare clear interface specifications before developing connected modules. These should describe the required inputs, outputs and data formats so every member understands how information is exchanged. The team can also conduct short joint review sessions when work is transferred between modules and use Pair Programming for functions involving multiple modules. These practices improve communication, reduce misunderstanding and help identify integration problems earlier.

## **4.2 Extreme Programming (XP) Engineering Practices**

Extreme Programming (XP) is an Agile software development approach that focuses on improving code quality, teamwork and continuous feedback. For the expanded CCA103 Student Consultation and Appointment Booking System, three XP practices are proposed to improve code quality and shorten feedback loops.

### **4.2.1 Pair Programming**

### **4.2.2 Test-First Programming (TDD)**

### **4.2.3 Continuous Integration (CI)**

