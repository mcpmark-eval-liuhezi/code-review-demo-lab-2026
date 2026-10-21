# Demo Script: 20-Minute Code-Review Workshop

Total time: 20 minutes. Everything below runs against the disposable sandbox repository, so nothing here can affect a real project. Times are cumulative from the start of the session.

| Time | Duration | What happens |
|------|----------|---------------|
| 0:00 | 2 min | **Welcome and framing.** Why we review code at all: catching defects early, spreading knowledge, and shared ownership. Point at the sandbox repo on screen and state the ground rule for the session — every action today happens in the demo repo and nowhere else. |
| 0:02 | 3 min | **Open the pull request.** Show the PR view: title, description, and the list of changed files. Read the description out loud, then open `docs/reviewer-checklist.md` from the branch so the group can follow along with the checklist we will apply. |
| 0:05 | 4 min | **Walk the diff.** Go file by file in the order they appear in the PR. For each file, say which checklist items apply and demonstrate one inline comment on a specific line. Emphasize that comments should name the problem and suggest a fix, not just express a preference. |
| 0:09 | 3 min | **Issues and sub-issues.** Open the umbrella issue and expand its two sub-issues. Explain when to use an umbrella with sub-issues versus a single issue: break work apart when different people will pick up different parts. |
| 0:12 | 5 min | **Live review exercise.** Each participant picks one checklist item and leaves one comment on the PR using it. Walk the room and help people frame their comment. Reserve the last minute for the author persona to reply to one comment so the group sees a review conversation. |
| 0:17 | 2 min | **Approve and merge.** Submit the review with an approval summary, then merge the PR and show that the branch disappears from the branch list. Note that merging is the point where a review becomes binding. |
| 0:19 | 1 min | **Teardown and Q&A.** Open `docs/teardown-notes.md`, confirm everyone knows the sandbox will be deleted after the session, and take questions. |

**Presenter notes:** If the live PR view is slow, the same content is in the repo's `docs/` folder on the `demo/checklist` branch. Keep an eye on the clock at 0:12 — the exercise is the part that always runs long. If you lose the room, jump straight to the merge at 0:17 and finish with teardown.
