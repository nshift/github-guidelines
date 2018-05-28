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

## Labels

### Immutablity

GitHub labels should define immutable informations about issues, in order to avoid non-updating scenarios. States should be defined in project section.

**Preferred:**
```markdown
- type
- severity
```

**Not Preferred:**
```markdown
- priority
- status
```

### Colors

Colors should be variants of Red-Orange-Green to provide a sense of state. It is better to use similar color styling accross categories for a stronger visual identification. Red being the ones that require the most attention. Green being the ones that require little attention.

**Preferred:**
```markdown
- `Severity: Low`: green
- `Severity: Medium`: orange
- `Severity: Critical`: red
- `Change: Minor`: green
- `Change: Medium`: orange
- `Change: Master`: red
```

**Not Preferred:**
```markdown
- `Severity: Low`: blue
- `Severity: Medium`: blue
- `Severity: Critical`: blue
- `Change: Minor`: green
- `Change: Medium`: green
- `Change: Master`: green
```

### Categories

Labels should help reviewers to quickly get information about the reviewing effort. Labels should be categorized to provide the same amount of information for each issue. Issues cannot have more than one label from the same category.

**Preferred:**
```markdown
- `Severity: Low`
- `Severity: Medium`
- `Severity: Critical`
- `Change: Minor`
- `Change: Medium`
- `Change: Master`
```

**Not Preferred:**
```markdown
- `Low`
- `Medium`
- `Critical`
- `Blocked`
- `Feature`
- `WorkInProgress`
```

*Pro tip:* GitHub orders labels aphabetically, so following this format allows to keep categories dislayed in the same order accross every issues.

#### Type

Type labels should be used to define the type of task done inside the issue.

- `Type: Feature` **#00cc41**
The issue is the development of a new feature of your project.

- `Type: Bug` **#ff0000**
The issue is an identified bug that needs to be fixed.

- `Type: Enhancement` **#ffe700**
The issue is a suggestion of enhancement to your project.

- `Type: Documentation` **#c3b2ef**
The issue is the creation or refinement of a document.

#### Severity

Severity labels are mostly used for bug-related issues. It allows to identify the critical aspects of the work implied inside the issue.

- `Severity: Blocker`**#ff0000**
The issue is blocking an impending release.

- `Severity: Critical` **#ff4000**
The issue causes data loss, crashes or hangs salt processes, makes the system unresponsive, etc.

- `Severity: High` **#ff8100**
The issue reports incorrect functionality, bad functionality, a confusing user experience, etc.

- `Severity: Strong` **#ffe700**
The issue concerns changes to the core areas of the project.

- `Severity: Medium` **#00cc41**
The issue reports cosmetic items, formatting, spelling, colors, etc.

- `Severity: Low` **#c3b2ef**
The issue concerns a new feature or any addition to the project.

#### Type of change

Type of change labels are only used for pull requests. They give information about the effort needed to review a pull request. We strongly recommend to define core areas to help define the estimated effort.

- `Change: Minor` **#c3b2ef**
Less than 64 lines changed, or less than 8 core lines changed.

- `Change: Medium` **#00cc41**
Less than 256 lines changed, or less than 64 core lines changed.

- `Change: Master` **#ffe700**
More than 256 lines changed, or more than 64 core lines changed.

- `Change: Expert`**#ff0000**
Needs specialized, in-depth review.

## CHANGELOG

## CONTRIBUTING.md

## Resources
