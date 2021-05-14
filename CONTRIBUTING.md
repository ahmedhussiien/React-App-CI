# Contributing to this project

## Git flow

Gitflow is a workflow that helps with continuous software development and implementing DevOps practices.

this workflow uses two branches mainly to record the history of the project:

- The master branch stores the stable releases of your code.
- The develop branch serves as an integration branch for features.

in addition to some helper branches:

- Hotfix: if any bug appeared on the master branch you can use this branch to fix it.
- Feature: developers should spend most of their time on these branches developing new features.
- Release: once the develop branch has acquired enough features for a release, a release branch is created from the develop branch.

<br />
<p align="center"><img src="https://github.com/ahmedhussiien/React-App-CI/raw/master/readme_assets/branches.svg?raw=true" width="75%" height="75%"></p>
<br />

## Features & Releases lifecycle

The following is a walk-through of the life-cycle of a feature:

- Fork a new feature branch from the develop branch.
- Update, add, commit, and push changes incrementally.
- When you finish, open a pull request to merge your branch with the develop branch.
- Resolve conflicts & feedbacks.
- Another team member or you should merge the pull request.

Releases lifecycle:

- When the team members decide that the develop branch is ready for a release, a release branch is created from the develop branch.
- Team members can add the final touches for the release ( Shouldn't be anything major ).
- Open a pull request to merge with the master.
- After your code passes the tests, approve the pull request.
- Horray! your code is live

## The DevOps process

We -the DevOps team- want you as a developer to focus more of your time on the development. So instead of multiday merge nightmares, you integrate code continuously and always keep it in a deployable state. And instead of deploying code once per month, you can deploy code dozens of times per day, or even after every single commit. Thus, we can create a streamlined development process.

<p align="center"><img src="https://github.com/ahmedhussiien/React-App-CI/raw/master/readme_assets/devops_process.png?raw=true" width="75%" height="75%"></p>

## How to achieve that

### Your responsibilities

- Apply incremental improvements instead of bulk committing code.
- We encourage you to use pull requests since it will automatically run unit tests and integration tests on your code.

### Our promise

Whenever you commit or merge a branch to the develop or the master branches we configured an automated process to do the following:

- Build your code.
- Run unit, and E2E tests.
- Package your code.
- Deploy your code either to the development environment if it was committed to develop branch or the production branch if it was committed on the master branch.

This streamlined development process will help you see your code live much faster, catch bugs early in the development environment, be confident in the production releases to work well, and speed up our time to market.
