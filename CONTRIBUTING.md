# Contributing to Excelsior Family GitHub Guidelines
>We won't ship shit. <3

Thank you for willing to contribute to our [Github Guidelines](https://github.com/ExcelsiorFamily/github-guidelines). The following contributing guidelines intend to ease contribution on this project. These are mostly guidelines, not rules. 

## Table of Contents

* [Asking A Question](#asking-a-question)
* [How To Contribute](#how-to-contribute)
	* [Before Contributing](#before-contributing)
	* [Suggesting An Enhancement](#suggesting-an-enhancement)
* [Styleguides](#styleguides)
	* [Git Commit Messages](#git-commit-messages)
	* [Documentation](#documentation)
* [Issues And Pull Requests Labels](#issues-and-pull-requests-labels)
	* [Type Of Change](#type-of-change)
	* [Severity](#severity)
	* [Type](#type)

## Asking A Question

>**Note:** Please do not file an issue to ask a question. You'll get faster results by following the guidelines below.

We will make some additions to the README file with a FAQ section where you should be able to find answers to most of your questions.

If your question is not in the FAQ list, please feel free to ask you question directly on [slack](excelsior-family.slack.com).

## How To Contribute

### Before Contributing

You are welcome contribute to the GitHub Guidelines whenever you feel it can be improved or you can add to it.

Before you go on with your contribution and create a new issue, make sure to first do these steps :

1. Determine if the enhancement should be suggested in this repository.
2. Perform a search inside the [issues](https://github.com/nshift/github-guidelines/issues) and [pull requests](https://github.com/nshift/github-guidelines/pulls) sections to see if the enhancement has already been suggested or not. If it has and the issue is still open, add a comment to the existing issue instead of opening a new one.

>:warning: If you create a new issue that addresses an enhancement that has already been suggested, your issue will be closed.

### Suggesting An Enhancement

Any enhancement should be tracked as an issue created with the [Enhancement Template](https://github.com/nshift/github-guidelines/blob/master/Templates/ISSUE_TEMPLATE/enhancement.md).

**Preferred:**
```markdown
* [X] I've read, understood, and done my best to follow the [CONTRIBUTING guidelines](/CONTRIBUTING.md).

## Goals
Define the guidelines in terms of label management.
This issue intends to specify what labels to use, why use them and when to use them.

## Attachments
- [Atom Contributing](https://github.com/atom/atom/blob/master/CONTRIBUTING.md).
```

**Not Preferred:**
```markdown
#Labels
Define labels guidelines.
```

Each issue should see itself assigned with the following two types of labels :

- `Severity`
- `Type`

## Styleguides

### Git Commit Messages

Git commit messages should help reviewers to do better reviews.

* Write short messages (we recommend 72 characters or less)
* Use the present tense
* Use the imperative mood
* Reference issues and pull requests liberally after the first line
* Start your commit with :memo: `:memo:` to make it clear Documentation was improved.

### Documentation

A good documentation should be short, clear and explicit so that the reader is able to quickly find the information he is looking for. Each documented guideline should first explain why it exists and then how it should be implemented.

**Preferred:**
```markdown
### Issue Reference

Referencing issue in git commit messages should help anyone to track progress on a specific issue. Git commit messages should always reference issues at the end.

**Preferred:**

- Improve cache management. Related to #42.
- Remove unused ViewController method. Related to #1024.


**Not Preferred:**

- Improve cache management.
- #1024 Remove unused ViewController method.

```

**Not Preferred:**
```markdown
### Issue Reference
Commit messages should always have a reference to their related issue. To do so use # then the number of the issue.

ex: `Improve issue reference description. Related to #123.`
```

## Issues And Pull Requests Labels

Labels help reviewers identify issues and pull requests quickly. Only one type of each category should be assigned at the same time.

### Type Of Change

| Label name | Description |
| --- | --- |
| `Change: Minor` | Less than 64 lines changed, or less than 8 core lines changed |
| `Change: Medium` | Less than 256 lines changed, or less than 64 core lines changed |
| `Change: Master` | More than 256 lines changed, or more than 64 core lines changed |
| `Change: Expert` | Needs specialized, in-depth review |

### Severity

| Label name | Description |
| --- | --- |
| `Severity: Blocker` | The issue is blocking an impending release |
| `Severity: Critical` | The issue causes data loss, crashes or hangs salt processes, makes the system unresponsive, etc. |
| `Severity: High` | The issue reports incorrect functionality, bad functionality, a confusing user experience, etc. |
| `Severity: Strong` | The issue concerns changes to the core areas of the project |
| `Severity: Medium` | The issue reports cosmetic items, formatting, spelling, colors, etc. |
| `Severity: Low` | The issue concerns a new feature or any addition to the project |

### Type

| Label name | Description |
| --- | --- |
| `Type: Feature` | The issue is the development of a new feature of your project |
| `Type: Bug` | The issue is an identified bug that needs to be fixed |
| `Type: Enhancement` | The issue is a suggestion of enhancement to your project |
| `Type: Documentation` | The issue is the creation or refinement of a document |

