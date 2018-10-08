# Contributing to Full Stack Interview Questions & Answers

Please take a moment to review this document in order to make the contribution
process easy and effective for everyone involved.

## Submitting New Questions & Answering Questions

You are welcome to make improvements to existing answers, answer unanswered questions and post new questions / answers. Whenever possible, add a list of references and supplementary material. 
Follow the existing format of markdown and code.

## Using the issue tracker

The [issue tracker](https://github.com/monkey3310/full-stack-interview/issues) is
the preferred channel for spelling mistakes, errors or any general feedback. If you want to work on an existing issue, please add a comment in it stating your interest so it can be assigned to you. That way duplicate PRs can be avoided.

## Pull requests

Please adhere to the coding conventions used throughout the project (spelling, indentation, punctuation etc.).

Adhering to the following process is the best way to get your work included in the project:

1. [Fork](https://help.github.com/articles/fork-a-repo) the project, clone your fork, and configure the remotes:

   ```bash
   # Clone your fork of the repo into the current directory
   git clone https://github.com/<your-username>/full-stack-interview.git
   # Navigate to the newly cloned directory
   cd full-stack-interview
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/monkey3310/full-stack-interview.git
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout master
   git pull upstream master
   ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream master
   ```

5. Squash your commits down to a single one (we want to keep the master branch nice and clean)

5. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
    with a clear title and description.

## Code of Conduct

Please note our Code of Conduct and follow it in all your interactions with the project.

**IMPORTANT**: By submitting patches, you agree to allow the project owners to license your work under the terms of the [MIT License](../LICENSE.md).
