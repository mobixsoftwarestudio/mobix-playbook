# Project Management

During the execution of projects, Mobix has a major cycle of Project Management like below:

`(PLANNING -> DAILY -> DEV DONE -> QA -> APPROVED -> READY TO DEPLOY)`

Our Project Manager \(PM\) needs to organize his tasks by the following features:

## Methodology

At Mobix we use Scrum Methodology to achieve the goals. Divided by Sprints, we set up expectations with the Team and with the Client to plan and tackle possible challenges that we might need to achieve the goals. As Scrum is an Agile Methodology applied on Software Engineering process, a few events are made with the Team:

### Sprint Planning

The Team receives the deliverables provided to the Client and PM of the project. At this point, we have the UI requirements documented with the high fidelity prototypes and further recommendations of the Client regarding some prioritizations.

During the planning, we analyze each User Story \(US\) \(provided by UX/UI team along with the PM\) and set up complexity for each US to balance through the Team's ability to deliver the amount of work.

Right after we analyze the complexity of each US, we set up the ones that the Team will be able to achieve during the Sprint Cycle \(notice that our standards take up to 10 business days of the cycle\).

During the Sprint Cycle, neither the Client nor the PM is able to change requirements nor add more deliverables for the Sprint Cycle.

Thus, we can start to work and align with the Client all the expectations of the next delivery.

### Sprint Daily Meeting

The Team along with the PM set up a moment during the workday to align the information of the Team during the Sprint Cycle. This moment is called Daily Meeting. During a maximum of 15 minutes, the whole Team needs to update themselves with the current status of their development. Normally we follow some guidelines for Daily Meetings:

* What I did since the last Daily Meeting
* What am I doing now? 
* Which problems am I facing? \(being objective, with further details for discussion with someone of the Team able to help\)
* What am I gonna do until the next Daily Meeting?

### Sprint Delivery

Considering that the Sprint Cycle is finished, the team needs to prepare the deploy process and have the quality assurance process approved. After the QA Approval, the task can be set up as Done. In case the task has some bugs or some other issues, the task downgrades its level to QA Failed and the developer needs to tackle that as soon as possible. The Sprint Cycle is approved successfully if all the US planned during the planning were Approved by QA. In either case, the Sprint Cycle will fail.

### Sprint Retrospective

After the Deploy process and the Approval/Disapproval of the Sprint Cycle, the Team needs to review their work during the past cycle and share with each other to improve and align any other problems that is affecting the developers individually and as a team. Here are the guidelines for the Retrospective:

* What happened during the Cycle that the team needs to review?
* What was nice on the Cycle?
* What needs to improve?
* What we can do for the next Sprint?

### **DAKI Exercise**

* **D** for Drop: When team members want to drop or remove something that bothers them. For example, a team wants to remove \(drop\) weekly meetings with their manager because of micromanaging.
* **A** for Add: What does the team want to add to improve the process? Perhaps adding a weekly breakfast for the whole team or a company to share feelings/feedback with the rest of the people.
* **K** for Keep: When team members want to keep something. For example, the team decides to keep a stand up meeting with a song chosen by a team member.
* **I** for Improve: Something that a team wants to improve. A good example is when a team reduces the technical debt from legacy code to avoid fixing bugs all day long.

## Tasks Management

We use Asana for task management. We have two different scenarios for task management:

### Kanban Oriented

When the delivery needs to run on a fast track with the Client, we set up a Kanban Board using some oriented steps:

* Backlog
* Sprint Backlog
* In Progress

"In Progress" column means that the developer is currently working on the specific task, no matter if it's a bug fix or a task implementation.

* Dev Done

"Dev Done" means that the developer's finished its work and it's ready for QA Process. Those items will be used for the QA Engineer at Mobix to validate them and set up as "QA Failed" or "Approved". On Asana the QA may add a tag within a card that represents a "Bug", so we can understand at the end of Sprint which items were rolled back and were not approved at the first delivery. The developer is not allowed to set the card as Approved.

* QA Failed

"QA Failed" are the items that the QA Engineers set up for the developers to work on it. Those are higher priority than the "Sprint Backlog" items. When the developer starts it, he needs to put the card on "In Progress" column again.

* Approved

"Approved" means that the QA has validated the feature and found no bugs into the task. It's ready for presentation to the client.

For each card on the board, we normally put the invision link for the high fidelity prototype and the link for the requirements document provided for the Project.

The developer is able to select which cards will be inserted on "Sprint Backlog" column, which will participate in the Sprint Cycle and asserts that those cards will be delivered.

### List Oriented

When the delivery has its roadmap created by the UX/UI team, it's created a section on Asana called "Roadmap", with the User Story for each entity set up and ready for evaluation within a Sprint Cycle.

During the planning, the team checks the US and validates using Scrum metrics to set up the complexity and tasks needed for implementation.

After planning, it's generated another section on Asana called "Sprint X'' where X is the number of the current Sprint and all the US planned are fulfilled into the Section, with assignees for each developer from the Team.

It's created custom fields called "In Progress", "Dev Done", "QA Failed", "Approved" for each line of the section that sets up the current status of implementation. The definitions of the custom fields have the same behavior that we have on the "Kanban Oriented" section.

