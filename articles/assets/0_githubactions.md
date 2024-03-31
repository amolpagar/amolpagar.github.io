---
permalink: articles/getting-started-with-github-actions
topic: getting-started-with-github-actions
---

# Getting Started with GitHub Actions

GitHub Actions allows you to automate your workflow directly from your GitHub repository. You can build, test, and deploy your code right from GitHub. In this tutorial, we'll cover the basics of setting up a GitHub Actions workflow.

## Step 1: Create a Workflow File

Create a new directory named `.github/workflows` in your repository if it doesn't already exist. Inside this directory, create a new file named `main.yml`. This file will define your workflow.

```yml
name: My Workflow
on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2
    - name: Run a one-line script
      run: echo Hello, world!

```

This workflow will run whenever you push to your repository and will echo "Hello, world!" as a demonstration.

## Step 2: Commit and Push
Commit your changes and push them to your repository.

## Step 3: View the Workflow
Visit the "Actions" tab in your repository on GitHub. You should see your workflow running or queued. Click on the workflow to view details and logs.

## Step 4: Customize Your Workflow
You can customize your workflow by adding more jobs, steps, or actions. Explore the GitHub Actions Marketplace for pre-built actions that you can use in your workflows.

Congratulations! You've set up your first GitHub Actions workflow. Explore more features and possibilities to automate your development workflow further.