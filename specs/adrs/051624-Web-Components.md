# WebComponents

## Context and Problem Statement
It is necessary to not create redundant component references in a vanilla html + js project. Although with frameworks like React / Vue / Angular, components are intuitively meant to be reused across the application, it is easy to not follow such pattern with HTML. Therefore, utilizing WebComponent to properly scope and reuse common components across the entire application.

## Decision Drivers
* Improves code quality and readability
* Increases user experience due to less application size from reusing the components
* Better developer experience from scoped components (e.g. minimum style pollution)

## Considered Options
* WebComponents

## Decision Outcome
* Use WebComponents to implement majority of our customized components in the final project