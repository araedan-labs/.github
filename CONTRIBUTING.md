# Contributing to Araedan-Labs projects

## Getting started, building, and testing

If you haven't already, take a look at the project's `DEVELOPMENT.md` and its
documentation.

## Discussion

If you've run into behaviour in a project you don't understand, or you're having
trouble working out a good way to apply it to your code, or you've found a bug
or would like a feature it doesn't have, we want to hear from you!

Our main forum for discussion is the project's GitHub issue tracker.  This is
the right place to start a discussion of any of the above or most any other
topic concerning the project.

## Style guide

For Python code, the [Google Style
Guide](https://google.github.io/styleguide/pyguide.html) must be followed.

For documentation, the [Google Style Python
Docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
must be followed.

## First Time Contributors

We appreciate your contribution! If you are interested in helping improve any
project, there are several ways to get started:

* Work on documentation. Play around with the code and add tests to find bugs.

## Submitting Changes

Even more excellent than a good bug report is a fix for a bug, or the
implementation of a much-needed new feature. (*)  We'd love to have your
contributions.

(*) If your new feature will be a lot of work, we recommend talking to us early
-- see below.

We use the usual GitHub pull-request flow, which may be familiar to you if
you've contributed to other projects on GitHub.  For the mechanics, see
[GitHub's own
documentation](https://help.github.com/articles/using-pull-requests/).

Anyone interested in our projects may review your code.  One of the core
developers will merge your pull request when they think it's ready. For every
pull request, we aim to promptly either merge it or say why it's not yet ready;
if you go a few days without a reply, please feel free to ping the thread by
adding a new comment.

## Preparing Changes

Before you begin: if your change will be a significant amount of work to write,
we highly recommend starting by opening an issue laying out what you want to do.
That lets a conversation happen early in case other contributors disagree with
what you'd like to do or have ideas that will help you do it.

The best pull requests are focused, clearly describe what they're for and why
they're correct, and contain tests for whatever changes they make to the code's
behaviour.  As a bonus these are easiest for someone to review, which helps your
pull request get merged quickly! Standard advice about good pull requests for
open-source projects applies.

Also, do not squash your commits after you have submitted a pull request, as
this erases context during review. We will squash commits when the pull request
is merged.

## Core developer guidelines

Core developers should follow these rules when processing pull requests:

* Always wait for tests to pass before merging PRs.
* Use "[Squash and merge](https://github.com/blog/2141-squash-your-commits)"
  to merge PRs.
* Delete branches for merged PRs (by core devs pushing to the main repo).
* Edit the final commit message before merging to conform to the following
  style (we wish to have a clean `git log` output):
  * When merging a multi-commit PR make sure that the commit message doesn't
    contain the local history from the committer and the review history from
    the PR. Edit the message to only describe the end state of the PR.
  * Make sure there is a *single* newline at the end of the commit message.
    This way there is a single empty line between commits in `git log`
    output.
  * Split lines as needed so that the maximum line length of the commit
    message is under 80 characters, including the subject line.
  * Capitalize the subject and each paragraph.
  * Make sure that the subject of the commit message has no trailing dot.
  * Use the imperative mood in the subject line (e.g. "Fix typo in README").
  * If the PR fixes an issue, make sure something like "Fixes #xxx." occurs
    in the body of the message (not in the subject).
  * Use Markdown for formatting.

## Issue-tracker conventions

We aim to reply to all new issues promptly.  We'll assign a milestone to help us
track which issues we intend to get to when, and may apply labels to carry some
other information.  Here's what our milestones and labels mean.

### Task priority and sizing

We use GitHub "labels" to roughly order what we want to do soon and less soon.
There's two dimensions taken into account: **priority** (does it matter to our
users) and **size** (how long will it take to complete).

Bugs that aren't a huge deal but do matter to users and don't seem like a lot of
work to fix generally will be dealt with sooner; things that will take longer
may go further out.

We are trying to keep the backlog at a manageable size, an issue that is
unlikely to be acted upon in foreseeable future is going to be respectfully
closed.  This doesn't mean the issue is not important, but rather reflects the
limits of the team.

The **question** label is for issue threads where a user is asking a question
but it isn't yet clear that it represents something to actually change.  We use
the issue tracker as the preferred venue for such questions, even when they
aren't literally issues, to keep down the number of distinct discussion venues
anyone needs to track.  These might evolve into a bug or feature request.

Issues **without a priority or size** haven't been triaged.  We aim to triage
all new issues promptly, but there are some issues from previous years that we
haven't yet re-reviewed since adopting these conventions.
