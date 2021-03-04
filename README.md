# Trivadis Good Practice Template

<!-- markdownlint-disable MD013 -->
[![markdown-lint](https://github.com/Trivadis/good-practice-template/actions/workflows/mdlint.yml/badge.svg)](https://github.com/Trivadis/good-practice-template/actions/workflows/mdlint.yml) [![Doc Build](https://github.com/Trivadis/good-practice-template/actions/workflows/pandoc_builds.yml/badge.svg)](https://github.com/Trivadis/good-practice-template/actions/workflows/pandoc_builds.yml)

Welcome to the *Good Practice Template*. This repository is a template for various *Good Practice Guidelines*. It contains the necessary structures, base documents and CI pipelines for the automatic creation of these documents. When creating a new *Good Practice Guidelines*, this repository can be used directly as a template. Corresponding links and references in the Markdown files have to be adapted to the new repository afterwards. In general, these are just the links in this [README.md](README.md).

## Downloads and Latest Builds

The official release documents are always attached to the releases. See also the
[release](https://github.com/Trivadis/good-practice-template/releases) page of
this repository.

- Word document [en](https://github.com/Trivadis/good-practice-template/releases/download/v0.1.0/tvd-good-practice-template_en.docx), [de](https://github.com/Trivadis/good-practice-template/releases/download/v0.1.0/tvd-good-practice-template_de.docx)
- PDF document [en](https://github.com/Trivadis/good-practice-template/releases/download/v0.1.0/tvd-good-practice-template_en.pdf), [de](https://github.com/Trivadis/good-practice-template/releases/download/v0.1.0/tvd-good-practice-template_de.pdf)
- [Source code](https://github.com/Trivadis/good-practice-template/archive/v0.1.0.zip/)

Nightly Builds respectively builds on commit are attached as artefacts to the
GitHub workflow, see [Generated Documents](https://nightly.link/Trivadis/good-practice-template/workflows/pandoc_builds/main/Generated%20Documents.zip).

## Files and Folders

- [de](de) German documentation files.
- [en](en) English documentation files.
- [images](images) Images and logo files.
- [templates](templates) Various pandoc templates.
- [AUTHOR_GUIDE](AUTHOR_GUIDE.md) General author's guide to *Good Practices*.
  This has to be adapted to the corresponding guideline.
- [CHANGELOG](CHANGELOG.md) Change log for the *Good Practices*.
- [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) Code of conduct for the interaction
  and cooperation within the framework of this project.
- [CONTRIBUTING](CONTRIBUTING.md) Guide how to contribute to this project.

## Releases and Versions

You find all official releases and release information on the GitHub release page [here](https://github.com/Trivadis/good-practice-template/releases). As well documented in the [CHANGELOG](CHANGELOG.md).

The versioning and release tags follow the [semantic versioning](https://semver.org/).
A version number is specified by MAJOR.MINOR.PATCH, increase the:

- *MAJOR* version when you make incompatible API changes,
- *MINOR* version when you add functionality in a backwards compatible manner, and
- *PATCH* version when you make backwards compatible bug fixes.

Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

## Issues and Enhancements

Please file your bug reports, enhancement requests, questions and other support requests within [Github's issue tracker](https://help.github.com/articles/about-issues/).

- [Questions](https://github.com/Trivadis/good-practice-template/issues?q=is%3Aissue+label%3Aquestion)
- [Open enhancements](https://github.com/Trivadis/good-practice-template/issues?q=is%3Aopen+is%3Aissue+label%3Aenhancement)
- [Open bugs](https://github.com/Trivadis/good-practice-template/issues?q=is%3Aopen+is%3Aissue+label%3Abug)
- [Submit new issue](https://github.com/Trivadis/good-practice-template/issues/new)

## How to Contribute

It is highly recommended to take into account [CONTRIBUTING](CONTRIBUTING.md) and [AUTHOR_GUIDE](AUTHOR_GUIDE.md) when contributing to this *Good Practice*. However contributing covers the following steps.

1. Describe your idea by [submitting an issue](https://github.com/Trivadis/good-practice-template/issues/new)
2. [Fork this respository](https://github.com/Trivadis/good-practice-template/fork)
3. [Create a branch](https://help.github.com/articles/creating-and-deleting-branches-within-your-repository/), commit and publish your changes and enhancements
4. [Create a pull request](https://help.github.com/articles/creating-a-pull-request/)

## License

Trivadis/good-practice-template
 is licensed under the Apache License 2.0. You may obtain a copy of the License at <http://www.apache.org/licenses/LICENSE-2.0>.
