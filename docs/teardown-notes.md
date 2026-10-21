# Teardown Notes

Run through these steps after the workshop to remove the sandbox. The demo is entirely disposable — the goal is to leave no trace in your real projects.

1. **Archive the runbook.** Copy the secret gist URL into your notes or the workshop materials while the repo still exists. Once the repo is deleted, links into it stop working, so keep the runbook itself as the durable record of what was demoed.
2. **Merge or close anything still open.** Check the repository's pull request and issue tabs and close whatever remains open. An open PR or issue in a repo you are about to delete has no purpose and only creates confusion if the repo is later restored.
3. **Dismiss and clear notifications.** Open the notifications inbox, filter to the repository, and mark everything read. This prevents setup noise — reviews, comments, and issue activity — from cluttering your inbox after the session.
4. **Delete the sandbox repository.** Go to the repository's Settings page, scroll to the Danger Zone, and delete it. Confirm when prompted. If you would rather keep it as a reference for a future workshop, archive it instead; archiving makes it read-only while preserving everything for a rerun.
5. **Delete the branch objects if you kept the repo.** If you archived instead of deleting, remove the `demo/checklist` branch from the branches page; it was merged, so the content lives on the default branch and the branch itself is redundant.
6. **Verify the gist still makes sense.** Reopen the runbook gist and check that its references — repository name, pull request number, commit SHA, and issue numbers — match what you demoed. If you plan to reuse this sandbox pattern for another session, update the gist rather than starting a fresh one.

**Total teardown time:** roughly 5 minutes if you delete the repo, closer to 10 if you archive and tidy the branches.
