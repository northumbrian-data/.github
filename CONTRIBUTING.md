# gliff.ai Contribution Guide

👋 **Hello there! Thanks for your interest in contributing!** 👋

The purpose of this guide is to ensure all contributors have a unified approach to contributing to all projects within the [gliff.ai](https://gliff.ai) space.

[gliff.ai](https://gliff.ai) is a small company aiming to help get healthcare and life science AI products regulated with a focus on privacy and security; fairness, accountability and transparency; all by keeping experts in the loop to ensure high quality outputs for real people and solutions across the world. Because the [gliff.ai team](https://gliff.ai/about/) is small, we look for the help of volunteer developers like you to contribute to our open-source code ensuring [gliff.ai](https://gliff.ai) can have the best and biggest positive impact possible.

Each repository has one of two topic tags to help you and fellow contributors understand which repositories [gliff.ai](https://gliff.ai) is open to contributions outside of our team. They are:

- **contributions-welcome** – We welcome all types of contributions on this repository!
- **no-contributions** – This repository does not accept most contributions unfortunately! However, an issue can still be raised if you recognise a problem you wish to bring to the gliff.ai teams attention.

👍🎉 **Thank you from the gliff.ai team for your interest and hopefully taking the time to contribute!** 🎉👍

## Table of Contents

Looking for something specific? 🔍

- [Introduction](#gliffai-contribution-guide)
- [Code of Conduct](#code-of-conduct)
- [Create an Issue](#create-an-issue)
- [Create a Pull Request](#create-a-pull-request)
- [Linting, Formatting and Testing](#linting-formatting-and-testing)
- [Commit Best Practices and Naming Conventions](#commit-best-practices-and-naming-conventions)
- [Assigning Reviewers Best Practices](#assigning-reviewers-best-practices)
- [Labels](#labels)
- [Contact](#contact)

## Code of Conduct

[{{back to navigation}}](#table-of-contents)

All projects and contributors are governed by the [gliff.ai Code of Conduct](https://github.com/gliff-ai/.github/blob/main/CODE_OF_CONDUCT.md) 📝. By contributing, you are expected to uphold this code to ensure a positive and welcome community space for all.

Please report unacceptable behavior ⚠️ to the gliff.ai team at [contact@gliff.ai](mailto:contact@gliff.ai?subject=Report%20GitHub%20Behavior) or on GitHub.

## Create an Issue

[{{back to navigation}}](#table-of-contents)

Our team uses 4 templates for creating issues across gliff.ai repositories, and we would appreciate you also using these and filling them out with as much detail as you are able to provide. The templates include:

- **Bug Report** – report any bugs whether technical or visual (the “bug” label will be automatically applied). 
- **Feature/Enhancement Request** – request any new features or enhancements of current features (the “enhancement” label will be automatically applied).
- **Test Request** – request a new test not currently available (the “test” label will be automatically applied).
- **Security Vulnerability** – report a suspected vulnerability which risks the security of our code (the “vulnerability” label will be automatically applied, and two gliff.ai team members will be automatically assigned). Read the [gliff.ai Security Policy](https://github.com/gliff-ai/.github/blob/main/SECURITY.md) to learn more!

Please remember to first determine which repository the issue should be raised in, then [search the gliff.ai repositories](https://github.com/search?q=user%3Agliff-ai+is%3Aissue+is%3Aopen) to ensure the issue you want to open is not already open! 

## Create a Pull Request

[{{back to navigation}}](#table-of-contents)

The **Pull Request** template should be filled out as much as possible. Your pull request should include a summary of the changes you have made and your motivation behind them. Please list any dependency changes, added tests, documentation changes, database changes (if applicable) and complete our checklist to ensure you have completed all the necessary steps.

Please remember to first determine which repository the pull request should be created in, then [search the gliff.ai repositories](https://github.com/search?q=user%3Agliff-ai+is%3Apr) to make sure the pull request you want to create is **not already open or closed**! 

After you submit your pull request, please assign 3 or less reviewers following our [assigning reviewers best practices](#assigning-reviewers-best-pratices) and assign any [labels](#labels) you think are applicable. Please also verify that all status checks are passing. If for some reason they are failing and you believe it’s unrelated to your change or unsure why, please leave a comment on the pull request explaining this and someone on the gliff.ai team will further investigate.

## Linting, Formatting and Testing

[{{back to navigation}}](#table-of-contents)

For linting and formating our team uses [flake8](https://github.com/PyCQA/flake8) and [black](https://github.com/psf/black) for linting and auto-formatting our Python code alongside [pytest](https://docs.pytest.org/en/6.2.x/) for our Python code tests, or [eslint](https://eslint.org) and [prettier.io](https://prettier.io) for linting and auto-formatting our TypeScript code alongside [jest with react-testing-library](https://jestjs.io/docs/tutorial-react) for our TypeScript code testing.

For system and visual testing our team uses [BrowserStack](https://www.browserstack.com) – specifically [Automate with Selenium](https://www.browserstack.com/automate), and [Percy](https://www.browserstack.com/percy) Snapshots together to test at scale the platform works as antipicated.

_Any further or alternative specifics and configuration files can be found in each of our repositories._

If you create a pull request, your contributed code will automatically be linted, formatted and tested by the GitHub Action we have set up. New code should always use the same linters and formatters the gliff.ai reposorities currently use. We would also really appreciate new code to come with new tests, where appropriate, to be run against all existing tests!

## Commit Best Practices and Naming Conventions

[{{back to navigation}}](#table-of-contents)

Our commit best practises encourage creating small and frequent commits with clear log messages while editing the source code. This ensures commits are focused and any changes are easily understood and revertible if something goes wrong.

Commit messages should indicate the type and include a short summary of the commit using the following conventions:

- **feat**: The new feature you're adding to a particular application.
- **fix**: A bug fix.
- **build**: Development changes related to the build system (involving scripts, configurations or tools) and package dependencies.
- **refactor**: Refactoring a specific section of the codebase.
- **test**: Everything related to testing.
- **docs**: Everything related to documentation.
- **chore**: Regular code maintenance and/or style changes/formatting.

For example, “feat: add new icon svg file” or “fix: lint errors”.

One-line commit messages are perfect for small changes, but larger changes should include a paragraph describing what has changed and what is its impact alongside.

## Assigning Reviewers Best Practices

[{{back to navigation}}](#table-of-contents)

The key rule with assigning reviewers is we maintain a **maximum of 3 reviewers on a single pull request**. This comes off our team learning from the State of the Octoverse 2021 report where this rule ensures fast reviews. Now the question is, who should you assign?

The gliff.ai team active on our various projects are known as the **“techteam”** and subdivided into 4 self-explanatory smaller teams:

- **backend**: Requests 2 random members from this 4 person sub-team.
- **frontend**: Requests 2 random members from this 6 person sub-team.
- **ui-ux**: Requests 1 specific member from this 2 person sub-team.
- **documentation**: Requests 2 random members from this 4 person sub-team.

As best practice we recommended assigning reviewers using which team(s) are best involved with the content and solution of your pull request (e.g. UI bug fix (frontend & ui-ux), or new unit test (backend)).

## Labels

[{{back to navigation}}](#table-of-contents)

Each issue and pull request should be assigned one or multiple labels depending on the content. We actively encourage all contributors to attach labels onto any issues and pull requests they open to categorise tasks and problems, making it visually easier to find and understand which ever task or problem is being handled in each issue and pull request.

Our repositories have 7 label categories which are subdivided into their own labels.

**Welcome**  (white)
- [good-first-issue](https://github.com/search?q=user%3Agliff-ai+label%3Agood-first-issue+is%3Aopen) – Perfect for new contributors.

**Status**  (orange)
- [design-complete](https://github.com/search?q=user%3Agliff-ai+label%3Adesign-complete+is%3Aopen) – Design ready for implementation.
- [priority](https://github.com/search?q=user%3Agliff-ai+label%3Apriority+is%3Aopen) – This issue should be a priority for completion.

**Update**  (light grey)
- [dependencies](https://github.com/search?q=user%3Agliff-ai+label%3Adependencies+is%3Aopen) – Pull requests that update a dependency file.
- [javascript](https://github.com/search?q=user%3Agliff-ai+label%3Ajavascript+is%3Aopen) – Pull requests that update Javascript code.

**Problem**  (red)
- [bug](https://github.com/search?q=user%3Agliff-ai+label%3Abug+is%3Aopen) – Something isn’t working or looking right.
- [vulnerability](https://github.com/search?q=user%3Agliff-ai+label%3Avulnerability+is%3Aopen) – Security vulnerability report only.
- [question](https://github.com/search?q=user%3Agliff-ai+label%3Aquestion+is%3Aopen) – Further information is requested and/or required.

**Improvement**  (blue)
- [feature](https://github.com/search?q=user%3Agliff-ai+label%3Afeature+is%3Aopen) – New feature request.
- [enhancement](https://github.com/search?q=user%3Agliff-ai+label%3Aenhancement+is%3Aopen) – New feature request.
- [test](https://github.com/search?q=user%3Agliff-ai+label%3Atest+is%3Aopen) – Anything related to testing or tests.
- [ui/ux](https://github.com/search?q=user%3Agliff-ai+label%3Aui%2Fux+is%3Aopen) – User interface / user experience of the platform.
- [deployment](https://github.com/search?q=user%3Agliff-ai+label%3Adeployment+is%3Aopen) – Anything relating to deployment.
- [documentation](https://github.com/search?q=user%3Agliff-ai+label%3Adocumentation+is%3Aopen) – Improvements or additions to documentation.

**Release**  (yellow)
- [major](https://github.com/search?q=user%3Agliff-ai+label%3Amajor+is%3Aopen) – Major release.
- [minor](https://github.com/search?q=user%3Agliff-ai+label%3Aminor+is%3Aopen) – Minor release.
- [patch](https://github.com/search?q=user%3Agliff-ai+label%3Apatch+is%3Aopen) – Patch release.

**Inactive**  (black)
- [wont-fix](https://github.com/search?q=user%3Agliff-ai+label%3Awont-fix+is%3Aopen) – This will not be worked on.
- [duplicate](https://github.com/search?q=user%3Agliff-ai+label%3Aduplicate+is%3Aopen) – This issue or pull request already exists.

These labels are mostly consistent across gliff.ai repositories^ to make it easier for everyone while working across multiple. If you forget this don't worry, when you open your issue or pull request each label has a description!

**^ NOTE:** the [ROADMAP repository](https://github.com/gliff-ai/roadmap/blob/main/README.md) has its own unique labelling system.

## Contact

[{{back to navigation}}](#table-of-contents)

Need some help? 🤔 Have a question? 🧠 \
Reach out to the gliff.ai team at [community@gliff.ai](mailto:community@gliff.ai?subject=[GitHub]) or on GitHub.
