**Course:** Software Engineering I  
**Author:** Yino Alva
**Semester:** Fall 2026
**Instructor:** Dr. Victor Govindaswamy  

---
Youtube Videos:
https://youtu.be/zG_2VjeATvY?si=o_Vs9oikju10-G0Z
https://youtu.be/h9rMgdPAUWw?si=GdnY4hquEvIoOyUr
https://youtu.be/JIROyfUgI2k?si=AnzQYFBKq8bIq9gh
--- 
💼 **LinkedIn Post:** [View Promotional Post on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7518171391901237249/)
---
# Software-Process-in-Software-Engineering
Software Process in Software Engineering. Investigates core process activities, software process models (Waterfall, Incremental, Component Reuse, Agile), and real-world industrial practices comparing Netflix and NASA SLS. Includes technical documentation and presentation slides.

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
  
---
## Part 6 – Software Process Activities

### 1. Software Specification / Requirements Engineering
* **Role:** Establishes the boundary conditions, capabilities, and system constraints.
* **Contribution:** Prevents teams from building the wrong system by aligning technical output with stakeholder needs.

### 2. Software Design and Implementation
* **Role:** Transforms system specifications into an operational software executable.
* **Contribution:** Software design structures the internal system architecture, database models, and interface definitions, while implementation writes clean, maintainable code.

### 3. Software Validation
* **Role:** Evaluates software via unit testing, integration testing, system testing, and user-acceptance testing (UAT).
* **Contribution:** Ensures that the software operates accurately, satisfies security requirements, and meets specified expectations before deployment.

### 4. Software Evolution
* **Role:** Updates, patches, and refactors software in response to changing environments, bug discoveries, and user requests.
* **Contribution:** Software is dynamic; evolution ensures that software remains useful, secure, and operational over its commercial lifecycle.

---

## Part 7 – Coping with Change

### 1. Inevitability of Change in Software Projects
Software operates within dynamic business, technical, and human environments. Changes arise from shifting market demands, evolving consumer preferences, corporate restructuring, regulatory updates, hardware changes, and newly discovered security vulnerabilities.

### 2. Software Prototyping
A prototype is an initial version of a software system used to demonstrate concepts, evaluate design options, and discover requirements.
* **Clarifying Requirements:** Users test prototypes to discover missing features or clarify ambiguous specifications early in development.
* **Evaluating Design Decisions:** Architects use prototypes to test performance bottleneck issues or evaluate different UI/UX layouts.

### 3. Incremental Delivery
Incremental delivery supplies working software functionality directly to end-users in successive releases.
* **Early Customer Value:** Customers receive functional software sooner, allowing them to gain business value early rather than waiting years for a full release.
* **Impact of Change:** Managing change iteratively isolates cost, schedule, testing, and documentation impacts to specific increments rather than destabilizing the entire software platform.

---

## Part 8 – Two Real-World Software Engineering Applications

### Application 1: E-Commerce Platform (Shopify)
* **Company & System:** Shopify Inc. — Global E-Commerce Merchant Platform
* **System Function:** Powers 2M+ online merchant storefronts, handling product catalog navigation, checkout, payment gateways, and inventory tracking.
* **Development Approach:** Agile / DevOps / Continuous Delivery / Component Reuse
* **4 Core Process Activities:**
  * **Specification:** Dynamic backlog prioritized via merchant feedback, A/B testing, and market trends.
  * **Design & Implementation:** API-first microservices architecture; integrates pre-built third-party components (Stripe, PayPal, carrier shipping APIs).
  * **Validation:** Automated CI/CD pipelines, unit/integration testing suites, and canary deployments to ensure zero downtime.
  * **Evolution:** Continuous daily releases to production without interrupting active storefront sales.
* **Process Flow:**
  `Merchant Feedback → Agile Backlog → Microservice/API Coding → Automated CI/CD Testing → Continuous Deployment → Live Telemetry`

---

### Application 2: Healthcare Software (Epic Systems)
* **Company & System:** Epic Systems Corporation — EpicCare Electronic Health Record (EHR) System
* **System Function:** Manages electronic patient medical records, physician notes, prescription orders, and clinical workflows across hospital networks.
* **Development Approach:** Plan-Driven / Safety-Critical Waterfall Hybrid
* **4 Core Process Activities:**
  * **Specification:** Exhaustive upfront specifications driven by regulatory standards (HIPAA, FDA) and clinical safety protocols.
  * **Design & Implementation:** Modular clinical architecture with strict access control security models and data integrity baselines.
  * **Validation:** Months of multi-tier clinical simulation, security audits, and formal verification before code freeze.
  * **Evolution:** Scheduled quarterly/annual institutional releases managed by hospital Change Control Boards (CCB) to protect patient safety.
* **Process Flow:**
  `Regulatory/Safety Specs → Formal Architecture → Secure Module Coding → Clinical Simulation & Audits → Scheduled Institutional Rollout`

---

## Part 9 – 14-Category Comparative Matrix

| Category | Application 1 (Shopify) | Application 2 (Epic Systems) |
| :--- | :--- | :--- |
| **Company/Organization** | Shopify Inc. | Epic Systems Corporation |
| **Software/Application** | Shopify E-Commerce Storefront Infrastructure | EpicCare Electronic Health Record (EHR) System |
| **Primary Users** | Online merchants, store managers, and global shoppers | Doctors, nurses, pharmacists, and medical staff |
| **Development Approach** | Agile / DevOps / Microservices Architecture | Plan-Driven / Safety-Critical Waterfall Hybrid |
| **Requirements Process** | Dynamic product backlog driven by merchant usage analytics & A/B testing | Formal upfront specifications based on HIPAA rules & FDA regulations |
| **Development** | API-first microservices & pre-built third-party component integration | Modular clinical data engine with strict role-based access control |
| **Testing/Validation** | Automated CI/CD pipelines, unit suites, and canary deployments | Multi-tier clinical simulation, data integrity testing & HIPAA audits |
| **Deployment** | Continuous deployment (multiple updates pushed live per day) | Scheduled institutional release cycles (quarterly or annual updates) |
| **Maintenance/Updates** | Real-time cloud background updates without storefront downtime | Institutional patches governed by Change Control Board (CCB) oversight |
| **Customer Feedback** | Real-time site telemetry, merchant analytics, and live experimentation | Clinical advisory boards, hospital system feedback, and audit reports |
| **Waterfall Characteristics** | Core payment security baselines & financial data compliance rules | Sequential phase gates, exhaustive documentation, and signed-off specs |
| **Agile/Incremental Characteristics** | Rapid storefront feature updates and short sprint releases | Internal iterative engineering sprints prior to formal release freezes |
| **Major Advantage of Approach** | Rapid time-to-market and continuous scaling for merchants | Uncompromising patient safety, zero fault tolerance & regulatory compliance |
| **Major Challenge** | Handling massive real-time traffic spikes (e.g., Black Friday sales) | High cost, extreme complexity, and risk of modifying baseline core code |

---

## Part 10 – Advantages, Disadvantages, and Appropriate Use

### 1. Waterfall Model
* **Advantages:** Clear project milestones, detailed design documentation, predictable planning.
* **Disadvantages:** Inflexible to mid-project changes; working software delivered late in the process.
* **Appropriate Use:** Safety-critical, heavily regulated software (Healthcare EHRs, aerospace flight controls).

### 2. Incremental / Agile Models
* **Advantages:** Fast time-to-market, flexible to changing requirements, early user value.
* **Disadvantages:** Less predictable long-term schedules; requires continuous team coordination.
* **Appropriate Use:** Dynamic commercial applications (E-commerce storefronts, consumer web/mobile apps).

### 3. Why Use Hybrid Models?
* Allows companies to keep core engines plan-driven for safety/compliance while using agile iterations for user interfaces.

---

## Part 11 – Key Learnings & Summary

* **No "One-Size-Fits-All" Process:** Software engineering processes must be tailored to the system's specific domain, risk profile, and target audience.
* **Safety & Regulation Drive Plan-Driven Processes:** Systems where errors risk patient safety or legal non-compliance rely on structured, documented phases.
* **Market Competition Drives Agile Processes:** Systems where customer expectations change quickly rely on iterative updates and continuous feedback.

---

## References

1. **Govindaswamy, V.** *Software Engineering Lecture 1: Basics of Software Engineering Parts 1–3*. Course Presentation Slides.
2. **Govindaswamy, V.** *Software Engineering Lecture 2: Software Processes Parts 1–2*. Course Presentation Slides.
3. **Shopify Engineering.** *How Shopify Delivers Software at Scale: Continuous Delivery & Microservices*. Shopify Tech Blog. Available at: [https://engineering.shopify.com](https://engineering.shopify.com)
4. **Shopify Engineering.** *Continuous Modernization & Infrastructure Scale for Enterprise Commerce*. Shopify Tech Blog, 2026. Available at: [https://www.shopify.com/enterprise/blog/continuous-modernization](https://www.shopify.com/enterprise/blog/continuous-modernization)
5. **Shopify Engineering.** *IT Transformation & Continuous Feature Delivery Benchmarks*. Shopify Tech Blog, 2026. Available at: [https://www.shopify.com/enterprise/blog/it-transformation](https://www.shopify.com/enterprise/blog/it-transformation)
6. **Epic Systems Corporation.** *Safety-Critical System Validation and Healthcare Compliance Standards*. Epic Technical Documentation. Available at: [https://www.epic.com](https://www.epic.com)
7. **Epic Systems Corporation.** *Epic EHR Security Features & Healthcare Regulatory Compliance Standards*. Digital Health Engineering, 2026. Available at: [https://digitalhealth.folio3.com/blog/epic-ehr-security-features/](https://digitalhealth.folio3.com/blog/epic-ehr-security-features/)
8. **Accountable HQ.** *Epic HIPAA Compliance: Administrative, Technical Controls, and Change Oversight*. Security & Compliance Guide, 2026. Available at: [https://www.accountablehq.com/post/epic-hipaa-compliance-requirements-security-features-and-best-practices](https://www.accountablehq.com/post/epic-hipaa-compliance-requirements-security-features-and-best-practices)
