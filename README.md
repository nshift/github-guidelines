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

Milestones should be based on iterative development and produce incremental builds. It enforces Agile methodology and promote continuous integration and deployment. It allows you to follow overall progress and create [changelogs](#changelog) based on opened/closed issues.

### Incremental Title

Milestones should be described as increment based on software version.

**Preferred:**
```markdown
Milestones:

- 1.1.0
- 1.2.0
- 1.3.0
- 1.4.0
```

**Not Preferred:**
```markdown
Milestones:

- Backlog
- Ice Box
- Release 1.0
- Release 2.0
```

*Pro tip*: when closing a milestone, a git tag using software version should be created.

### Short Iterative Due Date

**Milestones must have short due dates to define small increment** and should only be closed when progress is at 100%, meaning that all issues and pull requests related to it are closed. If you do not consider an issue to be necessarily closed to finish your current milestone then it should be moved to another one.

**Preferred:**
```markdown
Milestones:

- 1.1.0 - Closed 4 weeks ago
- 1.2.0 - Closed 2 weeks ago
- 1.3.0 - Closed 1 day ago
- 1.4.0 - Due by June 8, 2018
```

**Not Preferred:**
```markdown
Milestones:

- Backlog - No due date
- Ice Box - No due date
- Version 1.0 - Due by September 1, 2019
- Version 2.0 - Due by September 1, 2022
```

*Pro tip*: when closing a milestone, webhooks can be used to automatically create a release flow.

### Github Issue And Pull Request Priority

Milestones should drive development for contributors and help them to focus on most priority issues and pull requests. Priorization should be based on comparaison and it's up to maintainers.

*Pro tip*: [labels](#label) should help maintainers to compare issues and pull requests easily.

## Label

## CHANGELOG

## CONTRIBUTING.md

## Resources
