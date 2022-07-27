---
layout: post
title: QA Best Practices
---

## How to prepare a QA process to ensure consistent delivery of a software.

Before we kickstart, it is important to note that throughout this article we will **not** talk about unit testing, test automation and integration testing. 

We're gonna focus on tests related to the Product area.


### What is QA?

Quality Assurance, also known as QA, aims to ensure the quality of a software for a team or organization through testing.

In Software Engineering, QA is based on requirements engineering, main and alternative flow and business rules as well, in addition to the UI interaction behavior.


### Why do we need testing?

1. We minimize inconsistencies in software delivery;
2. UX improvements, thus a user can give a feedback to your product;
3. Effective investment, since through the tests it is possible to identify the necessary business gaps for the creation of new product management strategies, so that they are validated based on the behavior of the final user.


### How is our QA process?

To know more about our management framework, [click here](https://www.mobixtec.com/process).

![process_eng (1)](https://user-images.githubusercontent.com/96849644/181298273-37bd0e18-560a-4776-a7bb-e3a1de7987ac.gif)

The discovery is performed using the Design Thinking technique called *[Double Diamond](https://www.designorate.com/the-double-diamond-design-thinking-process-and-how-to-use-it/)*. In the first diamond, surveys are carried out with users to immerse themselves in the challenge faced by the client. At the end of the process, we deliver a summary of what was understood and defined one or more objectives.

In the second diamond, ideas are generated to solve the challenges and the interfaces are also prototyped: in low, medium and high fidelity.

The implementation phase starts with defining and prioritizing tasks that need to be carried out, then we develop and deliver the feature to be implemented.

**QA will be working more actively in the development and delivery part.**

It is important to note that before a new feature is available to the final user, it goes through a Code Review process by the development team. This delivery validation process goes through two test environments until its final delivery.

The first environment is called *Development*, in which it is only accessed by the Development and QA team that acts more assertively. Here we seek to guarantee product quality, identify errors and report delivery problems. When the feature is working as expected, it will go to the *Staging* environment.

In this environment, which is the second test environment, in addition to the participation of a QA person, it is common for client to perform tests, it is a way to check how the feature is progressing and also to see if what was proposed is being developed correctly.

After the tests are complete, a few final users may be chosen to use this new feature before it becomes available to the general public. These final users can be chosen according to their engagement with the product, sending feedback frequently and promoting engagement in solution delivery.

At the end of the process, the delivery in Production is carried out where all users can have access to the features that have already passed through a testing period.


### What are the tools used in this process?

At Mobix, we use three main tools to give support the testing process:

#### 1. Jira

Used for the management of the company, through Jira it is possible to identify which tasks are being carried out within a Sprint, and assess the status of each task. In that away, we were able to follow the deliveries and we were able to start the testing process.

![Depoy - Agile Board - Mobix (2) (1)](https://user-images.githubusercontent.com/96849644/181298509-3399efa9-654d-4689-b306-5073a1c14741.gif)

There is a Kanban board that is **divided into 5 columns**, where each column represents a development status:

- To Do
- In Progress
- Block
- Commit
- PR

After the Pull Request (PR) is approved, the task is automatically sent to the QA board, where the team can monitor the available features and carry out their tests. The **Deployment board** is structured as follows:

- QA
- Ready for Staging
- Staging
- Ready for Production
- Production

#### 2. Productboard

The Productboard is a complete tool for tracking and managing products, but the QA team uses it to track the tests' progress on each story.

The platform works by dividing lines and columns, in which the lines contain the epics and stories of the product and the columns have different types of data for follow-up. One of these types is the status column for the QA team to track the test's progress in each development environment.

In the column of each development environment, there is a Jira integration. According to the task progress, the status is automatically updated on the Productboard. That is, when a task is delivered by the development team, the status is updated and the Product team can decide if a certain story is available for testing.

![Maracatec - Features (2) (1)](https://user-images.githubusercontent.com/96849644/181298558-ea0cf0c5-9fb8-4dc9-a786-e16613da555a.gif)

There are **three columns**:

- QA Dev
- QA Staging
- QA Production

Inside each column is possible to put one of these **7 status**:

- Not Ready
- To Do
- In progress
- Small issues
- With bug
- Blocked
- Completed

“Small issues” indicates impediments that do not impact the flow of the feature, “With bug” indicates bigger problems that prevent the person from finishing the flow, and when the feature cannot be tested we say that it is “Blocked”.

#### 3. Notion

It serves to go with the requirements document of each product feature. It is divided into epics and stories, in which each story has two topics: Backend and Design. These topics are used so that the feature perspective can be seen by all members of the development team.

- **Backend**

  In this topic, technical observations for backend developers are listed, such as endpoints that need to be integrated and information about database modeling, diagrams that help in the implementation of flows (we usually use Sequence Diagrams) as well.

- **Design**

  Informs in detail the business rules of each feature and it is separated into some topics.

  - Figma Links: In this part, links are added to the story flow and to the navigable prototype of the screens.
  - Acceptance Criteria: Informs the development and QA team how to get to the feature by browsing the software (input), what the feature does (behavior) and how to get out of it (output).
  - Use cases: It is in this topic that the business rules of the feature will be explained.

  Example: The telephone field will be mandatory at the time of registration.


---


## QA checklist


#### 1st step: Read the Changelog

Documentation that the development team lists all the tasks that were finalized in the version, separating them into three sections: **Adjustments, Improvements and Features**. In the tasks listed, a link is added that redirects to Jira, which will contain more details about it.


#### 2nd step: Bug Mapping

Mapping of the bugs that usually appears during testing. The mapping template is below:

**Title:**

1. **Bug Summary**: Briefly state what the bug is.

**Body:**

1. **Environment:** Must be informed in which environment the bug was found (Develop, Staging, Production);
2. **Device:** Desktop or Mobile (Android or iOS);
3. **Browser:** Chrome, Edge, Safari;
4. **User account:** Login and password of the account used to perform the tests, if the disclosure of this information is allowed;
5. **Steps to reproduce:** The flow that was made until the bug occurred;
6. **Real behavior:** What is happening at the moment to be considered as a bug;
7. **Expected behavior:** What the correct behavior should be;
8. **Image or video:** Visual record of the bug to facilitate understanding.


#### 3rd step: Client support

Sometimes it is possible for the client or final users to find bugs and map what happened. They will not provide all the information that is added in the bug mapping, that's why the QA team works to collect this information.

After collect this data, the QA team tries to reproduce the bug and map out correctly for the development team to fix.


## Conclusion

This process allows the QA team to do specific and detailed work, concluding that tests are heavily based on requirements documentation.

In addition, the person assigned for the product management role can identify in a macro way how the tests are progressing and reduce the risks to release a new version.

Another important factor is that the client also has the freedom to follow this process through the tools, generating trust in the team and a sense of belonging.
