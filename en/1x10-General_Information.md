# Introduction
<!-- markdownlint-configure-file { "MD013": { "tables": false } } -->
Add a short introduction to the *Good Practice* guide.

## Scope

Define Scope of this *Good Practice*

## Document Conventions

Define Documentation convetions.

### Severity of the rule

!!! bug "Blocker"
    Will or may result in a bug.

!!! danger "Critical"
    Will have a high/direct impact on the maintenance cost.

!!! warning "Major"
    Will have a medium/potential impact on the maintenance cost.

!!! tip "Minor"
    Will have a low impact on the maintenance cost.

!!! info "Info"
    Very low impact; it is just a remediation cost report.

### Keywords used

| Keyword     | Meaning                                                                         |
|-------------|---------------------------------------------------------------------------------|
| Always      | Emphasizes this rule must be enforced.                                          |
| Never       | Emphasizes this action must not happen.                                         |
| Avoid       | Emphasizes that the action should be prevented, but some exceptions may exist.  |
| Try         | Emphasizes that the rule should be attempted whenever possible and appropriate. |
| Example     | Precedes text used to illustrate a rule or a recommendation.                    |
| Reason      | Explains the thoughts and purpose behind a rule or a recommendation.            |
| Restriction | Describes the circumstances to be fulfilled to make use of a rule.              |

### Validator support

The tool PL/SQL Cop (see the "Tool Support" chapter) cannot support *all* the
guidelines in this document. Those guidelines that are *not* supported by
PL/SQL Cop validators are marked like this:

!!! missing "Unsupported in PL/SQL Cop Validators"
    Reason why the specific guideline is not supported by the validators.

The PL/SQL Cop repository documents the [details of validator limitations](https://github.com/Trivadis/plsql-cop-cli/blob/main/validator-limitations.md#guidelines).

### Why are standards important

For a machine executing a program, code formatting is of no importance. However,
for the human eye, well-formatted code is much easier to read. Modern tools can
help to implement format and coding rules.

Implementing formatting and coding standards has the following advantages for
PL/SQL development:

- Well-formatted code is easier to read, analyze and maintain (not only for the
  author but also for other developers).
- The developers do not have to define their own guidelines - it is already
  defined.
- The code has a structure that makes it easier to avoid making errors.
- The code is more efficient concerning performance and organization of the
  whole application.
- The code is more modular and thus easier to use for other applications.

### We have other standards

This document only defines possible standards. These standards are not written
in stone, but are meant as guidelines. If standards already exist, and they are
different from those in this document, it makes no sense to change them.

### We do not agree with all your standards

There are basically two types of standards.

1. Non-controversial

    These standards make sense. There is no reason not to follow them. An
    example of this category is
    [G-2150](../../4-language-usage/2-variables-and-types/1-general/g-2150):
    Avoid comparisons with NULL value, consider using IS [NOT] NULL.

2. Controversial

    Almost every rule/guideline falls into this category. An example of this
    category is [3 space indention](../../3-coding-style/coding-style/#rules). -
    Why not 2 or 4 or even 8? Why not use tabs? You can argue in favor of all
    these options. In most cases it does not really matter which option you
    choose. Being consistent is more important. In this case it will make the
    code easier to read.

For very controversial rules, we have started to include the reasoning either
as a footnote or directly in the text.

Usually it is not helpful to open an issue on GitHub to request to change a
highly controversial rule such as the one mentioned. For example, use 2 spaces
instead of 3 spaces for an indentation. This leads to a discussion where the
people in favor of 4 spaces start to argument as well. There is no right or
wrong here. You just have to agree on a standard.

More effective is to fork [this repository](https://github.com/Trivadis/plsql-and-sql-coding-guidelines)
and amend the standards to fit your needs/expectations.
