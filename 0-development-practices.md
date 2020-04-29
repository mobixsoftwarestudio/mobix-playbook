# Development Practices

## Standards

### Project Kickstart

During the kickstart process, we have some requirements that we feel it's mandatory for a healthy project development lifecycle:

* [x] Amount of hours per week/month and which people are going to participate
* [x] Requirements documentation / API documentation
* [x] UI Documentation
* [x] Project board for management (modules and features set up based on requirements)
* [x] Project board for development
* [x] Repository created in our GitHub account with our standards.

The project won't have its kickstart while we have our requirements checked up.

### Development Ground Rules

As a mandatory behavior, all developers need to attend to the following implementation process:

* [x] start coding
* [x] e2e implementation (test scenarios needs to be mapped on planning at Asana's)
* [x] run tests locally
* [x] validate implementation
* [x] pre-commit analysis before sendint to repo
* [x] open a pull request
* [x] check if CI/CD passed

### Boilerplates

To kickstart a project at Mobix, we need to evaluate the project complexity as well as the type of architecture.

On regular projects we develop, we avoid to start from scratch - we have our standards for each project we develop. Thus, we can keep a good maintanance and also share internally our practices and keep always the culture of improvements.

We set up some hours during the week/month in our team's allocation to check our boilerplates. Usually we share some good practices we used in some projects with our clients and put it together for future challenges.

**React Projects**

* [React JS using Typescript](https://github.com/mobixsoftwarestudio/react-typescript-boilerplate)
* [React Native using Context](https://github.com/mobixsoftwarestudio/react-native-context-boilerplate)
* [React Native using Redux](https://github.com/mobixsoftwarestudio/react-native-redux-boilerplate)

**Node Projects**

* [NodeJs for Web API](https://github.com/mobixsoftwarestudio/node-boilerplate)
* [NodeJs for Microservices](https://github.com/mobixsoftwarestudio/node-ms-boilerplate)

### Git Flow

#### Branch Standards

At Mobix we introduce a configuration model tailoring the best practices of code configuration.

Tailoring the project structure, we define two main branches:

* master
* homolog
* develop

Where `master` tags the _production_ version of the software. In that scenario, the version we deploy and go live is tagged with its specific version.

`homolog` delivers the current version of the project to validate our results with our client. We also keep our track on QA assessment before going live.

Regarding to `develop`, we merge all implementations that we do in our team to validate the sprint.

Outside those two main branches, we define the following approach:

* feature - for new implementations
* issue - for bug fixes or small adjustments 
* hotfix - for critical fixes 
* release - to tag a version for going live

#### Pull Requests (PRs)

We use Pull Requests as standard for software development.

For each Pull Request opened, we apply CI/CD as a preview integration an delivery. We validate not only what was implemented, but also check if the tests were done correctly.

We also have a culture of Code Review for each PR, where we verify code practices and check quality and performances that we might need to improve.

#### Technical Debts

Technical debts are one of the most important topics around software development. The need to tackle and avoid debts into our code is one of the things we keep on track to improve our projects.

We use [Code Climate](https://codeclimate.com/) to check all maintainability/code smells and test coverage report in the project and set up a moment during the Sprint cycle to check all comments regarding our code and tests. 
The whole team participates on this event, getting a good and deep thoughts about the way we are coding.

### CI / CD flow

![](https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/CI:CD.png?raw=true)

[Jenkins](https://www.jenkins.io/) + [Selenium](https://www.selenium.dev/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Jenkins_Selenium.png?raw=true" width="120">

[Netlify](https://www.netlify.com/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Netlify.png?raw=true" width="120">

#### Mobile Apps

[Bitrise](https://www.bitrise.io/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Bitrise.png?raw=true" width="120">

[Detox](https://github.com/wix/Detox):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Detox.png?raw=true" width="120">

[Appetize](https://appetize.io/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Appetize.png?raw=true" width="120">

#### Devops

[Docker](https://www.docker.com/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Docker.png?raw=true" width="120">

[Kubernetes](https://kubernetes.io/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Kubernetes.png?raw=true" width="120">

[Heroku](https://www.heroku.com/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Heroku.png?raw=true" width="120">

[Digital Ocean](https://www.digitalocean.com/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/Digital_Ocean.png?raw=true" width="120">

[Amazon Web Services (AWS)](https://aws.amazon.com/):

<img src="https://github.com/mobixsoftwarestudio/mobix-playbook/blob/master/Images/AWS.png?raw=true" width="120">

#### Fake Back End

It is common to face a client that needs to validate his/her product, but with no structure for that. Also doing a pipeline of development may loose the opportunity window for his/her business, so we need to make it fast.
To tackle this challenge, we have implemented an approach to mock an API to the frontend team to avoid barriers in terms of back end demands.

We only need to add a `api.json` file into the project with the expected data structure that it's supposed to be your desired API and then can be runned out with a continuous deploy and it's online in a few minutes.

