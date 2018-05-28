# Github Guidelines

> We will do all that we can to keep the productivity of ourselves, and others, as high as possible -- Uncle Bob

These guidelines are based on [Building a strong community Github documentation](https://help.github.com/categories/building-a-strong-community/) and intend to promote a better collaboration.

## Table of Contents

* [Issue & Pull Request Template](#issue--pull-request-template)
	* [Multiple Issue Templates Over Single Issue Template](#multiple-issue-template-over-single-issue-template)
	* [Issue & Pull Request Expectation](#issue--pull-request-expectation)
	* [Promoting A High Contribution Quality](#promoting-a-high-contribution-quality)
	* [Git Commit Messages](#git-commit-messages)
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

### Git Commit Messages

#### Content

Git Commit messages should always be clear about what has been done. It should be written at the present tense and imperative Mood.

**Preferred:**
```markdown
- Add get user feature.
- Update navigation storyboard.
```

**Not Preferred:**
```markdown
- Added get user feature.
- Updates navigation storyboard.
```

#### Reference

Git Commit messages should reference issues at the end.

**Preferred:**
```markdown
- Improve cache management. Related to #42.
- Remove unused ViewController method. Related to #1024.
```

**Not Preferred:**
```markdown
- Improve cache management.
- #1024 Remove unused ViewController method.
```

#### Emojis

For clear visual identification start the commit message with an applicable emoji:

   - :art: `:art:` when improving the format/structure of the code
   - :racehorse: `:racehorse:` when improving performance
   - :non-potable_water: `:non-potable_water:` when plugging memory leaks
   - :memo: `:memo:` when writing docs
   - :bug: `:bug:` when fixing a bug
   - :fire: `:fire:` when removing code or files
   - :green_heart: `:green_heart:` when fixing the CI build
   - :white_check_mark: `:white_check_mark:` when adding tests
   - :lock: `:lock:` when dealing with security
   - :arrow_up: `:arrow_up:` when upgrading dependencies
   - :arrow_down: `:arrow_down:` when downgrading dependencies
   - :shirt: `:shirt:` when removing linter warnings


## Milestone

## Label

## CHANGELOG

## CONTRIBUTING.md

## Resources
