# Github Guidelines

> We will do all that we can to keep the productivity of ourselves, and others, as high as possible -- Uncle Bob

These guidelines are based on [Building a strong community Github documentation](https://help.github.com/categories/building-a-strong-community/) and intend to promote a better collaboration.

## Table of Contents

* [Issue & Pull Request Template](#issue--pull-request-template)
	* [Multiple Issue Templates Over Single Issue Template](#multiple-issue-template-over-single-issue-template)
	* [Issue & Pull Request Expectation](#issue--pull-request-expectation)
	* [Promoting A High Contribution Quality](#promoting-a-high-contribution-quality)
* [Milestone](#milestone)
* [Label](#label)
* [CHANGELOG](#changelog)
* [CONTRIBUTING.md](#contributingmd)
* [Resources](#resources)

## Issue & Pull Request Template

Issue and pull request templates should drive reporters to give all the necessary information to help reviewers.

Import the [pull request template](/Templates/pull_request_template.md) and [issue template](/Templates/issue_template.md) into `.github` folder in your repository root directory.

### Multiple Issue Templates Over Single Issue Template

[Multiple issue templates](https://help.github.com/articles/about-issue-and-pull-request-templates/) are prefered over [single issue templates](https://help.github.com/articles/manually-creating-a-single-issue-template-for-your-repository/) in order to specify required information for each type of issue.

Import the following issue templates into `.github/ISSUE_TEMPLATE/` folder in your repository root directory:

- [Feature request](/Templates/ISSUE_TEMPLATE/feature-request.md)
- [Bug report](/Templates/ISSUE_TEMPLATE/bug-report.md)

### Issue & Pull Request Expectation

Issue and pull request templates should contains title (h2) and description using html comment.

**Preferred:**
```markdown
## Description
<!-- A clear and concise description of what the bug is. -->

## How to reproduce it
<!-- Steps to reproduce the behavior. -->

...
```

**Not Preferred:**
```markdown
**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

...
```

### Promoting A High Contribution Quality

Templates should promote a high contribution quality by referring [contributing guidelines](#contibutingmd).

**Preferred:**
```markdown
> Please fill out this template when filing an issue. It is based on [Excelsior Family Github guidelines](https://github.com/ExcelsiorFamily/github-guidelines).
>
> This template intends to describe a bug report. If you are describing a non existing feature, please use the [feature request template](https://github.com/ExcelsiorFamily/github-guidelines/issues/new?template=feature-request.md).

* [ ] I've read, understood, and done my best to follow the [CONTRIBUTING guidelines](/CONTRIBUTING.md).

## Description
<!-- A clear and concise description of what the bug is. -->

## How to reproduce it
<!-- Steps to reproduce the behavior. -->

...
```

**Not Preferred:**
```markdown
## Description
<!-- A clear and concise description of what the bug is. -->

## How to reproduce it
<!-- Steps to reproduce the behavior. -->

...
```

## Milestone

## Label

### Immutablity

GitHub labels should define immutable informations about issues, in order to avoid non-updated scenarios. States should be defined in project section.

**Preferred:**
```markdown
- Type: Feature
- Severity: Low
```

**Not Preferred:**
```markdown
- WorkInProgress
- Critical
```

### Colors

It is better to use similar color styling accross categories for a consistent and stronger visual identification. Colors should be variants of Red-Orange-Green to provide a sense of state. Red being the ones that require the most attention. Green being the ones that require little attention.

**Preferred:**

- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) `Severity: Low`
- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) `Severity: Medium`
- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) `Change: Minor`
- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) `Change: Medium`

**Not Preferred:**

- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) `Severity: Low`
- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) `Severity: Medium`
- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) `Change: Minor`
- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) `Change: Medium`

### Categories

Labels should help reviewers to quickly get information about the reviewing effort. Labels should be regrouped into categories to provide consistent information about every issue. Issues cannot have more than one label from the same category.

**Preferred:**
```markdown
- Type: Documentation
- Severity: Medium
- Change: Minor
```

**Not Preferred:**
```markdown
- Question
- Feature
- Documentation
```

*Pro tip:* GitHub orders labels aphabetically, so following this format allows to keep categories dislayed in the same order accross every issues.

#### Type

Type labels should be used to define the type of task done inside the issue.

- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) (**#00cc41**) `Type: Feature`: The issue is the development of a new feature of your project.
- ![#ff0000](https://placehold.it/15/ff0000/000000?text=+) (**#ff0000**) `Type: Bug`: The issue is an identified bug that needs to be fixed.
- ![#ffe700](https://placehold.it/15/ffe700/000000?text=+) (**#ffe700**) `Type: Enhancement`: The issue is a suggestion of enhancement to your project.
- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) (**#c3b2ef**) `Type: Documentation`: The issue is the creation or refinement of a document.

#### Severity

Severity labels are mostly used for bug-related issues. It allows to identify the critical aspects of the work implied inside the issue.

- ![#000000](https://placehold.it/15/000000/000000?text=+) (**#000000**) `Severity: Blocker`: The issue is blocking an impending release.
- ![#ff4000](https://placehold.it/15/ff4000/000000?text=+) (**#ff4000**) `Severity: Critical`: The issue causes data loss, crashes or hangs salt processes, makes the system unresponsive, etc.
- ![#ff8100](https://placehold.it/15/ff8100/000000?text=+) (**#ff8100**) `Severity: High`: The issue reports incorrect functionality, bad functionality, a confusing user experience, etc.
- ![#ffe700](https://placehold.it/15/ffe700/000000?text=+) (**#ffe700**) `Severity: Strong`: The issue concerns changes to the core areas of the project.
- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) (**#00cc41**) `Severity: Medium`: The issue reports cosmetic items, formatting, spelling, colors, etc.
- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) (**#c3b2ef**) `Severity: Low`: The issue concerns a new feature or any addition to the project.

#### Type of change

Type of change labels are only used for pull requests. They give information about the effort needed to review a pull request. We strongly recommend to define core areas to help define the estimated effort.

- ![#c3b2ef](https://placehold.it/15/c3b2ef/000000?text=+) (**#c3b2ef**) `Change: Minor`: Less than 64 lines changed, or less than 8 core lines changed.
- ![#00cc41](https://placehold.it/15/00cc41/000000?text=+) (**#00cc41**) `Change: Medium`: Less than 256 lines changed, or less than 64 core lines changed.
- ![#ffe700](https://placehold.it/15/ffe700/000000?text=+) (**#ffe700**) `Change: Master`: More than 256 lines changed, or more than 64 core lines changed.
- ![#ff0000](https://placehold.it/15/ff0000/000000?text=+) (**#ff0000**) `Change: Expert`: Needs specialized, in-depth review.

## CHANGELOG

## CONTRIBUTING.md

## Resources
