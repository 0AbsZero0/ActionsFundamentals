# GitHub Actions Fundamentals

Repo for the `GitHub Actions Fundamentals` training.

## 👉 Objectives

- Understand the __basic components__ and vocabulary of GitHub Actions
- Understand the __YAML__ syntax (scalar types, quotes, literal blocks, maps, and sequences)
- Understand the __workflow syntax__ and how to write workflows using intellisense
- Understand events that can __trigger__ workflows
- Learn the __context and expression syntax__ as well as workflow commands
- Know the different types of __actions__ and how to create/publish them
- Understand the different hosting options for __runners__
- Use __Secrets__ and __Environments__ for staged deployments
- Workflow templates and __reusable workflows__

## Getting ready

Please follow [these instructions](GettingReady.md) and make sure you have set up everything correctly following the [prerequisites](#-prerequisites).

## 📆 Agenda

### Day 1: 🚀 Getting started

- [ ] Introduction and Icebreaker
- [ ] GitHub Actions Fundamentals
- [ ] The YAML syntax
- [ ] Basic workflow syntax
- [ ] Events that trigger workflow
- [ ] Jobs and steps
- [ ] :mag: Demo: Creating a workflow
- [ ] 🔨 Hands-on: [My first Action workflow](hol/01-My-first-workflow.md)
- [ ] Advanced [workflow syntax](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions)
- [ ] :coffee: Break
- [ ] GitHub Actions
- [ ] Types of Actions
- [ ] 🔨 Hands-on: [My first container Action](hol/02-My-first-action.md)
- [ ] Typescript and composite actions
- [ ] Sharing and releasing actions
- [ ] Using the GitHub API and Octokit
- [ ] Job descriptions

### GitHub Actions Fundamentals
- Source Control software
- leverage the power of the open-source commmunity
- flexible platform
- CI/CD pipeline accessibility, workflow flexibility
- Actions in GitHub Marketplace from Verified Creators (blue badge partners) versus individuals
- can be Referenced in Workflow directly
- Integration in GitHub editor
- can control what type of Actions, creators from the Marketplace
- [GitHub Marketplace](https://github.com/marketplace?type=actions)
- automate with workflows with generic workflow engine
- 35 events can trigger a workflow

### The YAML syntax
- .yml or .yaml
- strict superset of JSON
- syntactically relevant newlines and indentation instead of braces
- data-serialized writeable/reable language
- "#" for comments
- key-value pairs
- do not need quotations for spaces
- literal_block is 4 spaces of indentation which keeps line breaks and empty lines until next element
- JSON syntax
- Sequence and array
- Maps use 2 spaces of indentation

### Basic Workflow Syntax
- text file in repository [GitHub Workflows](.github/workflows)
- YAML: "Yet Another Markup Language"
- Events trigger workflows (on:), web-based
- jobs
- execute runners
- contains steps, a reuseable step is an Action

### Events that Trigger Workflow
- webhook, scheduled, manual events
- cron syntax for schedule
- repository dispatch event, allows a repository to webhook into another repository where the event is held; done through GitHub CLI, curl, octokit, etc., needs to autheticate

### Jobs and Steps
- map is runned in parallel by default
- can be chained using keyword
- runs on runner in process
- contains sequence of steps
- steps can be shell command or action
- sequence in a job runs in the same process/directory, runs in shell

### Types of Actions
- Container; Dockerfile or existing image, inputs
- JavaScript/Typescript (unsupported)
- Composite

### Try
- Super-Linter by GitHub for source code validation
- Checkout for branch navigation
- CTRL + SPACE for intellisense
- OPTION + SPACE for Mac
- https://github.com/actions/toolkit
- https://docs.github.com/en/actions/creating-actions/publishing-actions-in-github-marketplace
- [Suleiman Suleiman](ssuleiman@microsoft.com)

### Day 2
- [ ] Introduction
- [ ] Actions for CI/CD
- [ ] Permissions for GitHub Token
- [ ] Environments and Secrets
- [ ] Staged deployments with environments, approvals, and deployment gates
- [ ] 🔨 Hands-on: [Staged deployments](hol/03-Staged-deployments.md)
- [ ] :coffee: Break
- [ ] Action policies
- [ ] Running your workflows
- [ ] Sharing workflows
- [ ] 🔨 Hands-on: [Reusable workflows](hol/04-Reusable-workflows.md)
- [ ] Best practices and security

### Actions for CI/CD
- [Actions: Continuous Integration](https://lab.github.com/githubtraining/github-actions:-continuous-integration)
- [Super Linter](https://github.com/github/super-linter)

## ⚡ Prerequisites

The workshop is designed for developers that have used other platforms like Azure DevOps, GitLab, or Bitbucket and now want to switch to GitHub. But it is also suitable for people that are new to topics like git, CI/CD, and DevOps.

For this workshop you need the following:

- A laptop (Windows, Mac, or Linux)
- A free account for https://github.com
- It is recommended to have a second screen for the hand-on labs

## Cheat Sheet
Find common terminology for reference [here](./CheatSheet.md)

