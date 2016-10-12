---
layout: default
---
* TOC
{:toc}

# Code
 * Get a [GitHub](https://github.com) account.
 * Fork [DaisyDiff](https://github.com/DaisyDiff/DaisyDiff)
 * DaisyDiff uses Continuous Integration (CI). That runs unit tests automatically on every commit. Next to each successful run you see a green tick at [DaisyDiff commits](https://github.com/DaisyDiff/DaisyDiff/commits/master). That links to an automatic report of running unit tests.
 * Set up CI for your repository: _github.com/your-name/your-fork-name_ > Settings > Integrations & services > Add service > Travis CI. DaisyDiff also works with Jenkins: [https://qa.nuxeo.org/jenkins/job/Vendor/job/daisydiff/](https://qa.nuxeo.org/jenkins/job/Vendor/job/daisydiff/) and [https://github.com/nuxeo/nuxeo-diff](https://github.com/nuxeo/nuxeo-diff). If you make it work with other CI service, please update this.
 * Commit to your fork. Create pull requests.

# Documentation
To update this documentation, follow [DocumentationStandard](http://selite.github.io/DocumentationStandard) but replace 'selite' with 'daisydiff'.

Similar to the above, fork [DaisyDiff.github.io](https://github.com/DaisyDiff/DaisyDiff.github.io). Commit to your fork. Create pull requests.

If you use an IDE other than NetBeans, and if setting up Maven/unit tests is not trivial, please do document how to configure your IDE.