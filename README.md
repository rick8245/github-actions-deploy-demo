# GitHub Actions Deploy Demo

This repository showcases a GitHub Actions workflow that builds a Java Gradle project and deploys the resulting package using the `digital-ai/github-actions-deploy` custom action. This guide will walk you through the setup and functionality of the workflow.

---

## Project Overview

This project is a straightforward Java Gradle application specifically designed to illustrate the power of GitHub Actions for CI/CD. The workflow performs the following key steps:

1.  **Code Checkout**: Retrieves the latest code from your repository.
2.  **JDK Setup**: Configures **JDK 17** for the build environment, ensuring compatibility with your project.
3.  **Gradle Wrapper Permissions**: Grants execute permissions to the Gradle wrapper script (`gradlew`), which is essential for running Gradle commands within the workflow.
4.  **Project Build**: Compiles and packages the Java project using **Gradle**.
5.  **Package Creation, Publishing, and Deployment**: Utilizes the `digital-ai/github-actions-deploy` action to create a deployable package, publish it, and then deploy it to your specified target environment.

---

## Workflow Files

All workflow definitions are located in the `.github/workflows` directory of this repository. You can review these files to understand the precise configuration and steps involved in the deployment process.

---

## Running the Workflow

This workflow is configured for manual triggering via the GitHub Actions interface, leveraging the `workflow_dispatch` event. To execute the workflow:

1.  Navigate to the **Actions** tab within your GitHub repository.
2.  From the "All workflows" sidebar, select the specific workflow you wish to run.
3.  Click the **Run workflow** button, usually found in the top right corner of the workflow details page.

---

## Conclusion

This demo project effectively illustrates how to integrate the `digital-ai/github-actions-deploy` action into your GitHub Actions workflows for streamlined building and deploying of Java Gradle projects. It provides a solid foundation for automating your software delivery pipeline.