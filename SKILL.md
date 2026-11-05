---
name: implement
description: Implement a piece of work based on a spec or set of tickets.
disable-model-invocation: true
license: MIT
metadata:
  author: Matt Pocock
  adapted_by: Igor Guariroba
  version: 1.0.0
---


Implement the work described by the user in the spec or tickets. Before editing, record the starting HEAD and existing staged/unstaged/untracked changes. Preserve the user's work and use that starting SHA as the review base.

Read `../tdd/SKILL.md` and apply it where possible, at pre-agreed seams. Resolve skill references relative to this skill directory; Pi loads their instructions through file reads, not a Skill tool.

Work in the current Pi session by default. When independent work benefits from delegation, read `references/pi-workers.md` and use fresh Pi processes; each concurrent writer needs its own worktree. Herdr is optional under that guide's conditions.

Run typechecking regularly, single test files regularly, and the full test suite once at the end.

Once implemented and validated, read `../code-review/SKILL.md` to review both your commits and your uncommitted changes against that SHA. Fix actionable findings and rerun the affected checks before concluding.

Commit only your work to the current branch. Report the commit, acceptance criteria covered, checks run and any remaining blockers; completion requires every requested criterion to be accounted for.
