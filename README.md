# DevOps Interview Questions and Answers

1. What is Azure Boards?

Azure Boards is a project management and tracking tool in Azure DevOps used to plan, track, and discuss work across teams. It helps teams manage work items like user stories, bugs, tasks, and epics using Kanban or Scrum boards.

Example:
- A team creates a user story: “As a user, I want to log in with email and password.”
- It is assigned to a developer and moved from “To Do” to “In Progress” to “Done.”

2. What is Jira?

Jira is a popular issue and project tracking tool by Atlassian. It is widely used for Agile project management, bug tracking, and sprint planning.

Example:
- A QA tester reports a bug: “Login button not working on mobile.”
- The bug is assigned to a developer, the fix is made, and it is marked resolved.

3. What is Trello?

Trello is a simple visual project management tool based on boards, lists, and cards. It is easy to use for small teams and personal projects.

Example:
- A board named “Website Launch”
- Lists: To Do, Doing, Review, Done
- Cards: “Create homepage,” “Test login,” “Publish article”

4. What are the different work items in Agile?

Common Agile work items are:

- Epic: Large body of work that contains many related features.
  Example: “Customer Portal Redesign”
- Feature: A significant capability delivered to users.
  Example: “User profile page”
- User Story: Short requirement from a user perspective.
  Example: “As a customer, I want to update my profile picture.”
- Task: A specific technical action.
  Example: “Create profile image upload API”
- Bug: Something broken in the product.
  Example: “Password reset email fails”
- Issue: A problem, risk, or blocker.
  Example: “Third-party API is down”

5. How do you organize work items on an Agile board?

Work items are organized on an Agile board by workflow stages such as:
- Backlog
- To Do
- In Progress
- In Review
- Done

Example:
- “Add login page” is in Backlog.
- A developer picks it and moves it to In Progress.
- A reviewer checks it and moves it to In Review.
- Once approved, it is marked Done.

This helps visualize progress and manage flow.

6. What are Azure DevOps dashboards?

Azure DevOps dashboards are customized views that show project metrics, progress, and status. They can include charts, widgets, KPI data, and build/test reports.

Example:
- A dashboard shows:
  - Number of open bugs
  - Sprint burndown
  - Build success rate
  - Completion of user stories

This gives stakeholders a quick overview of project health.

7. What are Azure Pipelines, and how do you create a pipeline?

Azure Pipelines is a CI/CD service that automates build, test, and deployment.

How to create a pipeline:
1. Go to Azure DevOps.
2. Select your project.
3. Go to Pipelines.
4. Click “New Pipeline.”
5. Choose your repository (GitHub, Azure Repos, etc.).
6. Select a template.
7. Configure YAML or classic pipeline.
8. Save and run.

Example:
- A .NET app is automatically built when code is pushed to GitHub.
- Unit tests run.
- The app is deployed to Azure App Service.

8. What are service connections, and how do you connect Azure DevOps to external services?

Service connections are secure links between Azure DevOps and external services such as Azure subscriptions, Docker Hub, GitHub, Kubernetes clusters, or cloud platforms.

Example:
- To deploy to Azure:
  - Create a service connection in Azure DevOps
  - Authenticate with the Azure subscription
  - Use that connection in the pipeline for deployment

This avoids hardcoding secrets in YAML files.

9. What is GitOps?

GitOps is a way of managing infrastructure and application deployment using Git as the source of truth. Changes are made in Git, and automation applies them to the environment.

Example:
- A developer updates Kubernetes YAML files in Git.
- A GitOps tool such as Argo CD notices the change.
- The cluster is automatically updated to match the Git state.

This makes deployments consistent, reviewable, and auditable.

10. What are the advantages and disadvantages of DevOps?

Advantages:
- Faster software delivery
- Better collaboration between teams
- Automation reduces manual work
- Better quality through continuous testing
- Faster bug detection and fixing

Disadvantages:
- Initial setup can be expensive
- Requires skilled team members
- Tool integration may be complex
- Culture change is needed
- Automation failures can cause deployment issues if not monitored

11. What is the role and importance of DevOps in full-stack development?

DevOps plays a key role in full-stack development by connecting frontend, backend, database, and deployment workflows into a continuous process.

Importance:
- Automates builds and deployments
- Improves code quality through CI/CD
- Helps teams release updates faster
- Ensures the app works across environments
- Simplifies collaboration between developers and operations

Example:
- A full-stack app has frontend, Node.js API, database, and deployment pipeline.
- DevOps ensures code is built, tested, and deployed consistently.

12. What is the difference between Azure DevOps, Git, GitHub, and GitOps?

- Git: Version control system for tracking code changes.
  Example: git commit, git push

- GitHub: Cloud platform for hosting Git repositories and collaboration.
  Example: Pull requests, issues, code review

- Azure DevOps: Complete DevOps platform with boards, repos, pipelines, test plans, and artifacts.
  Example: CI/CD, sprint planning, release pipelines

- GitOps: Deployment model where Git defines the desired system state.
  Example: Argo CD syncs a cluster with the Git repository

In simple words:
- Git stores code history
- GitHub hosts code and collaboration
- Azure DevOps manages DevOps processes
- GitOps manages infrastructure using Git

13. What is the difference between Docker and containers? How do they help in DevOps?

- Container: A lightweight running instance of an application and its dependencies
- Docker: A platform/tool used to create, run, and manage containers

Example:
- A Node.js app depends on Node, libraries, and OS packages.
- Docker wraps the app into a container so it runs the same in development, testing, and production.

How they help in DevOps:
- Consistent environments
- Easier deployment
- Faster setup
- Better scalability
- Works well with CI/CD pipelines

14. What is the DevOps process? How does it work, and what are the architectures of Azure DevOps and GitOps?

The DevOps process typically works like this:
1. Plan
2. Develop
3. Build
4. Test
5. Deploy
6. Monitor
7. Improve

Example:
- A team plans a feature in Azure Boards.
- Developers code it in Git.
- Azure Pipelines builds and tests it.
- It is deployed using Azure DevOps or GitOps tools.
- Monitoring detects issues and feedback is used for the next improvement.

Azure DevOps architecture:
- Boards for planning
- Repos for code
- Pipelines for CI/CD
- Artifacts for package management
- Test Plans for testing

GitOps architecture:
- Git repository stores desired state
- CI/CD automation detects changes
- GitOps controller (such as Argo CD) syncs cluster state
- Kubernetes or cloud environment matches Git

Example:
- Kubernetes deployment YAML files are in Git.
- Argo CD pulls those files and applies them to the cluster automatically.

Conclusion:
DevOps is a culture and practice that combines development and operations to improve speed, quality, and collaboration. Tools like Azure DevOps, GitHub, Docker, and GitOps support this by automating and standardizing the software lifecycle.

If you want, I can also turn this into:
1. Short exam-style answers
2. 2-mark and 5-mark university answers
3. Very simple interview answers
4. A polished assignment format with headings and examples