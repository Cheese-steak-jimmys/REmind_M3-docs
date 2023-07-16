# DylanDavidson_T3A2-A

---

## REmind_M3 Full Stack App (Part A)

[![github icon](https://skills.thijs.gg/icons?i=github)](https://skills.thijs.gg) [T3A2-A Github Repo](https://github.com/Cheese-steak-jimmys/REmind_M3-docs)

<img src="https://d33wubrfki0l68.cloudfront.net/96c17da373ab36f886cfc255d2de340a476c3b49/eb40a/assets/images/tool-icons/trello.png" alt="drawing" width="43"/> [T3A2-A Trello board](https://trello.com/b/ji5PjIUX)

## Table of Contents

- [Description](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#description)
- [Purpose](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#purpose)
- [Functionality/Features](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#functionality--features)
- [Target Audience](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#target-audience)
- [Tech Stack](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#tech-stack)
- [Dataflow Diagram](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#dataflow-diagram)
- [Application Architecture](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#application-architecture-diagram)
- [User Stories](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#user-stories)
- [Wireframes](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#wireframes)
- [Trello Board](https://github.com/Cheese-steak-jimmys/REmind_M3-docs#Trello-Board)

## Description

REmind_M3  
Have you ever missed an astronomical event, like witnessing the blood moon in 2022 or missing a show when your favourite 90's artist was in town?  
  
Maybe you didn't know. Maybe you did and forgot.  
  
This is an app that will give you a notification when you don't want to miss out on something.  
Create events for your eyes only or viewable on a public forum. Add someone else's to your list, who knows what you may discover.

### Purpose  
The purpose of this application is to help people stay informed by keep ahead of events, get the most out of their interests and share with others.

### Functionality / features

* Create events that trigger an alert at a desired time and date.  
* View main listings as a guest user or sign up to obtain a profile.
* Edit and delete events.  
* Events can be private or viewable to all on a public wall.  
* View and save others events, get notifications when they do.


### Tech Stack

---

### **Front-end**

[![My Skills](https://skills.thijs.gg/icons?i=html)](https://skills.thijs.gg) HTML  
[![My Skills](https://skills.thijs.gg/icons?i=js)](https://skills.thijs.gg) JavaScript  
[![My Skills](https://skills.thijs.gg/icons?i=css)](https://skills.thijs.gg) CSS  
[![My Skills](https://skills.thijs.gg/icons?i=react)](https://skills.thijs.gg) React

#### **Back-end**

[![My Skills](https://skills.thijs.gg/icons?i=nodejs)](https://skills.thijs.gg) NodeJS

<img src="https://ajeetchaulagain.com/static/7cb4af597964b0911fe71cb2f8148d64/87351/express-js.png" alt="drawing" width="49"/> ExpressJS

#### **Database**

[![Mongo icon](https://skills.thijs.gg/icons?i=mongo)](https://skills.thijs.gg) MongoDB

<img src="https://camo.githubusercontent.com/55c96f41fc5dba5af624827c4205fdb469978360e0554d081b71cab80d0b2e1d/687474703a2f2f7777772e6572696b61736c616e642e636f6d2f7374617469632f696d616765732f6d6f6e676f6f73652e706e67" alt="mongoose icon" width="60" border-radius=""/> Mongoose

#### **Project Management Tools**

<img src="https://d33wubrfki0l68.cloudfront.net/96c17da373ab36f886cfc255d2de340a476c3b49/eb40a/assets/images/tool-icons/trello.png" alt="drawing" width="43"/> Trello

#### **Testing**

- [Cypress](https://www.cypress.io/)
- [Jestjs](https://jestjs.io/)

#### **DevOps Tools**

[![git icon](https://skills.thijs.gg/icons?i=git)](https://skills.thijs.gg) Git

[![github icon](https://skills.thijs.gg/icons?i=github)](https://skills.thijs.gg) GitHub

[![VSCode icon](https://skills.thijs.gg/icons?i=vscode)](https://skills.thijs.gg) Visual Studio Code

#### Design Tools

[![figma icon](https://skills.thijs.gg/icons?i=figma)](https://skills.thijs.gg)
[Figma](https://www.figma.com/)

- [Lucidchart](https://www.lucidchart.com/pages/what-is-a-flowchart-tutorial#top)

- [DALL-E Image Generator](https://www.bing.com/create)  

- [Canva](https://www.canva.com/)


## Dataflow Diagram

![Dataflow Diagram](docs/img/data-flow-diagram.png)  
#### Detail  
1. The user interacts with the User Interface (UI) to log in, create an account, continue as a guest, or log in using an API from GitHub or Google.

2. If the user chooses to log in using an API, the browser sends a request to the Server to authenticate the user through the selected API.

3. If the user chooses to log in or create an account, the browser sends the appropriate request to the Server, which authenticates the user’s credentials or creates a new account in the Database.

4. Once authenticated or if continuing as a guest, the user can view posts on a public wall through the UI, which sends a request to the Server to retrieve public posts from the Database.

5. If the user is a guest and checks a box next to a post to indicate that they would like to receive notifications for the event described in that post, they are prompted to sign up for an account.

6. If the user is logged in, they can create a new post through the UI, specifying whether it should be private or public and including information about an event (such as date and time).  
*The user may also choose to include a GIF from Giphy which sends a request to the Giphy API to retrieve relevant GIFs. This is only the case if I have time to include it.*

7. The UI sends a request to the Server to store the post in the Database.

8. The user can also view their profile page through the UI (if logged in), which sends a request to the Server to retrieve all of their posts (both private and public) as well as public posts from other users that they have checked to receive notifications for.

9.  When an event described in a post occurs, the Server sends a notification to the user through the UI (if logged in).

10.  The Server processes these requests and sends responses back to the UI, which displays the data (and GIFs, if applicable) to the user.

## Application Architecture Diagram

![Application Architecture Diagram](docs/img/AAD-ss.png)

## User Stories 


### Personas  
![Personas](docs/img/personas-ss.png)

## Wireframes

#### Homepage![Dataflow Diagram](docs/img/homepage-wireframe-draw-ss.png)

#### Homepage - Signup![Dataflow Diagram](docs/img/homepage-signup-wireframe-draw-ss.png)  
  
#### Wall Page![Dataflow Diagram](docs/img/wall-wireframe-draw-ss.png)


#### Profile Page![Dataflow Diagram](docs/img/profile-wireframe-draw-ss.png)
---

## Trello Board (Kanban)
#### Kanban Starting Point![Trello Board](docs/trello-ss/trello-T3A2-A-base-ss.png)

#### Making Card labels for priority![Trello Board labels](docs/trello-ss/trello-T3A2-A-label-ss.png)  
  
#### Progression of agile method![Trello Board labels](docs/trello-ss/trello-progress-01-ss.png)
