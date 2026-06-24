# InterTrack
UX design repository for a centralized internship management platform, focusing on streamlining administrative workflows, tracking progress, and enhancing the interaction between students and supervisors through user-centered interfaces.

## Index
- [1. Introduction](#1-introduction)
   - [1.1. The Problem](#11-the-problem)
   - [1.2. The Solution](#12-the-solution)
- [2. Team](#2-team)
- [3. Strategy](#3-strategy)
   - [3.1. Value Proposition Canvas](#31-value-proposition-canvas)
   - [3.2. UIX Persona](#32-uix-persona)
   - [3.3. Benchmarking](#33-benchmarking)
- [4. Structure](#4-structure)
   - [4.1. Navigation Flow](#41-navigation-flow)
- [5. Skeleton](#5-skeleton)
   - [5.1. Low-Fi Wireframes](#51-low-fi-wireframes)
- [6. Surface](#6-surface)
   - [6.1. Interface Evolution](#61-interface-evolution)
   - [6.2. Results of the Heuristic Evaluation](#62-results-of-the-heuristic-evaluation)
   - [6.3. Accessibility Considerations](#63-accessibility-considerations)
   - [6.4. High Definition Interfaces](#64-high-definition-interfaces)


## 1. Introduction

### 1.1. The Problem

Administrative fragmentation and the lack of a centralized channel for internship monitoring force students and supervisors to navigate multiple platforms and emails. This dispersion creates a high administrative workload, a loss of traceability in report submissions, and delays in hour validation, turning an academic process into a bureaucratic bottleneck that hinders direct communication and the real-time fulfillment of evaluative milestones.

### 1.2. The Solution

The solution is a centralized mobile app designed exclusively for Civil Computer Engineering students at the Universidad de La Frontera (UFRO), which eliminates administrative fragmentation by unifying the entire internship lifecycle into a single, 100% trackable digital environment. To directly address the loss of traceability and bureaucratic bottlenecks, the app integrates a workflow managed through a synchronized dashboard for the three key roles: Students, Company Supervisors, and the University Coordinator. This unified channel not only streamlines the initial connection (or match) between student profiles and IT job offers, but also guarantees real-time visibility over document signing, automatic hour validation, and the fulfillment of evaluative milestones, ensuring transparent and direct communication from start to finish.
  
## 2. Team

- Arturo Avalos – Project Manager: Responsible for the overall coordination and planning of the project. Ensures that deadlines are met, organizes team activities, coordinates meetings, and leads presentations. Also supervises the integration of all deliverables to maintain consistency throughout the project.
- Benjamin Fernandez – UX Research Analyst: Responsible for conducting user research and analyzing collected information. Develops UX Personas, Customer Journey Maps, and the Value Proposition Canvas. Identifies user needs, pain points, and opportunities to improve the proposed solution.
- Christian Gajardo – UI/UX Designer: Responsible for designing the user experience and user interface. Creates low-fidelity and high-fidelity prototypes, designs navigation flows, and ensures visual consistency across all screens. Applies usability and accessibility principles throughout the design process.
- Maximiliano Sepulveda – Documentation and Repository Manager : Responsible for organizing and maintaining the project repository. Ensures that all documentation is complete, properly structured, and written in English. Manages deliverables, annexes, and supporting materials while maintaining quality standards and version control.

## 3. Strategy

### 3.1. Value Proposition Canvas

This canvas illustrates the strategic alignment between the platform’s features and the actual needs of the academic community. By identifying the heavy administrative burden and information scattering as primary pain points, the solution focuses on centralizing workflows through automated time logging and unified document management. The value lies in transforming a fragmented, email-dependent process into a transparent, real-time ecosystem that ensures data integrity and reduces the operational friction for students, supervisors, and university coordinators alike.

![Value Proposition Canvas](./Docs/Value-Proposition-Canvas.png)

### 3.2. UIX Persona

This tool allowed us to build detailed profiles of the key stakeholders interacting with the platform, taking into account aspects such as:

 - Demographic data: Age, role (student or supervisor), and location.

 - Goals: What they hope to achieve, such as securing high-impact internships, centralizing student traceability, or providing efficient technical mentoring.

 - Frustrations: Current problems like lack of transparency in job postings, job "ghosting," manual bureaucracy, and administrative chaos.

 - Needs and motivations: The search for a solution that automates validations, provides real-time reporting, and simplifies the institutional agreement process.

<img width="1345" height="754" alt="image" src="https://github.com/user-attachments/assets/955114dd-67b4-4929-86a8-8b9562febcc9" />

<img width="1920" height="1080" alt="Brainstorming User Persona Minimalista Azul" src="https://github.com/user-attachments/assets/896b7511-600e-41f2-ac28-dcb7fe24037f" />

<img width="1155" height="644" alt="Diego beñaldo" src="https://github.com/user-attachments/assets/a069fb1e-5eff-4a09-9b39-d40a3bdfca6a" />

The Persona Canvas helped us clearly represent the behaviors and expectations of our users, making it easier to design an experience that directly responds to the need for professionalizing and streamlining the internship ecosystem.

### 3.3. Benchmarking

The current university management process relies on three disconnected tools. **Google Forms** collects data across five isolated stages, forcing users to constantly repeat the exact same information in generic formats. **Gmail** functions as the main communication channel, where crucial links and documents get lost in cluttered inboxes, causing severe uncertainty and delays. Finally, **Looker Studio** acts like a "black box"—it is a static visual dashboard exclusive to coordinators that leaves the student completely in the dark regarding their progress and lacks any functionality to manage or approve requests directly on screen.

![Fica](./Docs/Benchmark/Apps/fica-ufro-interships.png)

![Fica-i](./Docs/Benchmark/Apps/fica-ufro-intership.png)

On the other hand, the **FICA Web** (fica.ufro.cl) acts as a public job board. Although in practice it is not the exclusive or most used platform for students to find an internship, it remains the official channel and follows the faculty's most standardized operating model. Its main drawback is that it mixes job offers from all engineering fields, and attempting to apply redirects the user to external forms or emails, breaking the workflow. However, its baseline structure is an excellent data source and the perfect foundation to clean up, improve, and integrate as a built-in search engine 100% focused on the IT sector.

To understand how to solve this fragmentation, we evaluated two major benchmarks utilized in the university and professional environment: **Reqlut** and **GoSprout**.

![reqlut](./Docs/Benchmark/Apps/reqlut-interships.png) | ![reqluts](./Docs/Benchmark/Apps/reqlut-intership.png) | ![reqlut](./Docs/Benchmark/Apps/gosprout-home.png)

* **Reqlut:** Widely adopted by Chilean universities, it stands out for providing an excellent user experience by allowing students to build modular profiles and apply to job openings directly with a single click. However, it completely overlooks the follow-up and tracking of the internship once the work placement actually begins.
* **GoSprout:** This international application excels at hour tracking and milestone monitoring step-by-step through clear visual indicators (such as radial charts and status labels), but it lacks an integrated job search engine or placement matching.

**Intertrack** bridges this gap by combining the best of both worlds into a single mobile application: quick profile-based applications and real-time progress monitoring.

Based on the diagnostic of the current tools and the analyzed benchmarks, we defined our user-centered design strategy using four action pillars:

![Benchmark](./Docs/Benchmark/benchmark.png)

#### Increase
We aim to increase features focused exclusively on the IT sector. Since current university forms and websites target all engineering majors, we will add specific fields to detail the programming languages, tech stacks, and frameworks that will be used during the internship. We will also increase search precision through advanced technical filters, allowing students to apply with a single click using their saved profile.

![Fica-f](./Docs/Benchmark/Apps/fica-ufro-form.png)

#### Reduce
It is critical to reduce repetitive paperwork and administrative delays. Currently, the student, the company supervisor, and the coordinator must manually type their names, National ID (RUT), and emails across five different forms; Intertrack will automate data persistence. Additionally, we will reduce overly long, unstructured job descriptions through standardized templates and minimize the waiting times caused by the process depending on manual email replies.

#### Include
We will include key features currently missing from the UFRO ecosystem to eliminate uncertainty. Instead of a Looker Studio dashboard that only coordinators can access, we will include an interactive, visual progress bar so students know exactly who has their paperwork and what step is missing. Furthermore, we will integrate a native evaluation module so both supervisors and students can submit grades directly within the app without waiting for external links via email.

![Fica-i](./Docs/Benchmark/Apps/looker-ev.png)

![Fica-i](./Docs/Benchmark/Apps/looker-status.png)

#### Eliminate
Finally, we will eliminate elements that confuse and slow down users. This means completely filtering out job offers from other engineering fields that provide no value to computer science students. We will also eliminate the lack of feedback when submitting documents by replacing traditional email communication with automated in-app notifications. In short, we eliminate the need for four separate platforms so that all three key roles can seamlessly interact in one centralized workspace.

Synthetic Comparative Table

The following matrix consolidates the mandatory baseline dimensions alongside domain-specific criteria tailored to our IT internship scope:

| Evaluation Dimension | Current UFRO Process (Forms + Gmail) | Competitor A: Reqlut | Competitor B: GoSprout | Our Proposed Solution: **Intertrack** |
| :--- | :--- | :--- | :--- | :--- |
| **Target Audience** | UFRO Engineering students, supervisors, and coordinators. | Broad university student base and multi-industry recruiters. | Vocational trainees, program managers, and field supervisors. | **Computer Science & IT students, tech companies, and academic coordinators.** |
| **Main Value Proposition** | Manual validation of academic graduation requirements. | Multi-purpose job-board and applicant matching portal. | Administrative compliance and on-the-job hours auditing. | **End-to-end mobile automation, technical matching, and real-time step monitoring.** |
| **Onboarding Flow** | Disconnected. Starts manually via external Google Forms links. | Multi-step personal resume builder with manual text inputs. | Private registration via institutional invitation link. | **Instant integration leveraging pre-existing UFRO intranet credentials.** |
| **Primary UI Navigation** | No layout pattern. Fragmented web-links and emails. | Bottom tabs paired with classic hierarchical text list details. | Bottom navbar combined with a central persistent FAB. | **Intuitive bottom navigation combined with a linear step-by-step milestone timeline.** |
| **Domain Dimension 1: Technical Stack/IT Filters** | **None.** Job board mixes all engineering fields randomly. | **None.** Uses generic keyword search bars with no tech filter fields. | **None.** Focuses purely on general vocational hour-tracking metrics. | **Advanced tags filtering by programming languages, frameworks, and roles.** |
| **Domain Dimension 2: 3-Way Sync Compliance** | **Fragmented.** Done manually by typing data into 5 separate forms. | **Partial.** Connects application but lacks post-hire tools. |  **Full.** Real-time automated verification loops. | **Centralized. In-app document synchronization for Student, Boss, and University.** |

---

Findings and Design Decisions

Analyzing the domain standards revealed critical design patterns that **Intertrack** will adopt or systematically redefine:

1. **Adoption of Collapsible Modular Profiles (from Reqlut):** We will implement a structured, persistent profile framework to eliminate data duplication. Students input personal and academic details once, which then automatically populates future validation steps.
2. **Adoption of Radial Progress Indicators (from GoSprout):** To dismantle the current "black box" experience of Looker Studio, we are adopting explicit status tracking labels and visual indicators. This ensures students get clear feedback on exactly who is reviewing their paperwork.
3. **Rejection of Complex Corporate Dashboard Data (from GoSprout):** We are purposefully omitting complex financial graphs or multi-tiered corporate apprentice wage trackers to maintain a minimalist, accessible interface centered around UFRO's academic requirements.

**Intertrack** effectively bridges this market gap by merging the search and matching capabilities of **Reqlut** with the visual tracking and administrative feedback loop of **GoSprout** into a single mobile environment.

## 4. Structure

### 4.1. Navigation Flow

The navigation architecture is designed as a role-based ecosystem, ensuring a streamlined experience for each user type. Upon authentication, the system branches into two distinct dashboards: Student and Company, each housing its specific operational tools. This structure minimizes cognitive load by isolating role specific tasks, while a global Settings module provides unified access to profile and notification management, ensuring a cohesive and efficient user journey across the entire internship lifecycle.

![Value Proposition Canvas](./Docs/AppMap-2.png)

## 5. Skeleton

### 5.1. Low-Fi Wireframes

The wireframes are focused on 3 different user roles, who share emails and collaborate when starting, advancing, and finalizing an internship:

#### 1. Intern (Student)
* View the general status of all their internships.
* View internship details and history tracking.
* Browse internship offers to apply, or register an external internship.

![My Interships](./Docs/Low-Fi/Mis-Practicas.png) 

![My Interships](./Docs/Low-Fi/Oferta-Practicas.png)


#### 2. Academic Coordinator
* Authorize internships.
* View detailed information about students currently enrolled in internships.
* Evaluate completed internships.

![coordinators](./Docs/Low-Fi/coordinator.png)

#### 3. Supervisors
* Post internship opportunities for students.
* Track the progress and status of their interns.
* Evaluate at the end of the internship and close the cycle.

![supervisor](./Docs/Low-Fi/supervisor.png)

All Low-Fi Wireframes can be seen here: [Figma](https://www.figma.com/design/xn8Vwx0Js6ZoTdfAgoNmRJ/Wireframes?node-id=0-1&p=f&t=0ggaOzU6UwhOb6P5-0)

## 6. Surface

### 6.1. Interface Evolution

The final version of InterTrack was developed through several design iterations, evolving from the initial low-fidelity wireframes into a complete high-fidelity prototype. The objective of these iterations was to improve usability, simplify administrative processes, and provide a more intuitive experience for both students and company supervisors.

Throughout the design process, feedback received during presentations, internal reviews, and benchmark analysis was incorporated into the final proposal.

### Main Design Changes

The transition from the initial wireframes to the final prototype introduced several improvements focused on usability and information clarity.

| Area | Initial Design | Final Design |
| :--- | :--- | :--- |
| User Roles | Three-role architecture | Simplified into Student and Company workflows |
| Internship Monitoring | Basic information display | Progress tracking and internship status visibility |
| Job Opportunities | Simple listings | Match percentage and detailed offer information |
| Evaluations | Basic forms | Structured evaluation workflow |
| Internship Management | Fragmented information | Centralized internship overview |
| Authentication | Login only | Password recovery and verification flow |
| Interface Consistency | Independent screens | Unified design system and navigation |

---

### Authentication Flow Evolution

The initial design only considered a traditional login screen with too much information.

During subsequent iterations, the authentication process was optimized to improve:

- Password recovery.
- Verification code validation.
- Password reset flow.
- Improved form hierarchy and visual feedback.

These changes provide a more complete onboarding and account recovery experience.

#### FINAL LOGIN STUDENT VS LOW-FI LOGIN STUDENT

<img width="737" height="615" alt="image" src="https://github.com/user-attachments/assets/90deee80-0dc4-4b5f-a021-b6051b1018ae" />

#### FINAL REGISTER COMPANY VS LOW-FI COMPANY

<img width="581" height="618" alt="image" src="https://github.com/user-attachments/assets/d8c9663c-2d5d-4f48-8632-98981494acce" />

### Internship Tracking Evolution

One of the main problems identified during the research was the oversaturation and mismanagement of size in the sections that students experienced when trying to understand the current state of their internship process.

To address this issue, the final design redesign:

- Internship progress visualization.
- Hours tracking.
- Validation status indicators.
- Evaluation status indicators.
- Historical internship records.

This information is now accessible directly from the internship dashboard.

#### FINAL OFFERS SCREEN VS LOW-FI OFFERS SCREEN

<img width="814" height="834" alt="image" src="https://github.com/user-attachments/assets/0a910d4d-6e84-4af7-8a18-28a5e8b85054" />

### Company Management Evolution

The company workflow underwent one of the most significant redesigns.

Originally, company interactions were distributed across several independent views.

The final design centralizes:

- Internship publications.
- Applicants.
- Accepted interns.
- Internship monitoring.
- Evaluations.

This redesign reduces navigation effort and allows supervisors to access the most important actions from a single workflow.

#### FINAL COMPANY FLOW VS LOW-FI COMPANY FLOW
<img width="567" height="595" alt="image" src="https://github.com/user-attachments/assets/aaa6a235-00dd-422f-b47f-21c9980173c7" />
<img width="591" height="775" alt="image" src="https://github.com/user-attachments/assets/79f11618-8416-4b0f-a7b4-8538aeb3d26c" />


### Evaluation Process Evolution

The evaluation process was refined to improve clarity and structure.

The final version incorporates:

- Weighted evaluation criteria.
- Dedicated descriptions for each category.
- Final score calculation.
- General comments section.
- Pending evaluation management.

This structure creates a more transparent evaluation experience for both students and supervisors.

#### FINAL EVAKUATION FLOW VS LOW-FI EVALUATION FLOW
<img width="574" height="758" alt="image" src="https://github.com/user-attachments/assets/22405b92-8e6e-4002-841d-339e0dc388eb" />

## 6.2. Results of the Heuristic Evaluation

To validate the usability of the final prototype, a heuristic review based on Nielsen's usability principles was conducted.

The objective was to identify potential usability issues and verify whether the final design effectively addressed the main problems detected during the research phase.

### Evaluation Summary

| Heuristic | Observation | Implemented Improvement |
| :--- | :--- | :--- |
| Visibility of System Status | Students had difficulty understanding internship progress. | Added progress indicators and status labels. |
| Match Between System and Real World | Administrative processes were difficult to understand. | Internship terminology was simplified and organized. |
| Consistency and Standards | Similar actions appeared differently across screens. | Standardized navigation, forms and cards. |
| Recognition Rather Than Recall | Users needed to remember process stages. | Added persistent progress information and visual indicators. |
| User Control and Freedom | Important actions required multiple steps. | Reduced navigation depth and centralized actions. |
| Aesthetic and Minimalist Design | Some views contained excessive information. | Improved hierarchy and grouped related information. |

### Main Issue #1: Internship Visibility

Students lacked visibility regarding internship status, completed hours, and pending requirements.

#### Solution

The final design introduced progress indicators and status monitoring that provide immediate feedback regarding the internship lifecycle.

### Main Issue #2: Administrative Complexity

Company supervisors needed quick access to intern information and evaluations.

#### Solution

The redesign centralized internship management into dedicated sections for applicants, accepted interns, and evaluations.

### Main Issue #3: Fragmented Information

The internship process involved multiple independent screens with limited contextual information.

#### Solution

Information architecture was reorganized around complete workflows, reducing the need for users to switch between unrelated sections.

### Heuristic Evaluation Outcome

The evaluation confirmed that the redesign significantly improved:

- Process transparency.
- Navigation consistency.
- Information discoverability.
- Administrative efficiency.
- Progress visibility.

---

### 6.3. High Definition Interfaces

#### 1. Student Interfaces

The student workflow includes:

- Internship opportunities.
- Opportunity details.
- Internship tracking.
- Progress monitoring.
- Hour registration.
- Document management.
- Self-evaluation.
- User profile management.

The design prioritizes visibility of system status and quick access to the most relevant information.

#### Login student
<img width="367" height="776" alt="image" src="https://github.com/user-attachments/assets/bb1092ae-efe2-413c-aa9a-2534819d2614" />

#### Recover password
<img width="1102" height="754" alt="image" src="https://github.com/user-attachments/assets/4659c2f5-8d7c-47e6-8637-5f4cd5930793" />

#### Practical offers
<img width="828" height="821" alt="image" src="https://github.com/user-attachments/assets/44b46127-5206-4015-85ef-77b4312539c4" />

#### My practices
<img width="369" height="793" alt="image" src="https://github.com/user-attachments/assets/70bbbef5-9eae-41b2-b9d0-76e597e49039" />

#### My practice
<img width="922" height="778" alt="image" src="https://github.com/user-attachments/assets/e0861049-2d08-4a10-b198-f1a2805dc81f" />

#### Profile
<img width="382" height="813" alt="image" src="https://github.com/user-attachments/assets/afab9b66-33a1-44d8-84fd-3186061ffaea" />

#### Documents
<img width="285" height="606" alt="image" src="https://github.com/user-attachments/assets/ce1cab6e-6072-426b-97f8-183e89d39ec9" />

#### 2. Company

The company workflow includes:

- Internship publication.
- Applicant management.
- Accepted interns.
- Internship monitoring.
- Performance evaluations.

The interface was designed to simplify internship supervision and reduce administrative effort.

#### Login company
<img width="367" height="776" alt="image" src="https://github.com/user-attachments/assets/bb1092ae-efe2-413c-aa9a-2534819d2614" />

#### Register company
<img width="956" height="663" alt="image" src="https://github.com/user-attachments/assets/80ed2135-e1d4-447f-b7db-b1dce31be6f2" />

#### My posts
<img width="339" height="715" alt="image" src="https://github.com/user-attachments/assets/439515ac-01ba-4dbf-b575-d443adbcfb75" />

#### Search for practitioners
<img width="384" height="818" alt="image" src="https://github.com/user-attachments/assets/be125956-e6a4-40b5-a891-6e0c09101bb9" />

#### My practitioners
<img width="374" height="812" alt="image" src="https://github.com/user-attachments/assets/495c8405-d48e-479e-9ee0-97b516cd6485" />

#### Accepted practitioner
<img width="370" height="786" alt="image" src="https://github.com/user-attachments/assets/fa47db93-3893-4edd-b12c-60c52a0f3307" />

#### Publish offers
<img width="264" height="713" alt="image" src="https://github.com/user-attachments/assets/23f3ad12-1c77-4cd5-9548-d4e72c19492c" />

#### Applicant details
<img width="358" height="769" alt="image" src="https://github.com/user-attachments/assets/53c8ea1a-909f-491d-8786-b2b684d2a7d7" />

#### Practitioner information
<img width="360" height="770" alt="image" src="https://github.com/user-attachments/assets/4b1c746e-7c91-4ee8-8060-09d142df6db1" />

#### Evaluate practitioner
<img width="287" height="766" alt="image" src="https://github.com/user-attachments/assets/60126051-dbb7-4651-afda-7b346a610d77" />

#### Accept practitioners
<img width="690" height="706" alt="image" src="https://github.com/user-attachments/assets/302fa9ed-fe2e-41be-b669-e657c8975ce3" />



## 6.4. Accessibility Considerations

Accessibility considerations were incorporated during the refinement phase of the project.

Although accessibility was not the primary focus of the prototype, some measures were explored to improve usability across different visual conditions.

### Accessibility Improvements Considered

#### Dark Mode Exploration

A dark mode variation was explored for selected interfaces to evaluate readability and visual comfort under low-light conditions.

This approach aimed to:

- Reduce visual fatigue.
- Improve contrast in dark environments.
- Offer an alternative visual experience for users.

Because the project focused primarily on validating functionality and workflows, dark mode was not implemented across every final screen.

### Interface Readability

The prototype also incorporates:

- Clear typography hierarchy.
- Consistent spacing between interface elements.
- Large touch targets for mobile interaction.
- Visual grouping of related information.

These decisions contribute to improving readability and reducing cognitive load.

### DARK MODE EXPLORATION
<img width="644" height="672" alt="image" src="https://github.com/user-attachments/assets/970f2854-6813-47eb-af11-cbcfbd8c73f9" />


---

All high-fidelity frames can be found here: [Figma Design File](https://www.figma.com/design/uBHhHAYdy20HXp4pSSIV6f/InterTrack-UX?node-id=0-1&t=rjMESOzxybi2EGoh-1)

The interactive demo can be accessed here: [Figma Prototype](https://www.figma.com/proto/uBHhHAYdy20HXp4pSSIV6f/InterTrack-UX?node-id=2010-1992&t=toFJ6Q1mfvBwCbwI-1&starting-point-node-id=2010%3A1992)

