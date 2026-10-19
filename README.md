# Software-Process-in-Software-Engineering
Software Process in Software Engineering. Investigates core process activities, software process models (Waterfall, Incremental, Component Reuse, Agile), and real-world industrial practices comparing Netflix and NASA SLS. Includes technical documentation and presentation slides.

# Software Process in Software Engineering

**Course:** Software Engineering I  
**Author:** Yino Alva
**Instructor:** Dr. Victor Govindaswamy  

---

## Presentation & Media Deliverables

* 📄 **[View Presentation Slides](./Software_Process_in_Software_Engineering.pptx)**

---

## Part 1 – What Is a Software Process?

### 1. Definition of a Software Process
A software process is a structured, organized set of activities required to plan, design, develop, test, and maintain a software system. Rather than writing code in an ad-hoc manner, a software process provides a systematic framework that ensures predictability, quality, and maintainability throughout the system's life cycle.

### 2. Why Software Development Requires an Organized Process
Software engineering differs fundamentally from simple programming. While ad-hoc programming works for small, single-developer projects ("toy applications"), large-scale software systems are built by multi-disciplinary teams, must satisfy complex stakeholder requirements, and must evolve over many years. An organized software process is necessary because:
* **Complexity & Scale:** Modern software involves thousands to millions of lines of code with interacting components.
* **Team Coordination:** Clear structures define who does what, when, and how, preventing duplicated work or conflicting architecture decisions.
* **Cost & Schedule Control:** Structured processes enable cost estimation, resource planning, and progress tracking to avoid schedule overruns.
* **Quality Assurance:** Systematic validation ensures the software is dependable, usable, and secure before release.

### 3. Four Fundamental Software Process Activities
1. **Software Specification (Requirements Engineering):** Defining what the system should do, its operational constraints, and stakeholder requirements.
2. **Software Design and Implementation:** Engineering system architecture, database design, and code logic to produce executable software according to specification.
3. **Software Validation:** Testing and verifying the software to ensure it operates correctly and conforms to customer expectations.
4. **Software Evolution:** Modifying, updating, and extending the software over time to adapt to changing user needs and operational environments.

### 4. Practical Example
Consider developing a **Mobile Banking Application**:
* **Specification:** Engineers gather requirements from bank regulators and customers (e.g., multi-factor authentication, account balance display, wire transfers).
* **Design & Implementation:** Software architects design secure database schemas and REST APIs while mobile developers implement code in Swift/Kotlin.
* **Validation:** Quality assurance (QA) teams run automated security checks, unit tests, and user-acceptance testing (UAT) to confirm transfers occur accurately.
* **Evolution:** Post-launch, the team releases updates to support biometric authentication (Face ID) or new financial regulations.

---

## Part 2 – Software Process Models

### 1. Waterfall Model
* **Basic Idea:** A classic plan-driven model where development flows sequentially through distinct, separate phases.
* **Work Progression:** Progress moves strictly step-by-step: Requirements Definition $\rightarrow$ System/Software Design $\rightarrow$ Implementation & Unit Testing $\rightarrow$ Integration & System Testing $\rightarrow$ Operation & Maintenance. A phase must be formally completed before moving to the next.
* **Appropriate Projects:** Large systems engineering projects, safety-critical systems (e.g., flight control, medical devices), and embedded systems with stable, upfront requirements.

### 2. Incremental Development
* **Basic Idea:** The system is developed as a series of versions (increments), where each increment adds functional capabilities to the previous version.
* **Work Progression:** Specification, design, coding, and testing activities are interleaved rather than sequential. Core features are built first, and subsequent increments expand functionality based on customer feedback.
* **Appropriate Projects:** Business software, consumer web/mobile apps, and dynamic products where requirements change frequently.

### 3. Integration and Configuration (Component-Based Reuse)
* **Basic Idea:** Development focuses on assembling and configuring pre-existing software components, commercial off-the-shelf (COTS) software, or framework APIs rather than building everything from scratch.
* **Work Progression:** Starts with finding available components, refining system requirements to match component capabilities, configuring parameters, and integrating them into the system architecture.
* **Appropriate Projects:** Enterprise applications (ERP systems), e-commerce platforms, and web services leveraging standardized cloud APIs.

### 4. Plan-Driven Development
* **Basic Idea:** An approach where all process activities are planned in advance, and progress is measured against this explicit, detailed plan.
* **Work Progression:** Extensive upfront planning, detailed architectural design, formal milestone reviews, and strict change control boards govern progression.
* **Appropriate Projects:** Large software systems, critical systems, government contracts, and highly regulated industries where compliance and safety are mandatory.

### 5. Agile Development
* **Basic Idea:** An iterative approach emphasizing rapid release cycles, customer collaboration, and flexibility to adapt to change over following a rigid plan.
* **Work Progression:** Development occurs in short iterations (sprints). Cross-functional teams work on prioritized backlog items, delivering functioning software updates frequently.
* **Appropriate Projects:** Startup products, SaaS applications, mobile platforms, and competitive consumer markets.

---

## Part 3 – Waterfall Model

### 1. Major Phases of the Waterfall Model
* **Requirements Definition:** System goals, services, and operational constraints are established through consultation with stakeholders and documented in detail.
* **System and Software Design:** Establishes the overall system architecture and defines software abstractions and relationships.
* **Implementation and Unit Testing:** Software design is realized as a set of programs or units, which are individually tested against specifications.
* **Integration and System Testing:** Individual units are integrated and tested as a complete system to ensure software requirements are met.
* **Operation and Maintenance:** The system is deployed and put into practical use. Maintenance involves fixing bugs, improving implementation, and enhancing system services as new requirements emerge.
![Waterfall Process Model](./Images/Water_Fall_Model.jpg)

### 2. Why Waterfall is Plan-Driven
Waterfall is categorized as a plan-driven process because all activities (schedule, requirements, and system architecture) are explicitly planned and documented upfront before implementation begins. Progress is measured directly against the formal project plan.

### 3. Role of Documentation and Phase Completion
Because different teams often handle sequential phases, detailed documentation serves as the main communication bridge. Formally completing and signing off on each phase ensures requirements and architecture are fully validated before committing resources to downstream development.

### 4. Impact of Requirements Changes Mid-Development
If requirements change after development has started, previous phases must be reopened and reworked (e.g., re-architecting, re-writing code, and re-executing unit tests). This makes mid-development changes extremely costly and disruptive to project timelines.

---

## Part 4 – Incremental Development

### 1. Concept of Incremental Development
Incremental development breaks down software into manageable versions (increments), where each increment delivers a specific subset of complete system functionality.

### 2. Interleaving of Process Activities
Unlike Waterfall's distinct linear stages, specification, design, implementation, and testing activities are conducted concurrently during each increment. Requirements for upcoming increments are refined while current increments are actively being developed.

### 3. Importance of Customer Feedback
Customers receive early releases of working software and provide feedback based on actual usage rather than static spec documents. This direct feedback guides feature priorities for subsequent increments.

### 4. Cost Reduction for Requirements Changes
Because increments are small and modular, changes in requirements affect only current or future increments. This drastically reduces the total volume of code that must be rewritten compared to modifying a monolithic Waterfall build.

![Incremental Development Model](./Images/Incremental_Development_Model.jpg)

---

## Part 5 – Integration and Configuration

### 1. Reuse-Based Software Development
Modern software development frequently relies on integrating pre-built software components, off-the-shelf packages, and framework APIs rather than writing every module from scratch.

### 2. Process Stages in Component Reuse
1. **Requirements Specification:** Initial high-level requirements are defined.
2. **Software Discovery & Evaluation:** Developers search repositories for components matching system needs.
3. **Requirements Refinement:** Original requirements are modified to align with available component capabilities.
4. **Configuration / Adaptation:** Components are configured and parameterized for the target system.
5. **Integration:** Components and custom glue code are integrated into a single operating architecture.

### 3. Advantages and Limitations
* **Advantage:** Accelerates time-to-market, reduces development effort, and leverages pre-tested, reliable code.
* **Limitation:** Loss of control over system evolution. Third-party vendor updates or deprecated APIs can force unexpected system refactoring.
