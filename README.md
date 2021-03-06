# Adventure Todo List

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
An interesting daily planner that motivate users to finish their tasks by giving out rewards. Could be potentially used as a social/game app to form study/work group.

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category:**
Social Networking / Productivity 
- **Mobile:**
This app would be primarily developed for mobile but would be beneficial to have it on Watch and computer.
- **Story:**
This app is designed for people who use to procrastinate and lack motivation to get things done. The goal of this app design is to make the jobs seems less painful and offer more reward and happniess to user when they complete their tasks.
- **Market:**
Any individual could choose to use this app. 

- **Habit:**
Great for productivity and allows the user to maintain a habit of acomplishing their tasks via in-app milestones

- **Scope:**
We first want to focus on the basic todo list functionally, such as create a task, set a deadline, and send notification. Then, we want to implement a reward system that user can buy collections with the tasks they complished. Finally, it would be nice to have a friend circle functionality so that user can find their study groups. In addition to this, a nice feature to have would be sharing the same tasks with your friends

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* User logs in to view their current weekly schedule
* User have a profile where they can view all their task history
* User creates a task
  * User sets a name, type, and deadline
* User completes a task
* User chooses where notifications will be sent
* Reward user on completed tasks with in-app currency
* User purchases rewards with in-app currency
* Users can check their reward milestones

**Optional Nice-to-have Stories**

* User can log in through Google
  * Google Calendar integration
* Social feature between friends
  * Leaderboards, games, etc.
* If no internet connection, display user information from last online session

### 2. Screen Archetypes

* Login Screen
* Register Screen
   * User can sign up or login into their account
   * Upon returning to the app after it is closed, the user will remain logged in.
* Profile Screen
   * Displays profile picture, name, and task history
* Schedule Screen
  * Display upcoming task for the week
  * Option to view daily, weekly, and monthly tasks
* Store Screen
  * To purchase in-app features


### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Schedule
* Profile
* Store

**Flow Navigation** (Screen to Screen)

* [SignIn Page]
   * [SignUp page]
   * [Schedule page]
* [Schedule page]
   * [Tasks Page]
   * [Create Task Page]
   * [Notification Options Page]
   * [Edit Tasks Page]
   * [Tasks Completion Page]
* [Profile page]
   * [Edit Profile Page]
   * [Tasks History Page]
   * [Rewards Milestone Page]
* [Store page]
   * [Items Page]
   * [In App currency Page]
   * [Buy Item Page]

## Wireframes
Hand Sketched

<img src="https://user-images.githubusercontent.com/64571228/108005972-05ab3b80-6faf-11eb-8376-15b09e72f24d.png" width=600>

Digital Low Fidelity (With Flow Navigation Arrows)

<img src="https://user-images.githubusercontent.com/64571228/108005724-53737400-6fae-11eb-89c1-31808895bce1.png" width=600>

## Schema 
[This section will be completed in Unit 9]
### Models

Post

| Property        | Type              | Description                                |
| :-------------- |:----------------- | :----------------------------------------- |
| objectid        | String            | unique id for created task (default field) |
| author          | Pointer to User   | task author                                |
| taskName        | String            | name of task                               |
| taskCategory    | String            | category of task                           |
| taskDeadline    | DateTime          | deadline of task                           |
| taskDescription | String            | description of task                        |
| createdAt       | DateTime          | date when task is created (default field)  |
| updatedAt       | DateTime          | date when task is updated (default field)  |

### Networking
- [Add list of network requests by screen ]
- [Create basic snippets for each Parse network request]
- [OPTIONAL: List endpoints if using existing API such as Yelp]
