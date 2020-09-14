- [Title](#title)
- [Conference](#conference)
- [Status](#status)
- [Artifacts](#artifacts)
- [Abstract](#abstract)
- [Detailed description](#detailed-description)
- [Notes](#notes)

# Title

<!--- Proposal title -->

Intro to baking: Simple PyPI

[⬆️ Back to top](#title)

# Conference

<!--- Conference name and year + links -->

[dotPy 2020](https://www.dotpy.io/)

CFP Link: https://www.dotconferences.com/cfp

[⬆️ Back to top](#title)

# Status

<!--- 🎉 Accepted, 🚮 Rejected, 🚪 Withdrawn -->

🎉 Accepted

However the conference was cancelled because of COVID-19 :(

[⬆️ Back to top](#title)

# Artifacts

<!--- Links to recording, speaker page, slides etc. But also reason for rejection, if any. -->

[GitHub repository](https://github.com/kimadeline/pypi-simple-scraping), also at https://aka.ms/simple-pypi

[Slides](https://speakerdeck.com/kimadeline/simple-pypi)

[⬆️ Back to top](#title)

# Abstract

**Length limit:** N/A

Have you ever wondered how many PyPI package names contain the word 'python', or what the average package name length is? Impress your colleagues, friends and family by answering these questions using PyPI's simple API!

[⬆️ Back to top](#title)

# Detailed description

## Why this talk

<!-- Optional, depends on the proposal -->

This lightning talk focuses on PyPI and how you can extract information from it, so it would be a good fit for people interested in web scraping, package-related automation, or simply curious about PyPI.

[⬆️ Back to top](#title)

## Audience

<!-- Optional, depends on the proposal -->

N/A

[⬆️ Back to top](#title)

## Talk outline

<!-- Include time breakdown if any -->

- Title: simple 🥧🕵️‍♀️
- Before we start: PyPI/warehouse, PyPA, pypy in the corner
- Now the title was simple PyPI, let's look at it
- pypi.org/simple: HTML file with anchors to links to packages (show an excerpt)
- spec: PEP503
- You can extract some "fun facts" out of it -> show facts
- What happens if you click on one of these links? Let's take a random package like Django/ptvsd/debugpy/pydevd/black/pytest/numpy/scipy
- You get a list of downloadable files
- What does the filename tell us? if it's a tarball or a zip file -> source files, else: interpreter, ABI (what's ABI) and platform
- Great and all that, and you can parse the filenames yourselves to extract that metadata (manually or using the packaging module), if only there was a way to retrieve this metadata in, let's say an object notation
- Here comes the JSON API: `pypi/<package name>/json`
- spec: PEP566
- What it looks like (example with django): info (latest version), releases and urls (latest version)
- you can get metadata for a specific version in the "info" key with `<package name>/<version>/json`
- why would you need that? if you want to bundle packages in your product (think, OSes) so you're monitoring for the latest release of some packages, or for you to get a notification inside your IDE or product that there are package updates available
- questions? comments? want to code to extract the "fun facts"? https://aka.ms/simple-pypi or https://github.com/kimadeline/pypi-simple-scraping (will upload the slides there later this evening)

_References:_

- Regular dump of PyPI database: https://github.com/pypa/warehouse/issues/1478
- Would people be interested in a daily download of PyPI metadata until #1478 is implemented https://twitter.com/brettsky/status/1200536491388100608
- PyPI keyword stats: https://github.com/uranusjr/packaging-metadata-comparisons/blob/master/topics/keywords.md
- Core metadata specifications: https://packaging.python.org/specifications/core-metadata/
- Add API endpoint to get latest version of all projects: https://github.com/pypa/warehouse/issues/347
- JSON API documentation: https://warehouse.readthedocs.io/api-reference/json/
- PyPA projects: https://packaging.python.org/key_projects/#pypa-projects

[⬆️ Back to top](#title)

# Notes

<!---
Optionally, anything that doesn't fit in other sections:
Any additional equipment you might need, whether or not you’ve given this talk before, etc.
-->

**Talk type:** Lightning talk

**Talk duration:** 4 minutes

[⬆️ Back to top](#title)
