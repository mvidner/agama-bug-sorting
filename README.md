# Agama Bug Sorting (Triage)

Doing bug triage is surprisingly hard to do well.

It is 2026 and we have smart (and dumb) Large Language Models (LLMs), so let's
the machines toil instead of us humans.

In trying to do so, we will describe, to humans or machines alike, how to do the
triage (bug sorting) well.

### Be Kind

Remember there is a human on the other side, with feelings.

Sometimes I get so drawn in by the technical side of the bug that I start
behaving like a machine, being unnnecessarily terse. Or I get annoyed that the
bug is a proof that we did something wrong and now we have to fix it instead of
coding more shiny new features.

I start off my first bug comment by "Thanks for the report :)" to remind me of
the social cooperation that is part of the bug processing.

### Scope: Is It Our Bug

Example: when a user installs openSUSE by writing an OS image and they notice a
problem during their first minutes of booting or using the system, they may file
a bug for the *Installation* component, but in fact our installer was not
involved and the bug should be reassigned.

### Reporter / Commenter

Understanding the affiliation and team of the people reporting or commenting the
bug will help you providing context for their report, and selecting an
appropriate detail level for your response. The time zone they work in is also
relevant for dialog round trips.

You can look up the team of SUSE coworkers using Workday or Slack.

### Asking for help

If you ask a colleague for help, they may be more inclined to do it if you tell
them upfront that you only expect them to spend 1 minute on it.

### Making a Kanban/PBI/Trello Card

- Reassign to yast-internal@suse.de
- Put the card URL to the URL field (or to a comment, if the URL field is
  already taken by openQA)
- Add this comment so that people do not reply with "But I cannot access that URL!!!"

```txt
Adding this to the team Kanban board for work planning.

(You probably do not have access to that board if you are not in the installer team
but that's OK, we will continue to update this Bugzilla ticket.)
```

### Specific technologies

Browser: sometimes bugs are caused by user installed browser extensions. Retry
in Anonymous (Incognito) mode.
