# Service Worker

## Context and Problem Statement
Local-first is a very important aspect in web application to enhance performance, reliability, and user experience (e.g. graceful degradation). We can use Service Worker to achieve offline functionality, caching, and background synchronization to ensure users can access content without a stable internet connection.

## Decision Drivers
* Improve performance
* Enhance reliability in low or no internet connectivity environment

## Considered Options
* Service Worker

## Decision Outcome
* Use ServiceWorker API to enable offline functionality and improve local-first experience for our website