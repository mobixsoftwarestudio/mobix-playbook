# Development Practices

## Standards

### Development Kickstart

NOTE: If you want to check tools and process regarding the project management, please [click here](6-project-management.md).

During the kickstart process, we have some requirements that we feel it's mandatory for a healthy project development lifecycle:

* [x] Amount of hours and resources allocated for the project
* [x] Requirements documentation
* [x] API documentation
* [x] UX Research and documentation
* [x] UI Documentation \(Set up as an Invision, Sketch, Adobe XD, among others\)
* [x] Mocked board for project management \(Asana Board or Asana List\)
* [x] Estimated dates for Sprint ceremonies \(Sprint Planning, Daily Meetings, Sprint Retrospective\)
* [x] Repository created in our GitHub account with our standards reviewed and aligned with the team.

The project won't have its kickstart while we have our requirements checked up.

### Git Flow

At Mobix we introduce a configuration model tailoring the best practices of code management. At first, you already know that we use `GitHub` to manage everything.

Tailoring the project structure, we define two main branches:

* master
* develop

Where `master` pulls the _production_ version of the software. In that scenario, the version we deploy and go live is tagged with the specific version into that branch.

Regarding to `develop`, we pull all implementations that we do in our team to validate the sprints and present to the client while we don't pull it for production. It's also the branch we use for client's approval within the sprint presentation.

Outside those two main branches, we define the following approach:

* feature
* issue
* hotfix
* release

Each one from the above are set up as folders with the correspondent branches \(i.e `feature/my-branch`\).

### Boilerplates

To kickstart a project at Mobix, we need to evaluate the project complexity as well as the type of architecture.

On regular projects we develop, we usually avoid to start from scratch - which means we have our patterns set up and we keep our standards for each project we develop. Thus, we can keep a good maintanance and also share with our developers community our practices and keep always seeking for improvements.

We set up some hours during the week/month in our team's allocation to check our boilerplates by evaluating some good practices we implement in some projects that we would like to keep in further challenges.

**React Projects**

* ReactJs Projects: [https://github.com/mobixsoftwarestudio/react-boilerplate](https://github.com/mobixsoftwarestudio/react-boilerplate)
* React Native Projects: ~coming soon~

**Node Projects**

* NodeJs Projects: [https://github.com/mobixsoftwarestudio/node-boilerplate](https://github.com/mobixsoftwarestudio/node-boilerplate)

### Estimates Guideline

During the Sprint Planning ceremony, the whole team decide which user stories will be assigned to the next Sprint. For this to happen perfectly, we set up some estimates guideline to tackle the forecast of the user story deliveries.

For each user story \(US\), we usually slice it into small tasks to help us decide the complexity point we need to set up:

`User Story: Me, as an user, would like to authenticate into my account to have access to main features.`

* [ ] 1 : Easy task, with low complexity and fast to delivery.
* [ ] 2 : Easy task, with low complexity but requires more effort to delivery.
* [x] 3 : Medium task, with medium complexity with a known effort to delivery.
* [ ] 5: Medium task, with medium complexity which requires research and effort to delivery.
* [ ] 8: Hard task, with high complexity which requires research and higher effort to delivery.
* [ ] 13: Need to review the task and transform it to a user story.

The team assigned to that user story will estimate the effort needed to tackle the above challenge. Each team member will set the amount of points to tackle it and together they will assign officially the points for that US. At this moment, it's highly important for the team to create discussions to understand all possibilities before make it official.

**How we know the amount of work the team handles?**

During the kickstart process, we set a 1 week-sprint to understand the deliveries, team velocity and the unknown challenges the project might create during the development lifecycle.

In that case, we define a burndown chart with the team's accuracy on solving the tasks.

![](https://www.visual-paradigm.com/servlet/editor-content/scrum/scrum-burndown-chart/sites/7/2018/11/burndown-chart-and-emotion.png)

That chart helps a lot our PM and the team to understand how good we are in terms of velocity x effort.

### QA

~coming soon~

### ADA for Mobile Apps

~coming soon~

### Continuous Integration

~coming soon~

### Continuous Deploy

~coming soon~

