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
- [4. Scope](#4-scope)
   - [4.1. Customer Journey Map](#41-customer-journey-map)
- [5. Structure](#5-structure)
   - [5.1. Navigation Flow](#51-navigation-flow)
- [6. Skeleton](#6-skeleton)
   - [6.1. Low-Fi Wireframes](#61-low-fi-wireframes)
- [7. Surface](#7-surface)
   - [7.1. Interface Evolution](#71-interface-evolution)
   - [7.2. Results of the Heuristic Evaluation](#72-results-of-the-heuristic-evaluation)
   - [7.3. High Definition Interfaces](#73-high-definition-interfaces)


## 1. Introduction

### 1.1. The Problem

Administrative fragmentation and the lack of a centralized channel for internship monitoring force students and supervisors to navigate multiple platforms and emails. This dispersion creates a high administrative workload, a loss of traceability in report submissions, and delays in hour validation, turning an academic process into a bureaucratic bottleneck that hinders direct communication and the real-time fulfillment of evaluative milestones.

### 1.2. The Solution

The solution is a centralized mobile app designed exclusively for Civil Computer Engineering students at the Universidad de La Frontera (UFRO), which eliminates administrative fragmentation by unifying the entire internship lifecycle into a single, 100% trackable digital environment. To directly address the loss of traceability and bureaucratic bottlenecks, the app integrates a workflow managed through a synchronized dashboard for the three key roles: Students, Company Supervisors, and the University Coordinator. This unified channel not only streamlines the initial connection (or match) between student profiles and IT job offers, but also guarantees real-time visibility over document signing, automatic hour validation, and the fulfillment of evaluative milestones, ensuring transparent and direct communication from start to finish.
  
## 2. Team

- Arturo Avalos
- Benjamin Fernandez
- Christian Gajardo
- Maximiliano Sepulveda 

## 3. Strategy

### 3.1. Value Proposition Canvas

This canvas illustrates the strategic alignment between the platform’s features and the actual needs of the academic community. By identifying the heavy administrative burden and information scattering as primary pain points, the solution focuses on centralizing workflows through automated time logging and unified document management. The value lies in transforming a fragmented, email-dependent process into a transparent, real-time ecosystem that ensures data integrity and reduces the operational friction for students, supervisors, and university coordinators alike.

![Value Proposition Canvas](./Docs/Value-Proposition-Canvas.png)

### 3.2. UIX Persona

This tool allowed us to build detailed profiles of the key stakeholders interacting with the platform, taking into account aspects such as:

 - Demographic data: Age, role (student, supervisor, or coordinator), and location.

 - Goals: What they hope to achieve, such as securing high-impact internships, centralizing student traceability, or providing efficient technical mentoring.

 - Frustrations: Current problems like lack of transparency in job postings, job "ghosting," manual bureaucracy, and administrative chaos.

 - Needs and motivations: The search for a solution that automates validations, provides real-time reporting, and simplifies the institutional agreement process.

<img width="1345" height="754" alt="image" src="https://github.com/user-attachments/assets/955114dd-67b4-4929-86a8-8b9562febcc9" />

<img width="1342" height="752" alt="image" src="https://github.com/user-attachments/assets/90c24fd3-be2b-4a5e-a8b2-b8ecb7b96117" />

<img width="1155" height="644" alt="Diego beñaldo" src="https://github.com/user-attachments/assets/a069fb1e-5eff-4a09-9b39-d40a3bdfca6a" />

The Persona Canvas helped us clearly represent the behaviors and expectations of our users, making it easier to design an experience that directly responds to the need for professionalizing and streamlining the internship ecosystem.

### 3.3. Benchmarking

The current management process relies on three fragmented tools: Google Forms, which collects data across five disconnected stages (forcing users to constantly repeat information in generic formats); Gmail, used as the main communication channel where links and documents get lost in cluttered inboxes, causing uncertainty and delays; and Looker Studio, a static visual dashboard exclusive to the coordinators, which acts like a "black box" leaving the student completely in the dark about their progress and doesn't allow managing or approving requests directly on the screen.

![Fica](./Docs/Benchmark/Apps/fica-ufro-interships.png)

![Fica-i](./Docs/Benchmark/Apps/fica-ufro-intership.png)

For our comparative analysis, we evaluated two major benchmarks used in the university environment: Reqlut and GoSprout. On one hand, Reqlut, which is widely used in Chilean universities, stands out for letting students create their profiles and apply directly, but it completely overlooks tracking the internship once it begins. On the other hand, the international application GoSprout is excellent for tracking hours and showing milestone progress step-by-step with visual indicators, but it lacks a built-in job search engine. Intertrack bridges this gap by combining the best of both worlds into a single mobile application: quick profile-based applications and real-time progress monitoring.

![reqlut](./Docs/Benchmark/Apps/reqlut-interships.png) | ![reqluts](./Docs/Benchmark/Apps/reqlut-intership.png) | ![reqlut](./Docs/Benchmark/Apps/gosprout-home.png)

Meanwhile, the FICA Web (fica.ufro.cl) acts as a public job board. Although in practice it's not the exclusive or most used option for students to find an internship, it is the official channel and follows the faculty's most standardized operating model. Its main drawback is that it mixes job offers from all engineering fields, and when you try to apply, it redirects you to external emails or forms, breaking the workflow. However, its structure is an excellent data source and the perfect base model that we should take, clean up, and improve to integrate it as a search engine 100% focused on the IT sector.

![Benchmark](./Docs/Benchmark/benchmark.png)

To improve what is already in use, we want to Increase the features focused solely on IT. Since the current forms and the university website are for all majors, the idea is to add fields to detail what programming languages or technologies will be used in the internship. We also want to add filters to make the job offers more precise, allowing the student to apply with a single click using their saved profile, instead of filling everything out from scratch.

![Fica-f](./Docs/Benchmark/Apps/fica-ufro-form.png)

We also need to Reduce repetitive paperwork and delays. Currently, the student, their boss, and the professor have to type their name, ID (RUT), and email in five different forms; the goal is to cut down that work. Additionally, we will seek to summarize internship offers that currently have overly long descriptions and lower the waiting times caused when the whole process depends on someone manually checking and replying to an email.

![Fica-i](./Docs/Benchmark/Apps/looker-ev.png)

![Fica-i](./Docs/Benchmark/Apps/looker-status.png)

As for what is missing today, we will Include features that make the process much clearer. Instead of having a dashboard of charts that only coordinators can look at, we will add a visual progress bar so the student knows step-by-step who needs to review their paperwork and what is missing. Along with that, we will integrate evaluations directly into the platform, so both the student and the company boss can submit their grades right there, without having to wait for a link to arrive via email.

Finally, the goal is to Remove the things that only confuse and slow people down. This means filtering out the job offers from other engineering fields that are useless to IT students. We also want to put an end to that feeling of sending a document and not knowing if someone read it, by replacing emails with automatic notifications. In short, the main idea is to stop using four separate apps so that the student, the university, and the company can do everything in a single place.


## 4. Scope

### 4.1. Customer Journey Map

## 5. Structure

### 5.1. Navigation Flow

The navigation architecture is designed as a role-based ecosystem, ensuring a streamlined experience for each user type. Upon authentication, the system branches into three distinct dashboards: Student, Company, and Coordinator, each housing its specific operational tools—from time tracking and rubrics to legal authorizations. This structure minimizes cognitive load by isolating role-specific tasks, while a global Settings module provides unified access to profile and notification management, ensuring a cohesive and efficient user journey across the entire internship lifecycle.

![Value Proposition Canvas](./Docs/AppMap-2.png)

## 6. Skeleton

### 6.1. Low-Fi Wireframes

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

## 7. Surface

### 7.1. Interface Evolution

### 7.2. Results of the Heuristic Evaluation

### 7.3. High Definition Interfaces
