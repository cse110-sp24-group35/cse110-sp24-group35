# Netlify

## Context and Problem Statement
There can be many different builds of the same application throughout development process. Like production, development, nightly, etc. However, GitHub pages only allows building one entire site from one branch, which is not ideal.

## Decision Drivers
* Multiple deployments for different branches, ideally an automated deployment for each pull request so other team members can easily have a preview.

## Considered Options
* Netlify
* Vercel

## Decision Outcome
* Use Netlify to create development builds and feature builds. When a team members creates / updates the pull request, Netlify will automatically build a deployment based on that specific branch.
* Maintain the usage of GitHub pages for production build since Netlify has bandwidth limitation.