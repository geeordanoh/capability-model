# Open Source Engineering Capability Model



## Introduction

In this document, you can find a description of an Open Source Capability Model that serves as a reference path for our engineering teams to progress in their journey towards engineering excellence. As preached by its name, the model is *open source* (this is why it is versioned here), and we very much welcome and encourage contributions from everybody as described in the [Contribution](#contribution-model) section.

## How it works

This capability model was created with the intent to:

- Let engineering teams recurrently self-assess themselves (which is also part of one of the practices in the [Process](#1-process-15) category).
- Help teams evolve towards a better way of working using best practices.

The capability model is composed of three parts, *capabilities*, *scorecards*, and *capability levels*:

- *Capabilities* are behaviors we would like to have and principles we would like to stand by.
- *Scorecards* are lists of practices (divided into categories) that help us to implement the capabilities and measure our improvements towards them.
- *Capability Levels* are levels that indicate our maturity concerning the adoption of capabilities.

Please refer to the [Usage Example](#usage-example) section for an overview.

## Capabilities

- Adopting a well-structured agile development process
- Being aware and formalize *what good looks like*
- Adopting the [*three ways of DEVOPS*](https://www.alldaydevops.com/blog/three-ways-a-principle-based-devops-framework): flow, feedback, continuous learning
- Iterating towards small goals and through experimentation
- Applying the [Broken Window Theory](https://blog.codinghorror.com/the-broken-window-theory/) to software development
- Delivering and demonstrating regularly increments of *working software*
- Monitoring our engineering excellence through regular KPI reviews and actionable improvement plans
- Adopting a *cost-conscious* approach to software engineering and product development
- Caring about the satisfaction of team's individuals
- Adopting a *growth* mindset and *continuous improvement* via [Kaizen](https://en.wikipedia.org/wiki/Kaizen)
- Caring about our *co-worker experience*
- Following the principle: *you build it, you run it, you own it*
- Following the principle: *everything under one roof*, to enable *togetherness*, discoverability, and co-creation
- Ensuring alignment and code quality through the *four-eyes* principle
- Following the principle: *everything as code*, to ensure versioning, tracking, and discovery
- Following the principle: *automating everything you can*
- Following the principle: *cloud-agnostic*
- Ensuring decoupling and well-thought design by adopting an *API-first* approach to software development
- Releasing customer value without any friction and *at will*
- Adopting security, privacy, and traceability as *first-class citizens* in the development process

## Scorecards

### 1. Process (15)

#### Robust adoption of any mainstream agile framework

- [ ] The team runs recurring well-established agile events.
- [ ] All team's work is tracked on an agile board: no ticket no work.
- [ ] The team adopts a well-defined user story template and constantly relies on well-defined acceptance criteria as part of its stories.
- [ ] The Definition of Done is in place, publicly available, and the team abides by it.
- [ ] Retrospectives are published and contain follow-up actions that are assigned, monitored, and executed.
- [ ] Team product demos are recorded and published.
- [ ] Clear, public, and achievable sprint goals are shared at each sprint demo.
- [ ] Each demo contains a publicly accessible form to collect optionally anonymous feedback. The team regularly discusses the feedback in the retrospectives.
- [ ] The team tracks and recurrently reviews its engineering KPIs ([DEVOPS metrics](https://stelligent.com/2018/12/21/measuring-devops-success-with-four-key-metrics/)) and takes follow-up actions to improve.
- [ ] The team recurrently self-assesses its maturity against the DSM capability model, publishes its assessments, and commits to improving.
- [ ] The team follows a publicly documented and structured incident management (from detection to well-defined and monitored post-mortem actions).
- [ ] The team regularly follows a public and well-detailed onboarding plan for new joiners, which is regularly updated and contains measurable milestones (e.g., commit on the first day, own a user story in the first three sprints, etc).
- [ ] Each team member collects feedback with a 365 survey from teammates and peers with a standard optionally anonymous form, at least every tertial. An honest discussion is recommended without taking feedback personally.
- [ ] The team measures its well-being with a publicly shared optionally anonymous happiness matrix at every sprint, and a health check workshop every tertial.
- [ ] The team owns a cloud cost dashboard and reviews it regularly to minimize cloud costs.

### 2. Code (11)

#### Code is gold, how do we manage it?

- [ ] All source code is under GitHub and correctly assigned to the team as an owner.
- [ ] Team composition is up to date on GitHub.
- [ ] All team systems have been provisioned and are correctly listed and configured in our developer portal (e.g., backstage).
- [ ] All team systems publish (where applicable) artifacts on build on our company artifact server.
- [ ] All changes are subjected to a pull request, with no commits straight to master.
- [ ] The team follows a well-defined and publicly available development flow (e.g., GitHub flow).
- [ ] No raw commits: all commits have a JIRA issue associated with the commit message and branch name.
- [ ] Builds have a unique version number.
- [ ] Documentation is treated as code and stored beside it in the system's repo. Images are code as well. Docs are in our developer portal (e.g., backstage).
- [ ] Harmonizer and linting checker is part of the continuous integration pipeline.
- [ ] Technical debt is regularly measured (e.g., open tickets in an epic) and tackled by consciously assigning a defined percentage of the available development capacity.

### 3. Architecture and Infrastructure (13)

#### How do we build on solid foundations?

- [ ] Infrastructure as code is adopted for all team systems.
- [ ] All team systems are deployable worldwide (i.e., multi-cloud support).
- [ ] All team systems run on managed resources (e.g., managed K8S cluster).
- [ ] All team systems deploy independently.
- [ ] All team systems scale horizontally.
- [ ] All team systems rely on autoscaling.
- [ ] All our systems (where applicable) are documented in terms of produced/consumed API and events in our developer portal (e.g., backstage).
- [ ] Client and server code is automatically provisioned/generated based on API specs loaded on our developer portal (e.g., backstage).
- [ ] All exposed APIs and Events are versioned.
- [ ] Immutable architecture for all our environments.
- [ ] All team's services are managed through a service mesh.
- [ ] Distributed tracing tracks all messages exchanged.
- [ ] All application logs are aggregated and searchable.

### 4. Value (14)

#### How we deliver customer value?

- [ ] All systems can be released/rolled back at will, on click, in every environment. All team members know how to do that.
- [ ] Every release produces automated release notes in terms of JIRA issues included in that release.
- [ ] The team regularly brings working software at sprint demos, all user stories are demoed via working software.
- [ ] The team regularly performs design sprints.
- [ ] The team adopts the Company's design system.
- [ ] All our repositories are under continuous deployment.
- [ ] All our repos are under continuous delivery.
- [ ] Continuous delivery/deployment is automatically generated via automated provisioning (e.g., backstage).
- [ ] At the beginning of their initiatives, the team pitches their architecture and design in a public session.
- [ ] All systems can be released with zero downtime.
- [ ] Features can be released behind a standardized feature toggle mechanism.
- [ ] Releases can be deployed with standardized traffic or regional throttle.
- [ ] Features can be released with a standardized A/B test framework.
- [ ] Data from the service desk is regularly analyzed to improve the support or the product itself.

### 5. Security (6)

#### Shift left on security

- [ ] No credentials in the code, all secrets managed by our standard secret manager.
- [ ] No team account is passed around, all accounts are stored in our team vault.
- [ ] All cloud roles are well-defined and no ad-hoc cloud role is present in our cloud projects.
- [ ] All continuous integration pipelines include security scans (Blackduck, Prisma, OWASP).
- [ ] None (except continuous deployment/delivery agent) has access to the prod environment.
- [ ] InfoSec team is involved when pitching for any new major initiative (see [**Value**](#4-value-14)).

### 6. Data (7)

#### Data is king, how do we worship it?

- [ ] All our data sources are managed and with redundancy guarantees (e.g., cloud-based).
- [ ] Any data source can be restored to any point in time.
- [ ] Any data source has a clear system owner, we rely on queues or async mechanisms to support multiple writers.
- [ ] All data comply with European and Chinese privacy laws, recurring compliance checks are performed.
- [ ] Our schemas evolutions are versioned and automatically managed (e.g., flyway).
- [ ] All systems rely on predefined data pipelines (no ad-hoc solutions).
- [ ] All systems have in non-prod environments have automated  test data management (API-based test data generator and dataset reset).

### 7. Quality (10)

#### Quality matters

- [ ] Unit tests are part of the continuous integration pipeline and are triggered in any build.
- [ ] All our repositories are under continuous integration.
- [ ] Quality gates in the continuous integration prevent quality deterioration (e.g., code coverage gate quality).
- [ ] Continuous integration is auto-generated via automated provisioning (e.g., backstage).
- [ ] Contract testing is part of the continuous integration pipeline and covers all external dependencies.
- [ ] Static analysis is part of the continuous integration pipeline.
- [ ] Integration tests are part of the continuous integration pipeline.
- [ ] Performance tests are part of the continuous integration pipeline.
- [ ] Synthetic monitoring in place for all major business flows.
- [ ] Chaos engineering attacks regularly stress and/or tear down all systems.

### 8. Observability (5)

#### We are watching you

- [ ] Observability as code for all our systems. Baked in by default (e.g., via backstage provisioning).
- [ ] The team has a public dashboard of metrics and alarms.
- [ ] The team ensures 24/7 support via on-call rotation.
- [ ] Run-books for supporting on-call people are part of the documentation of every system.
- [ ] The status of all the product capabilities owned by the team are exposed publicly via a status page.

## Capability Levels

As mention before, the capability model exists to be used by teams in a recurrent self-assessment. With it, team will measure their capability adoption by evaluating themselves against each scorecard (each checkbox assigns one point to the team) to obtain a cumulative score for each area.

In line with the [Shuhari](https://en.wikipedia.org/wiki/Shuhari) principle, the scoring system is composed by belts, similar to the ones used in martial arts. The idea behind the system is that in order to reach the next level (or belt), the students needs to gather more knowledge than brought them to the current level.

The following table associates the percentage of achievements for each area that are needed to obtain the corresponding belt. *For Example* if a team obtained 8 out of 15 points in the scorecard related to the [Process](#1-process-15) area, then such team acquires the *Green Belt* for that area cause it have achieved 53% of the items.

| Belt color                                  | Items achieved |
|---------------------------------------------|----------------|
| ![white_belt](attachments/white_belt.png)   | 0% - 13%       |
| ![yellow_belt](attachments/yellow_belt.png) | 14% - 28%      |
| ![orange_belt](attachments/orange_belt.png) | 29% - 43%      |
| ![green_belt](attachments/green_belt.png)   | 44% - 60%      |
| ![blue_belt](attachments/blue_belt.png)     | 61% - 79%      |
| ![brown_belt](attachments/brown_belt.png)   | 80% - 99%      |
| ![black_belt](attachments/black_belt.png)   | 100%           |

## Contribution Model

This is an open-source capability model. Everybody should contribute, and contribution is part of the model itself. We believe that teams own their journey towards engineering excellence. Teams must contribute to this model and modify its capabilities, practices, or the whole model itself. To actively contribute to the capability model, open a pull request explaining the reason for your change, changes that raise the bar are the most welcome! The maintainers of this capability model will evaluate them and will come back to you.

## Usage example

This tertial the team *Chicago Bulls* performed its regular capability self-assessment and scored as follows:

| Section                       | Score       | Level                                       |
|-------------------------------|-------------|---------------------------------------------|
| Process                       | 8/15 (53%)  | ![green_belt](attachments/green_belt.png)   |
| Code                          | 9/11 (81%)  | ![brown_belt](attachments/brown_belt.png)   |
| Architecture & Infrastructure | 9/13 (69%)  | ![blue_belt](attachments/blue_belt.png)     |
| Value                         | 10/14 (71%) | ![blue_belt](attachments/blue_belt.png)     |
| Security                      | 2/6 (33%)   | ![orange_belt](attachments/orange_belt.png) |
| Data                          | 7/7 (100%)  | ![black_belt](attachments/black_belt.png)   |
| Quality                       | 7/10 (70%)  | ![blue_belt](attachments/blue_belt.png)     |
| Observability                 | 3/5 (60%)   | ![green_belt](attachments/green_belt.png)   |

Given the above results, the team realized they needed to improve their security practices where they felt weak. As a consequence, the team drafted a plan to tackle some tech debt, and some existing weak practices and committed to it. By pursuing such a plan, the team grew its capabilities and self-promoted themselves from orange belt to green belt in the following capability self-assessment: oorah! During this journey the team also discovered a new and innovative security practice and opened a PR to augment the DSM capability model, helping to co-create the road towards excellence of all DSM teams: double oorah!
