# Introduction

First off, thank you for considering contributing to Ascentrade.
It's still under active development, so we are grateful for interested and likeminded people to bring this project forward.

Following these guidelines helps to communicate that you respect the time of the developers managing and developing this open source project.
In return, they should reciprocate that respect in addressing your issue, assessing changes, and helping you finalize your pull requests.

Ascentrade is a free and open source project, and we love to receive contributions from our community — you!
You can contribute in many ways, from writing tutorials or blog posts, improving the documentation, submitting bug reports and feature requests or writing code which can be incorporated into Ascentrade itself.

# Getting started

If you [report a bug](#how-to-report-a-bug) or [suggest a new feature](#how-to-suggest-a-feature-or-enhancement), please check existing issues first.
Maybe someone already reported your issue and you can join the discussion or help reproducing the problem.

## Legal safeguards
Ascentrade doesn't require a CLA (Contributor License Agreement). The copyright belongs to all the individual contributors. Therefore, we recommend that every contributor adds the following line to the header of a file if they changed it substantially:

```
Copyright (c) <year>, <your name> (<your email address>)
```

We use the Developer Certificate of Origin (DCO) as an additional safeguard for the Ascentrade project.
This well established and widely used mechanism assures contributors have confirmed their right to license their contribution under the project's license.
Please read [Developer Certificate of Origin](./DCO).
If you can certify it, then just add a line to every git commit message:

````
  Signed-off-by: <your name> <your email address>
````

We will not merge pseudonymous or anonymous contributions, so we ask you to provide your real name.
If you set your `user.name` and `user.email` git configs, you can sign your commit automatically with `git commit -s`.
You can also use git [aliases](https://git-scm.com/book/tr/v2/Git-Basics-Git-Aliases) like `git config --global alias.ci 'commit -s'`. Now you can commit with `git ci` and the commit will be signed.

## How to report a bug
### Security vulnerability
> If you find a security vulnerability, do **NOT** open an issue.
> Please submit security issues directly to security@ascentrade.app.
> In order to determine whether you found a security issue, ask yourself these two questions:
> * Can I access something that's not mine, or something I shouldn't have access to?
> * Can I disable something for other people?

> If the answer to either of those two questions is "yes", then you probably found a security issue.
> Note that even if you answer "no" to both questions, you may still have found a security issue, so if you're unsure, just email us at security@ascentrade.app.

### Regular bugs
This section guides you through submitting a bug report for Ascentrade. Following these steps helps us understand your report, reproduce the behavior and find related reports.

When filing an issue, make sure to answer these three questions:

1. What did you do?
2. What did you expect?
3. What happened instead?

Please also provide relevant console output, logs and/or screenshots and make sure the title is **clear** and **descriptive**.

## How to suggest a feature or enhancement
This section guides you through submitting a feature request for Ascentrade. Following these steps helps us understand your suggestion and find related suggestions.

When submitting a feature request, make sure to answer these three questions:

1. What do you miss?
2. How would you describe the specific result of implementing the feature?
3. Why is this feature useful for others?

Please also provide relevant console output, logs and/or screenshots and make sure the title is **clear** and **descriptive**.

## Commit guidelines
### Prefer atomic commits
In general, the smaller the commit, the better. We prefer atomic coherent commits, which apply a distinct and related set of changes in a single action:

#### 1. All changes in a commit should be related.
Don't combine changes that address different problems into a single commit.

#### 2. All changes in a commit should address a single aspect of a problem or change.
Don't be afraid to break up a new feature, bug fix, or refactoring effort into multiple distinct changes.
This will help you keep track of what works and what doesn't: if there's a problem, you can always revert to the last known good state. If you wait too long between commits, you may lose a lot of work or spend too long finding the source of the problem.

#### 3. Prefer _small_ commits to _large_ commits.
This helps reviewers by allowing them to focus on a small set of related changes and helps future debugging efforts by increasing the probability that a [`git bisect`](https://git-scm.com/docs/git-bisect) operation will quickly identify the source of the problem.

#### 4. Keep whitespace and formatting cleanup distinct.
Don't mix code changes with whitespace or formatting changes! If you fix code formatting, include those changes separately from your code changes. 

### Commit message conventions
The example below represents a full commit message which will be explained in detail afterwards.

```
50-char-ish"subject" which summarizes the change

After the first line, include additional explanatory text. Include
one blank line in between the summary and the body. Various tools
like git log, git shortlog, and git rebase get confused if the two
sections run together.

You can also include bullet points:
* A
* B
* C

Fixes #102
Relates to #100, #8
```

#### The subject
Keep the first line of a commit message (subject) shorter than 50 characters.
Formulate the subject in **imperative mood** (`Add...`, `Remove...`, `Fix...`) instead of using past tense (`Added...`, `Removed...`, `Fixed...`).

General commit message subjects include:
* `Refactor component X`
* `Implement feature Y`
* `Remove deprecated methods`
* `Update to version 1.2.3`

Try to complete the following sentence with your subject line:
> If applied, this commit will [subject line here].

#### The body (optional)
In cases where the subject needs further explanation you can add details in the body.
The body defines the section after the subject **separated by a blank line**.
It can include bulleted lists but must not exceed 72 characters per line.

#### The footer (optional)
The footer includes optional metadata, such as fixed or related issues.
It is **separated by a blank line**.

# Acknowledgement
We want to expressively thank all those involved in the following open source projects, as they helped us form the foundation of this contributing guide:

* [**Elasticsearch**](https://github.com/elastic/elasticsearch/blob/master/CONTRIBUTING.md) and [**Hoodie**](https://github.com/hoodiehq/hoodie/blob/master/CONTRIBUTING.md) for the introduction
* **Embedded Artistry** for the [commit guidelines](https://embeddedartistry.com/fieldatlas/source-control-commit-guidelines/)
* **Atom** for the [bug report guidelines](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#reporting-bugs)
* **Travis CI** for the [vulnerability disclosure guidelines](https://github.com/travis-ci/travis-ci/blob/master/CONTRIBUTING.md#security-issues)
* **Nextcloud** for the [DCO](https://github.com/nextcloud/server/blob/master/.github/CONTRIBUTING.md#sign-your-work) and general [contributing guidelines](https://github.com/nextcloud/server#contribution-guidelines-)