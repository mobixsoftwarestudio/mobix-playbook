---
layout: post
title: Project Management
---

During the execution of projects, Mobix has a major cycle of Project Management like below:

`(PLANNING -> DAILY -> DEV REVIEW -> DEV DONE -> HOMOLOGATION -> APPROVED ->  PRODUCTION DEPLOY)`

Our Project Manager \(PM\) needs to organize his tasks by the following:

## Tasks Management

We use `Jira` for Project Management. 

We separate the project vision in three perspectives: Roadmap, Backlog and Active Sprint.

### Roadmap

Here is where we put the main vision of the project. Using metrics of Software Engineering and Project Design, we separate the main features in Modules.
Each module has a set of features. Each feature is mapped using the Backlog section.

#### Checklist for Roadmap Implementation

* [x] Map entities for project (business cases) (this needs to be aligned with the UX and Product teams)
* [x] Map a higher vision of project considering modules (this needs to be aligned with the UX and Product teams)
* [x] For each module, consider a set of features (this needs to be aligned with the UX and Product teams)
* [x] For each feature, consider UX/UI, Front End, Back End, QA
* [x] Write down a specific flow for each feature, considering Sequence Diagrams, Alternative Flows, Business Rules, Data Structures and UI link
* [x] Use those features as reference for Sprint Plannings and Client Prioritizations

Your roadmap should look like this:

* Module 1
  * Feature 1
    * Requirements, UI, Test Scenarios
  * Feature 2
    * Requirements, UI, Test Scenarios
* Module 2
  * Feature 1
    * Requirements, UI, Test Scenarios
  * Feature 2
    * Requirements, UI, Test Scenarios

### Backlog

Here we dive deep into our feature details. Each one needs to attend the following fields:

* [x] Description
* [x] Main Flow
* [x] Alternative Flow
* [x] API Structure / API link
* [x] Screens (if needed)
* [x] Tasks
* [x] Test Scenarios
* [x] Story Point

Note: `Main Flow` lists a sequence of steps needed which evolves all the feature objective. The `Alternative Flow` also do the same job, however focusing on behaviors that gravitates around the business rules. We use those two fields for Acceptance Criteria.

### Active Sprint

The Active Sprint sets all features that the team planned to do in our [Sprint Planning](#sprint-planning) cerimony.

Our Active Sprint takes up to 10 business days.

### Methodology

At Mobix we use Scrum Methodology to achieve the goals. Divided by Sprints, we set up expectations with the Team and with the Client to plan and tackle possible challenges that we might need to achieve the goals. As Scrum is an Agile Methodology applied on Software Engineering process, a few events are made with the Team:

#### Sprint Planning

The Team receives the deliverables provided by the PM of the project. At this point, we have the UI requirements documented with the high fidelity prototypes and further recommendations of the Client regarding some prioritizations.

During the planning, we analyze each Feature and set up complexity to balance through the Team's ability to deliver the amount of work. At this point the team creates tasks to accomplish its acceptance criteria. Those tasks will be used for managing the development cycle.

Right after we analyze the complexity of each Feature, we set up the ones that the Team will be able to achieve during the Sprint Cycle \(notice that our standards takes up to a 10 business days cycle\).

During the Sprint Cycle, neither the Client nor the PM is able to change requirements nor add more deliverables for the Sprint Cycle.

Thus, we can start to work and align with the Client all the expectations of the next delivery.

#### Kanban Board

The Kanban Board is organised as follows:

* To Do
* In Progress
* Block
* Task Done
* Code Review
* Code Review Failed
* Homologation Waiting Release
* QA Failed
* Homologation QA
* Homologation QA Failed
* Production Waiting Release
* Production QA
* Production QA Failed
* Approved

Notice that each phase of the kanban board represents a status of deployment for our Client. 

The higher the phase, the most critical is the task, so in case we have `Production QA Failed` means that we need full support to tackle those issues.

#### Sprint Daily Meeting

The Team along with the PM set up a moment during the workday to align the information of the Team during the Sprint Cycle. This moment is called Daily Meeting. During a maximum of 15 minutes, the whole Team needs to update themselves with the current status of their development. Normally we follow some guidelines for Daily Meetings:

* What I did since the last Daily Meeting
* What am I doing now? 
* Which problems am I facing? \(being objective, with further details for discussion with someone of the Team able to help\)
* What am I gonna do until the next Daily Meeting?

#### Sprint Delivery

Considering that the Sprint Cycle is finished, the team needs to prepare the deploy process and have the quality assurance process approved. 

After QA Approval, the task can be set up as Done. In case the task has some bugs or some other issues, the task downgrades its level to `QA Failed` and the developer needs to tackle it as soon as possible. 

The Sprint Cycle is approved successfully if all the US planned during the planning were Approved by QA. In either case, the Sprint Cycle will fail.

#### Sprint Retrospective

After the Deploy process and the Approval/Disapproval of the Sprint Cycle, the Team needs to review their work during the past cycle and share with each other to improve and align any other problems that is affecting the developers individually and as a team. Here are the guidelines for the Retrospective:

* What happened during the Cycle that the team needs to review?
* What was nice on the Cycle?
* What needs to improve?
* What we can do for the next Sprint?

#### Bug Reports

Homologation/Production phase, our process needs to be as smooth as possible. Thus, we provide a Service Desk for users to reports adjustments and bug reports. Its structure adapts on the project type (Web or Mobile).

The main points for report are:

* Name
* Email (optional)
* Environment (Dev, Homologation, Production)
* Current Behaviour (Here you tell us briefly what's going on)
* Executed Flow (Tell us what you did with a higher description) 
* This bug happens in... (Multiple browsers/Chrome/Firefox/Safari)(Iphone [Type], Android [Type])
* Resolution (Responsive (All resolutions), Start from Mobile to Tablet, Only Tablet, Web)
* Priority (P0 (ASAP), P1(Fundamental), P2(Important), P3(Wanted))
* Attachments (Video and/or Screenshots)

After user submit, this report is generated as an Asana task and comes for PM review and sent to the Kanban Board as `QA Failed`

## **DAKI Exercise**

* **D** for Drop: When team members want to drop or remove something that bothers them. For example, a team wants to remove \(drop\) weekly meetings with their manager because of micromanaging.
* **A** for Add: What does the team want to add to improve the process? Perhaps adding a weekly breakfast for the whole team or a company to share feelings/feedback with the rest of the people.
* **K** for Keep: When team members want to keep something. For example, the team decides to keep a stand up meeting with a song chosen by a team member.
* **I** for Improve: Something that a team wants to improve. A good example is when a team reduces the technical debt from legacy code to avoid fixing bugs all day long.
