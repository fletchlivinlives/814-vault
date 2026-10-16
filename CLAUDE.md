# How to work in this vault

This vault is the memory for Fletch's businesses. Every session starts from it and writes back to it. It is an Obsidian vault in git: Fletch reads it in Obsidian, Claude reads and edits the files.

## Start of every session

1. `git pull` so you have what other sessions wrote.
2. Read [[Home]], then the index note of the business the task is about (for example `01 814 Epoxy/814 Epoxy.md`) and every note it links to.
3. If the task matches a job in `Jobs/`, read that job's index note and every note it links to, then follow its steps in order.
4. Skim the index block at the top of the last few notes in `Daily/` for recent work.

## Memory lives here

- Do not use Claude's default memory directory. Anything worth remembering goes in this vault.
- **Append before you create.** Add to an existing note whenever one fits. Make a new note only when nothing fits, and link it from the right index note in the same edit. A note no index links to doesn't exist for the next session.
- Keep notes short and factual. Replace stale facts instead of adding a second version. If two notes cover the same thing, merge them.
- Every folder has one index note named after the folder. It says what the folder is for and links every note in it.
- A new business gets a numbered folder (`02 Name/`) only once something is actually happening. Ideas go in [[Ideas]] until then.
- Use the files in `Templates/` for new businesses, jobs and daily notes.

## Daily notes

- One note per day: `Daily/YYYY-MM-DD.md`, from `Templates/Daily.md`.
- Write to it at the end of a session, and mid-session after anything big. Several sessions may write the same day: pull first, then add your section; never rewrite another session's section.
- Keep the **Index** block at the top current: one line per item, so a later search can find the day without reading the whole note.
- Log decisions and the reason for them, not just what was done.

## Safety

- **Draft, then wait for Fletch's OK** before anything goes to a customer or moves money: sending email or texts, creating, sending or changing invoices, estimates or payment links, posting publicly. A job note may lift this for a specific step only if it says so explicitly.
- Never write to QuickBooks unless the current job says to and Fletch has approved it in this session.
- No passwords, API keys, tokens or full bank or card numbers in the vault. Say where a secret lives (for example "Script Properties of the QB sync project"), never its value.

## Git

- Work on `main`; the vault has one branch so every session and Obsidian see the same notes.
- Commit and push after each meaningful change, with a message that says what changed.
- If a push is rejected, pull (merge, not rebase), resolve, and push again. Never force-push.
