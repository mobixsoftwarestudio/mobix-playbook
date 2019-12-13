# Mobix Software Studio Playbook

# Development Practices

## Standards

### Development Kickstart

During the kickstart process, we have some requirements that we feel it's mandatory for a healthy project development lifecycle: 

- [x] Amount of hours allocated for the project
- [x] Requirements documentation
- [x] API documentation
- [x] UI Documentation (Set up as an Invision, Sketch, Adobe XD, among others)
- [x] Mocked board for project management (Asana Board or Asana List)
- [x] Estimated dates for Sprint ceremonies (Sprint Planning, Daily Meetings, Sprint Retrospective)
- [x] Repository created in our GitHub account with our standards reviewed and aligned with the team.

The project won't have its kickstart while we have our requirements checked up.

### Git Flow

At Mobix we introduce a configuration model tailoring the best practices of code management. At first, you already know that we use `GitHub` to manage everything. 

Tailoring the project structure, we define two main branches: 

- master
- develop

Where `master` pulls the *production* version of the software. In that scenario, the version we deploy and go live is tagged with the specific version into that branch.

Regarding to `develop`, we pull all implementations that we do in our team to validate the sprints and present to the client while we don't pull it for production. It's also the branch we use for client's approval within the sprint presentation.

Outside those two main branches, we define the following approach: 

- feature
- issue
- hotfix
- release

Each one from the above are set up as folders with the correspondent branches (i.e `feature/my-branch`).

### Boilerplates

To kickstart a project at Mobix, we need to evaluate the project complexity as well as the type of architecture. 

On regular projects we develop, we usually avoid to start from scratch - which means we have our patterns set up and we keep our standards for each project we develop. Thus, we can keep a good maintanance and also share with our developers community our practices and keep always seeking for improvements.

We set up some hours during the week/month in our team's allocation to check our boilerplates by evaluating some good practices we implement in some projects that we would like to keep in further challenges.

#### React Projects

- ReactJs Projects: https://github.com/mobixsoftwarestudio/react-boilerplate
- React Native Projects: ~coming soon~

#### Node Projects

- NodeJs Projects: https://github.com/mobixsoftwarestudio/node-boilerplate

### Estimates Guideline

~coming soon~

### QA

~coming soon~

### ADA for Mobile Apps

~coming soon~

### Continuous Integration

~coming soon~

### Continuous Deploy

~coming soon~
