# Static website deployment practice: reviewer guide

Static HTML/CSS files with a GitHub Actions deployment workflow.

## Start the review

Identify which source directory the workflow deploys and how a failed deployment would be investigated.

| Source | Review focus |\n| --- | --- |\n| [.github/workflows/deploy.yml](.github/workflows/deploy.yml) | Triggers, credentials, failure handling, and deploy conditions |\n| [.gitignore](.gitignore) | Implementation, assumptions, and operational boundaries |\n| [error.html](error.html) | Implementation, assumptions, and operational boundaries |\n| [index.html](index.html) | Implementation, assumptions, and operational boundaries |\n| [style.css](style.css) | Implementation, assumptions, and operational boundaries |\n| [website/error.html](website/error.html) | Implementation, assumptions, and operational boundaries |

## A useful interview walkthrough

1. State the problem and the specific part you implemented or changed.
2. Open the source above and follow one request, release, or failure from start to finish.
3. Show a reproducible result, including an actual failure and the observation that confirms recovery.
4. Explain one tradeoff and one limitation. Distinguish a local test from a live deployment.

## Evidence and limits

This guide is based on the default-branch source inspected on 16 October 2026. It is a source review, not a fresh deployment or a certification of every feature. Existing CI runs and tests should be checked at the commit being demonstrated. Do not present screenshots, inherited code, planned features, or old README statements as proof of a current deployment.
