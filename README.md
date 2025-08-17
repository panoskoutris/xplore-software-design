#  Xplore Web Application - Software Design
<p align="center">
  <img src=".\mockups\xplore-logo.png" alt="xplore-logo" width="200"/>
</p>

##  Overview

**Xplore** is an educational storytelling web application developed as part of the course **Software Engineering I** at the Aristotle University of Thessaloniki (AUTH), School of Electrical & Computer Engineering. . Inspired by the graphic novel *"Ποιός σκότωσε τον κ. Χ;"*, the platform allows interactive learning through stories, riddles, and character-driven progress.

The project follows a **Design-First API** approach and adheres to the **OpenAPI 3.0.4 specification**.

---

##  Functional Features

-  **Gamemaster**: Can browse stories and panels, invite solvers, and add riddles.
-  **Solver**: Accepts invitations and solves riddles.
-  **Story Flow**: Users proceed through stories using narrative panels.
-  **Custom Riddles**: Gamemasters can create or fetch riddles from the database.

---

##  Project Deliverables

The development of the project followed a structured process organized in **three main deliverables**:

###  Deliverable 1

- Collection of **User Requirements**
- Definition of **User Stories**
- Design of **Use Case Diagrams**
- Creation of **Activity Diagrams** for key functionalities

###  Deliverable 2

- Design of the **Class Diagrams**
- Implementation of **Sequence Diagrams** to model system interactions

###  Deliverable 3

- Definition and implementation of the **RESTful API**
- Documentation of the API using **OpenAPI (Swagger)**
- Organized project structure based on a **Design-First** approach
---

##  Repository Structure
```
xplore-software-design/
├── diagrams/                             # All UML and structural diagrams
│   ├── activity-diagrams/
│   │   ├── attempt-riddle.png
│   │   ├── choose-riddle.png
│   │   └── enter-storyline.png
│   │
│   ├── class-diagrams/
│   │   ├── account-package.png
│   │   ├── answer-package.png
│   │   ├── full-class-diagram.png
│   │   ├── full-collapsed-class-diagram.png
│   │   ├── hint-package.png
│   │   ├── invitation-package.png
│   │   ├── riddle-package.png
│   │   ├── solver-account-package.png
│   │   └── story-package.png
│   │
│   ├── design-patterns/
│   │   ├── bridge.png
│   │   └── proxy.png
│   │
│   ├── sequence-diagrams/
│   │   ├── attempt-riddle.png
│   │   ├── choose-riddle.png
│   │   └── enter-storyline.png
│   │
│   └── use-case-diagrams/
│       └── use-case-diagram.png
│
├── mockups/                             # UI mockups for key user actions
│   ├── accept-invitation.png
│   ├── answer-riddle-incorrectly.png
│   ├── answer-riddle.png
│   ├── app-logo.png
│   ├── choose-database-riddle-1.png
│   ├── choose-database-riddle-2.png
│   ├── choose-role.png
│   ├── choose-story.png
│   ├── congrats.png
│   ├── create-riddles.png
│   ├── final-story.png
│   ├── hint-page.png
│   ├── homepage-gamemaster.png
│   ├── homepage-solver.png
│   ├── log-in.png
│   ├── riddle-options.png
│   ├── sign-up.png
│   ├── story-panel.png
│   └── xplore-logo.png
│
├── swagger/                             # Design-First API specification
│   ├── api.json
│   └── components.json
│
├── user-stories/                        # Gherkin-style user story features
│   ├── attempt_riddle.feature
│   ├── choose_riddle.feature
│   └── enter_story.feature
│
└── README.md


```

---

##  API Specification

The full OpenAPI spec is defined in [`initial.json`](./initial.json), describing endpoints such as:

- `POST /user`: Create new user (solver or gamemaster)
- `GET /user/{id}/story/{story-id}/panel`: View panels
- `PUT /user/{id}/invitation/{invitation-id}`: Respond to invitations
- `POST /user/{id}/story/{story-id}/riddle`: Add custom riddles
- `GET /user/{id}/answer`: Retrieve answers by solvers


---

##  Technologies Used

- **OpenAPI 3.0.4**
- **Swagger UI / Editor**
- **JSON/YAML Schema Design**
- **UML Diagrams** (Activity, Class, Use Case)

---

##  Authors

- Team: Xplore API Team

---

##  License

Licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0.html).



