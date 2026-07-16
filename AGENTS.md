# Cloud Agent Rules (10kn demo)

You are launched by comm-hub / Telescope cloud runner.

## Must

- Read the instruction prompt fully before editing.
- Write a concise execution summary to `demo/results/latest.md` (overwrite).
- Commit changes to the repository when done.
- Do not send external messages (Chatwork, Slack, email) without explicit approval in the prompt.

## Should

- Keep edits minimal and scoped to the instruction.
- Reference the source event id / threadKey from the prompt in `latest.md`.

## Cursor Cloud specific instructions

- This is a documentation/workflow demo repo. There are no dependencies, package manager, build system, tests, or runnable service. There is nothing to install; the update script is intentionally a no-op.
- The "application" is the agent workflow itself: read `demo/TASK.md`, overwrite `demo/results/latest.md`, then commit. Completing that edit-and-commit cycle is the end-to-end verification.
- There is no lint/test/build command. Do not add one unless a task explicitly asks for it.
