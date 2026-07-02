# Jenkins GitHub Webhook Demo with SCM

## Objective

This project demonstrates Continuous Integration (CI) using GitHub Webhooks with SCM and Jenkins.

## Workflow

1. Developer commits code.
2. Code is pushed to GitHub.
3. GitHub Webhook notifies Jenkins.
4. Jenkins automatically triggers the pipeline.
5. Jenkins checks out the latest code.
6. Maven builds the project.
7. Build completes successfully.

## Technologies Used

- Git
- GitHub
- Jenkins
- Maven
- Java 17

## Expected Result

Whenever new code is pushed to GitHub, Jenkins automatically starts a new build without manually clicking **Build Now**.
