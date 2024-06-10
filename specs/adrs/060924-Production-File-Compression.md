# File Compression

## Context and Problem Statement
Less file size transferred = faster render time. However, for development purpose it is not ideal to have compressed scripts / styles / html served but instead the original version should've been there. The compression should only live in production.

## Decision Drivers
* Production needs to have the most minified files to serve clients better

## Decision Outcome
* Use [CSSO](https://github.com/css/csso-cli), [Terser](https://github.com/terser/terser), and [HTML-Minifier](https://kangax.github.io/html-minifier/) to compress CSS, JavaScript, and HTML **in the production deployment step only** in the continuous deployment pipeline. In this way, development builds won't be affected yet the production builds still benefit from the minified served files.