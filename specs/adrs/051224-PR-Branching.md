# PR, Branching

## Context and Problem Statement

Managing clean and well-maintained source repository is very hard as an objective in a team environment. How do we exactly do that across numerous pull requests and code reviews? What can we do to enforce strict policies to properly scope everyone's repository while making it very easy to merge all of them together at the end?

## Decision Drivers
* Maintain proper consistency and assert clarity for team members, leaders, TAs, and professor
* Assure quality and performance of the application

## Considered Options
* GitHub Pull Request Template
* CodeClimate for quality check
* CodeQL for vulnerability check

## Decision Outcome
* Use [Pull Request Template](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates#pull-request-templates) to submit a proper Pull Request
* The template includes following: 
  * Changes
  * Steps to test specific changes introduced
  * Screenshots (if applicable)
  * Checklist
* Everyone should use `first/feature` to own their own branch. For example: `allen/issue-8`.
* [Squash the commits](https://www.freecodecamp.org/news/git-squash-commits/) when the Pull Request looks ok and is going to be merged.
* PR Policy:
  * When a PR is in draft state, no policies will be enforced.
  * However, when a PR gets published, the following will be addressed:
    * All automated tests shall pass locally (including Unit & E2E & Linters)
    * Add new E2E and Unit tests to address the changes made
    * Manual testing has been performed according to the provided instructions
    * Code follows team's coding style, convention and standards
    * Test coverage exceeds 90% overall (as reported by NYC library)
    * Documentation has been updated to reflect relevant changes
    * Codebase passes CodeQL (for vulnerability) and CodeClimate (for quality) checks
    * Reviewed and approved by team leader

