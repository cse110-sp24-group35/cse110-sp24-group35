# Style Implementation

## Context and Problem Statement
There needs to be a balance between "using Shadow DOM to prevent style pollution from other components" and maintaining HTML size so the clients won't be lagged as much.

## Decision Drivers
* Be friendly to devices that don't like big HTML files
* Avoid style pollution as much as possible with Shadow DOM

## Decision Outcome
* Use Shadow DOM and internal styling for components that will be only rendered once (for example, Journal editors and file explorers)
* Use appropriate scoped CSS styles for components that need to be rendered multiple times in same page (for example, Kanban task cards)