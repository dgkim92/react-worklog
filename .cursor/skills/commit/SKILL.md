---
name: commit
description: Writes an English commit message from the current changes. Optional commit notes included with the request take priority over the diff. Asks the user when more detail is needed. Use when the user invokes /commit or asks to write a commit message for the current changes.
disable-model-invocation: true
---

# Commit

Write an English commit message from the current changes. Commit notes included with the request are optional. When they are present, they are the primary source for the message.

## Instructions

1. Read the current changes, including staged and unstaged diffs, and recent commit messages so the new message matches the repository's style.
2. If the user included commit notes, treat that wording and intent as the highest priority. Use the diff to confirm the notes and to fill in only what the notes leave out. If there are no notes, base the message on the diff.
3. Ask the user before writing the message when the notes and the diff conflict, or when there are no notes and the diff does not make clear why the change was made.
4. Write the commit message in English. Focus on why the change was made, in one or two sentences. When notes were provided, lead with them.
