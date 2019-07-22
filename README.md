# CMM Development Process with Gitlab CE
This document defines the CMM development process based on an agile methodology perspective using Gitlab CE

## Content

1. [Introduction](#introduction)
2. [Sprints](#sprints)
	- [Sprints Example](#Sprints-example)
3. [User Stories](#user-stories)
	- [User Story Example](#user-story-example)
4. [Tasks](#tasks)
5. [Epics](#epics)
	- [Epic Example](#epic-example)
6. [Backlog](#backlog)
7. [Boards](#boards)
	- [Board Example](#board-example)

## Introduction

This document defines the CMM Development Process based on an agile methodology perspective.
It takes in consideration that all stakeholders are familiar with agile methodologies like Kanban and Scrum.

## Sprints

The current CMM development process is conducted in iterations called Sprints, every Sprint lasts for 2 weeks.
In the context of Gitlab the Sprints are called *Milestones*.

Milestones in Gitlab are a way to track issues to achieve a broader goal in a certain period of time.
They allow to organize issues into a cohesive group, with a start date and a due date.

Set the milestone start date and due date to represent the start and end of the agile sprint.
Add an issue to your agile sprint by associating the milestone to the issue.

### Sprints Example
![Alt](/sprints_01.JPG "Sprints (Milestones)")

## User Stories

User stories may be written by various stakeholders including clients, users, managers or development team members.
They are written as a informal description of one or more features related to the functionality of CMM.
In Gitlab CE the User Stories are represented as Issues.

Every User Story (*Issue*) must comply:

- Is assigned at least to one Sprint (*Milestone*) or to the Backlog (*Milestone*)

- Has a Tag with the priority:
	- prio: Low
	- prio: Normal
	- prio: High

- Has a Tag with the status:
	- status: ToDo
	- status: Done
	- status: In progress
	- status: To verify

- Can include a Task section in the description. See Tasks.

During the Backlog Refinement meeting, the team defines new User Stories in the Backlog and reevaluate its priorities.
During the Spring Planning meeting, the team defines who is assigned to the UserStories. 

### User Story Example
![Alt](/userstory_01.JPG "Sprints (User Story)")

## Tasks

How detailed the tasks within a user story should be?
Whether splitting stories or creating tasks, the debate continues on many agile teams about the level of detail that should be included in a user story and associated tasks.

Task are written by the dev-team and for the team braking down a User Story into parts, with defined and specific technical actions.

In GitLab CE the Tasks can be handled by adding a *task section* in the description of the User Story (*Issue*).
See the in the [User Story Example](#user-story-example) the check boxes in the description.

## Epics

An epic is a large user story that cannot be delivered as defined within a single iteration or is large enough that it can be split into smaller user stories.

Gitlab Enterprise Edition (EE) has the infrastructure to handle Epics, however the Community Edition (CE) has not.

In Gitlab CE a way to represent Epics is using Issues with the following characteristics:

Every Epic (*Issue*)

- Has the Tag:
	- Epic

- Has a Tag with the priority:
	- prio: Low
	- prio: Normal
	- prio: High
	
- Has a Tag with the status:
	- status: ToDo
	- status: Done
	- status: In progress
	- status: To verify

At the top of the description:
Includes the list of its User Stories:

```
Epic User Stories:

  1. #813 Define development process with gitlab
  2. #814 Investigate: Migration of wiki
```

The User Stories that belong to an Epic should have as well at the top of the description:

```
Epic #22 Upgrade Kibana
```
See the in the [User Story Example](#user-story-example) the reference to the Epic.

### Epic Example
![Alt](/epic_01.JPG "Epic as an Issue")

## Backlog

The product backlog is the single authoritative source for things that a team works on. That means that nothing gets done that isn’t on the product backlog.

During the Backlog Refinement meeting, the team defines new User Stories in the Backlog and reevaluate its priorities.

To check the back log go to Milestones and select the Backlog or got to the Boards and filter by Milestone selecting Backlog.

## Boards

In order to see the status of the current Sprint go the Board section and add the Milestone corresponding to the Spring.

### Board Example
![Alt](/board_01.JPG "Boards")
