# SupaWorkers – Final Fall Design Report (CS 5001)

## Team Name and Advisor

**Team SupaWorkers**  
- Jubin Shaikh – Computer Science – shaikhjn@mail.uc.edu  
- Namra Ankoliya – Computer Science – ankolina@mail.uc.edu  
- Krish Patel – Computer Science – patel7kt@mail.uc.edu  

**Faculty Advisor:** Devang Patel  
**Industry Advisor:** Devang Patel, Infosense Global

---

## Project Abstract 

Secure online marketplace that connects hirers with nearby workers for short-term jobs. Users register, post or apply for tasks, and exchange messages through web and mobile interfaces. The system emphasizes strong authentication, protected data storage, and admin monitoring so that flexible work stays convenient, fair, and safe.

---

## Table of Contents

1. [Team Names and Project Abstract](#team-name-and-advisor)  
2. [Project Description](#project-description-assignment-2)  
3. [User Stories and Design Diagrams](#user-stories-and-design-diagrams-assignment-4)  
   - [User Stories](#user-stories)  
   - [Design Diagrams D0, D1, D2](#design-diagrams-level-0-level-1-and-level-2)  
   - [Description of Diagrams](#description-of-the-diagrams)  
4. [Project Tasks and Timeline](#project-tasks-and-timeline-assignments-5-6)  
   - [Task List](#task-list)  
   - [Timeline](#timeline)  
   - [Effort Matrix](#effort-matrix)  
5. [ABET Concerns Essay](#abet-concerns-essay-assignment-7)  
6. [PPT Slideshow](#ppt-slideshow-assignment-8)  
7. [Self-Assessment Essays](#self-assessment-essays-assignment-3)  
8. [Professional Biographies](#professional-biographies-assignment-1)  
9. [Budget](#budget)  
10. [Appendix](#appendix)

---

## Project Description (Assignment 2)

**File:** [`Project Description.md`](Project%20Description.md)

Our project is a secure full-stack web and mobile marketplace that connects businesses needing short-term workers with people seeking flexible shift-based employment. The design emphasizes authentication, session management, database security, and compliance with data protection and employment regulations.

Key technologies: React Native front end, FastAPI (or Node/Express equivalent) back end, and a cloud-hosted database for scalability.

---

## User Stories and Design Diagrams (Assignment 4)

### User Stories

**File:** [`User_Stories.md`](User_Stories.md)

The user stories cover the main roles in SupaWorkers:

- Hirers post tasks with descriptions, budgets, and timeframes to quickly find matching workers.  
- Workers browse and filter nearby tasks by category, pay, and date to accept best-fit jobs.  
- Hirers review worker profiles and prior ratings to select reliable workers.  
- Workers receive real-time notifications for new tasks and messages.  
- Admins monitor listings and reports to keep the marketplace safe and remove fraud/spam.

### Design Diagrams: Level 0, Level 1 and Level 2 

**File:** [`Design_Diagrams.pdf`](Design_Diagrams.pdf)

- **D0 – Context Diagram:** Shows hirers posting tasks, the SupaWorkers marketplace system processing them, and workers browsing and accepting tasks. Focus is on main inputs and outputs between users and the system.  
- **D1 – Major Subsystems:** Breaks the system into Auth & Profiles, Job Posting & Management, Search & Matching, Messaging & Notifications, Admin & Moderation, and the Database. It highlights the modular architecture and subsystem dependencies.  
- **D2 – Detailed Task Lifecycle:** Follows a job from hirer UI form submission through backend validation, storage, worker discovery, matching, and finally messaging via a real-time gateway (WebSocket/push) and database tables for tasks, skills, and messages.

### Description of the Diagrams

- The **context diagram (D0)** defines system boundaries and clarifies that only hirers and workers interact directly with the marketplace; all business logic remains inside the SupaWorkers system.  
- The **subsystem diagram (D1)** explains how we separate concerns: authentication, job workflow, matching, communication, and admin operations, all backed by a central database.  
- The **detailed workflow diagram (D2)** documents the journey of a task, ensuring every step (post, store, discover, match, notify, chat) has a responsible component and data store.

---

## Project Tasks and Timeline (Assignments 5–6)

### Task List

**File:** [`Tasklist.md`](Tasklist.md)

Tasks are assigned by role:

- **Jubin (PM/Security):** Requirements, admin console, usability testing, DB scalability checks, security validation (SQLi prevention, input validation, rate limiting), QA, bug fixes, and final documentation.  
- **Namra (Frontend):** Profile management, employer job posting UI, worker application UI, job search & filters, notification integration, UI/UX refinement, and mobile deployment.  
- **Krish (Backend):** Database schema design, secure registration with OTP and hashing, JWT-based login, API implementations, Swagger documentation, and backend deployment strategy.

### Timeline

**File:** [`Assignment6.pdf`](Assignment6.pdf)

The timeline covers Weeks 1–11:

1. Repo setup and requirements  
2. Database schema design  
3. User authentication and registration  
4. Employer job posting  
5. Worker applications  
6. Notification system  
7. Admin console  
8. Security validation  
9. Usability testing  
10. Final integration and documentation  

Each task has start/end dates and associated deliverables (e.g., ERD, Auth module, dashboards, security test results, final demo).

### Effort Matrix

The effort matrix allocates the percentage of work per task and per team member. For example:

- Requirements: Jubin 40%, Namra 30%, Krish 30%  
- DB Schema: Krish 60%, Jubin 20%, Namra 20%  
- Security Validation: Jubin 60%, Namra 20%, Krish 20%  

Assuming ~5–6 hours/week across 10+ weeks, these distributions justify **at least 45 hours of effort for each team member**, spread across requirements, implementation, testing, documentation, and coordination.

---

## ABET Concerns Essay (Assignment 7)

**File:** [`Constraint Essay.pdf`](Constraint%20Essay%20(1).pdf)

The essay discusses key constraints on SupaWorkers:

- **Economic:** Zero-cost budget relying on open-source tools (MongoDB, Node.js, React) and university hosting, limiting use of paid APIs and large-scale cloud services.  
- **Ethical:** Fair and inclusive job matching, avoiding bias and exploitation, transparency about algorithms and data use.  
- **Security:** Strong input validation, encryption, and rate limiting to protect sensitive credentials and job data from attacks like SQL injection and session hijacking.  
- **Social:** Promotes equitable access to temporary work, while remaining usable for users with limited digital literacy.  

---

## PPT Slideshow (Assignment 8)

**File:** [`CS5001_Presentation.pdf`](CS5001_Presentation%20(1).pdf)

The presentation includes:

- Team members and advisors  
- Expanded project abstract and goals  
- Core user stories and system overview  
- Summary of design diagrams (D0–D2)  
- Constraints mapped to security, economic, ethical, and social dimensions  
- Project progress, division of work, and expected accomplishments  
- Planned demo features such as secure login, job posting/applying, and admin monitoring  

---

## Self-Assessment Essays (Assignment 3)

**Files:**

- [`Individual Capstone Assessment - Jubin Shaikh`](Individual%20Capstone%20Assessment%20(1).docx)  
- (Team contract also part of Assignment 3; see below.)

Jubin’s assessment reflects on:

- Preparation from courses such as WAPH, Computer Networks, AI, and Cloud Computing  
- Co-op experience at Infosense Global (full-stack dev, REST APIs, Git, agile teamwork)  
- Motivation to build a secure, real-world-impact platform  
- Approach to dividing work, applying secure coding, and evaluating personal contributions  

---

## Professional Biographies (Assignment 1)

> If you already have separate `Professional_Biography_*.md` files from Assignment 1, link them here. Otherwise, you can paste brief bios similar to the summaries below.

- **Jubin Shaikh – Project Manager / Security & Testing Lead**  
  Computer Science major with experience in full-stack development and web security through co-op work and WAPH. Focused on secure architecture, testing, and coordination for SupaWorkers.

- **Namra Ankoliya – Frontend Lead**  
  Computer Science major specializing in UI/UX and modern frontend frameworks. Responsible for design consistency, accessibility, and smooth user flows for hirers and workers.

- **Krish Patel – Backend Lead**  
  Computer Science major with interest in API design, databases, and scalable cloud services. Leads backend architecture, data modeling, and performance for the marketplace.

---

## Budget

At this stage, our project has **no direct monetary expenses**.

- **Software/Services:**  
  - Open-source tools (React/React Native, Node.js or FastAPI, MongoDB/Postgres, Git, VS Code) – $0  
  - University-provided hosting and development environments – treated as in-kind support.

- **Donated/Provided Items:**  
  - Advisor time and guidance from Infosense Global (Devang Patel) – non-monetary professional support.  

If future deployment requires paid cloud hosting or premium APIs, we will document those projected costs separately.

---

## Appendix

### References and Links

- Code Repository: _(insert GitHub repo URL here)_  
- Design diagrams and timelines: see [`Design_Diagrams.pdf`](Design_Diagrams.pdf) and [`Assignment6.pdf`](Assignment6.pdf).  
- Course materials and security best practices: WAPH slides, OWASP Top 10, and MongoDB/Postgres documentation (links to be added as used).

### Team Contract

**File:** [`Team Contract Draft-Signed`](Team%20Contract%20Draft-Signed%20(1).docx)

The contract documents:

- Project focus on secure full-stack web development  
- Meeting schedule (weekly plus informal Discord check-ins)  
- Initial roles (PM/Security, Frontend Lead, Backend Lead)  
- Agreement on respect, punctuality, shared responsibilities, and conflict resolution practices  

### Evidence of Effort (Toward 45+ hours per member)

- Week-by-week milestones and deliverables in [`Assignment6.pdf`](Assignment6.pdf) and [`Tasklist.md`](Tasklist.md) map each member to concrete tasks.  
- Activities include requirements, design, implementation, testing, documentation, and presentation preparation.  
- Combined weekly workload across 10+ weeks exceeds 45 hours per student.

---

_Last updated: Fall 2025_
