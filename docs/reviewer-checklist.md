# Reviewer Checklist

Use this checklist on every pull request before approving it. Work top to bottom and do not skip steps, even on small PRs — most escapes happen in the steps people rush.

1. **Understand the intent.** Read the pull request description and any linked issue first. State in one sentence what the PR is trying to accomplish; if you cannot, stop and ask the author instead of guessing.
2. **Run the code locally before you read it.** Pull the branch, install dependencies, and reproduce the behavior the PR claims to change. A change that cannot be run cannot be meaningfully reviewed.
3. **Check the tests.** Confirm there is at least one test that fails before the change and passes after it. Verify the tests cover the boundary conditions, not only the happy path — empty inputs, large inputs, concurrency, and error cases.
4. **Read the diff line by line, not just the files changed.** Look for dead code, commented-out blocks, leftover debugging statements, and changes that look unrelated to the stated intent. Unexplained changes are the most common place for bugs to hide.
5. **Check for security and data handling problems.** Look for hardcoded credentials, unsanitized user input reaching a query or shell, overly broad permissions, and personal or sensitive data being written to logs.
6. **Verify naming, structure, and consistency.** New names should match the conventions of the surrounding code. Flag duplication that a small refactor would remove, and private functions that have grown large enough to deserve tests of their own.
7. **Confirm the public contract is intentional.** Anything that changes an API, a config file, a migration, or a shared schema needs an explicit callout in the review. Ask what happens to existing consumers.
8. **Leave actionable feedback.** Every comment should state the problem, why it matters, and a suggested fix or a question. Separate blocking comments from optional suggestions so the author knows what actually must change.

Before you approve: you can explain the change to a third party without help, the tests are green in CI, and you would be comfortable being paged at 3 AM because of this code.
