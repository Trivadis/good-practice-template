# Changelog
<!-- markdownlint-disable MD013 -->
<!-- markdownlint-configure-file { "MD024":{"allow_different_nesting": true }} -->
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased] - 2021-02-25

### Added

### Changed

### Fixed

### Removed

## [0.2.0] - 2021-03-01

### Added

- Add support for boxes in PDF build using *Pandoc filters*.
- Add a pptx template [trivadis.pptx](templates/trivadis.pptx)
- Add a VERSION file for `treeder/bump`

### Changed

- Change `metadata` file and add `header-includes` for PDF boxes.
- Update LaTeX template [trivadis.tex](templates/trivadis.tex).
- Update [AUTHOR_GUIDE](AUTHOR_GUIDE.md).
- Add example for boxes in
  [1x10-General_Information.md](en/1x10-General_Information.md)

### Fixed

- Fix wrong layout for listings, add `--listings` to pandoc build command

### Removed

## [0.1.0] - 2021-02-25

### Added

- This CHANGELOG file to keep changes documented.
- Add draft version of AUTHOR_GUIDE.
- Add draft version of CODE_OF_CONDUCT.
- Add draft version of CONTRIBUTING.
- Add Trivadis LOGO.
- Add local Template for TeX / LaTeX.
- Add local Template for HTML.
- Add draft version of english docs.
- Add draft version of english docs.

### Changed

- exclude markdownlint MD013 in CODE_OF_CONDUCT.
- update [README](templates/README.md)

## [0.0.1] - 2021-02-25

### Added

- initial release of documents and repository

### Changed

### Fixed

### Removed

[unreleased]: https://github.com/olivierlacan/keep-a-changelog/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/olivierlacan/keep-a-changelog/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/olivierlacan/keep-a-changelog/compare/v0.0.1...v0.1.0
[0.0.1]: https://github.com/olivierlacan/keep-a-changelog/releases/tag/v0.0.1
