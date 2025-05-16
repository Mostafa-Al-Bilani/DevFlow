<img src="./readme/title1.svg"/>

<br><br>

<!-- project overview -->
<img src="./readme/title2.svg"/>

> DevFlow is an AI-driven developer workspace that unifies repository management, CI/CD automation, and analytics into one seamless platform.  
> It analyzes commits, suggests improvements, and automates deployment pipelines so developers can focus on writing quality code.  
> With DevFlow, every push triggers intelligent insights and every merge powers your production workflow.

<br><br>

<!-- System Design -->
<img src="./readme/title3.svg"/>

### System Design

The backend of DevFlow is built on a robust relational schema powering users, repositories, commits, pipelines, analytics, and settings.

#### ER Diagram

![ER Diagram](./readme/DevFlow-ERDiagram.png)

The database is structured around core entities:

- `users`, `user_profiles`, `user_types`: handle authentication, roles (free, paid, researcher), and user metadata.  
- `repositories`, `commits`, `commit_suggestions`: store repo details, commit history, and AI-enhanced commit messages.  
- `cicd_pipelines`, `pipeline_runs`: manage CI/CD definitions and execution logs.  
- `analytics`, `metrics`: capture code quality stats, test coverage, and usage trends.  
- `settings`: user preferences for themes, notifications, and third-party integrations.

<br><br>

<!-- Project Highlights -->
<img src="./readme/title4.svg"/>

### Project Highlights

- **Automated CI/CD pipelines** defined and executed directly from the UI.  
- **AI-powered commit suggestion engine** that refines messages and enforces best practices.  
- **Deep repository analytics** with visualizations for code health, test coverage, and activity trends.  
- **GitHub OAuth integration** for seamless authentication and repo access.  
- **Role-based access control** supporting free, paid, and researcher users.

<br><br>

<!-- Demo -->
<img src="./readme/title5.svg"/>

### Demo Screens (Web)

| Dashboard                                        | Repository View                                 | Commit History                                  |
| ------------------------------------------------ | ----------------------------------------------- | ------------------------------------------------ |
| ![Dashboard](./readme/demo/dashboard.png)        | ![Repository](./readme/demo/repository.png)     | ![Commits](./readme/demo/commits.png)            |

| Profile Page                                     | Analytics Page                                  |
| ------------------------------------------------ | ----------------------------------------------- |
| ![Profile](./readme/demo/profile.png)            | ![Analytics](./readme/demo/analytics.png)       |

<br><br>

<!-- Development & Testing -->
<img src="./readme/title6.svg"/>

### Development & Testing

This section highlights how DevFlow structures its core logic, validation, and automated tests.

- **Services:** Business logic for commit analysis, pipeline orchestration, and analytics is encapsulated in service classes following SOLID principles.  
- **Validation:** All requests pass through dedicated form request classes to enforce data integrity and security.  
- **Testing:** Unit tests cover the commit suggestion engine and integration tests validate end-to-end CI/CD workflows.

| Services                                             | Validation                                         | Testing                                           |
| ---------------------------------------------------- | -------------------------------------------------- | ------------------------------------------------- |
| ![Service](./readme/services/CommitService.png)      | ![Validation](./readme/services/CommitRequest.png) | ![Test](./readme/services/CommitTest.png)         |

<br><br>

<!-- Deployment -->
<img src="./readme/title7.svg"/>

### Deployment Overview

- The DevFlow frontend and backend are containerized with Docker for consistency across environments.  
- CI/CD is orchestrated via GitHub Actions, automating tests and deployments on every push to main.  
- The application is hosted on AWS EC2:

  - **Staging:** `http://35.180.8.108`  
  - **Production:** `http://35.180.36.19`

| Postman API – List Repositories                         | Postman API – Create Commit                          | Postman API – Trigger Pipeline                       |
| ------------------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| ![List Repos](./readme/api/list_repositories.png)        | ![Create Commit](./readme/api/create_commit.png)     | ![Trigger Pipeline](./readme/api/trigger_pipeline.png) |

<br><br>
