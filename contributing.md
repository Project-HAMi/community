# Contributing to HAMi

Welcome to the HAMi community! We’re excited that you want to contribute. Whether you're here to fix bugs, add new features, or improve documentation, your help is valuable.

## Table of Contents
- [Before You Get Started](#before-you-get-started)
  - [Code of Conduct](#code-of-conduct)
  - [Community Expectations](#community-expectations)
- [Getting Started](#getting-started)
- [Your First Contribution](#your-first-contribution)
  - [Find Something to Work On](#find-something-to-work-on)
  - [File an Issue](#file-an-issue)
- [Contributor Workflow](#contributor-workflow)
  - [Creating Pull Requests](#creating-pull-requests)
  - [Code Review](#code-review)
- [Tell the world you're using HAMi](#tell-the-world-youre-using-hami)

## Before You Get Started

### Code of Conduct
Please read and follow our [Code of Conduct](CODE-OF-CONDUCT.md). It outlines the expectations for respectful and collaborative behavior within the community.

### Community Expectations
HAMi is driven by a diverse and inclusive community. We strive to foster a welcoming, productive, and friendly environment where contributors of all backgrounds can participate and grow.

## Getting Started

To contribute to HAMi, follow these simple steps:
1. **Fork the Repository** – Click the "Fork" button in the top-right corner of the GitHub repository.
2. **Make Your Changes** – Clone your fork, create a branch, and make the necessary code changes.
3. **Submit a Pull Request (PR)** – Once your changes are ready, open a pull request to the main repository.

## Your First Contribution

### Find Something to Work On
We always need help with various tasks, including fixing bugs, improving documentation, or adding new features. Here’s how you can get started:

#### Find a Good First Topic
Look for issues marked as "good first issue" or "help wanted." These issues are typically beginner-friendly and don’t require deep knowledge of the codebase. You can find these labels in the [issues section](https://github.com/Project-HAMi/HAMi/issues).

#### Work on an Issue
When you find an issue you'd like to work on, comment on the issue to let the maintainers know you're interested. They will assign the issue to you and guide you if needed.

### File an Issue
If you notice a bug or improvement area, we encourage you to file an issue. Ensure it is submitted under the appropriate sub-repository of HAMi. 

**Example:** A bug or feature request for the main HAMi repository should be opened in [Project-HAMi/HAMi](https://github.com/Project-HAMi/HAMi/issues).

Please follow the submission guidelines provided for creating a clear, actionable issue.

## Contributor Workflow

Here’s the basic flow for contributing to HAMi:

1. **Create a Topic Branch** – Create a branch from the main branch (`master`) for your changes.
2. **Make Logical Commits** – Break your work into smaller, logical commits that address specific changes.
3. **Push Changes** – Push your changes to your fork on GitHub.
4. **Submit a Pull Request** – Open a pull request from your fork to the main repository.

### Creating Pull Requests
When creating a pull request, please ensure you:

- Provide a clear description of the changes.
- Link the PR to the relevant issue if applicable.
- Ensure that your code is well-tested.
- Run the following local checks before submitting:
  - `make verify` – Make sure your changes pass all tests and format checks.

If the PR is small and manageable, it’s easier for the reviewers to give feedback promptly.

### Code Review
After submitting a PR, it will be reviewed by a maintainer. Here are some tips to make it easier for your PR to get accepted:

- Follow good coding practices. Refer to [Go code review comments](https://github.com/golang/go/wiki/CodeReviewComments) for style guidelines.
- Write meaningful commit messages that explain the "why" behind your changes. [Best practices for commit messages](https://chris.beams.io/posts/git-commit/) are a great resource.
- If your PR involves a large change, break it down into smaller, logical pieces that make incremental improvements. This helps reviewers follow the logic of your changes and ensures easier acceptance.

## Tell the world you're using HAMi

Running HAMi in production? Add yourself to our [Adopters](./adopters.md) page!

If you'd like a full case study interview, [create an issue](https://github.com/Project-HAMi/HAMi/issues/new), and we'll get in touch!