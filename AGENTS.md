# Agents

## Merge guardrail

Do not merge, and do not land commits on a default or protected branch, unless the user has sent an explicit GO for that merge in this conversation.

Explicit GO is the user's message `GO`, or a message that uses `GO` as the approval for that specific repository, branch, and pull request. Example: `GO merge this pull request`.

These messages do not authorize a merge: deploy, ship, merge when ready, looks good, approved, LGTM, yes, do it, go ahead, or a request to open a pull request.

Without GO, you may commit on a feature branch when asked, push that branch, and open a pull request.

Without GO, you may not run `gh pr merge`, merge through the GitHub UI or API, `git merge` into the default branch, or `git push` to `main`, `master`, or another default or protected branch. Squash and rebase merges that land on the default branch are included.

When the change is ready, stop. Name the repository, branch, and pull request, and ask for GO.
