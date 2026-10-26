# College Application Status Tracker

This repository holds the application status tracker maintained by a Gmail event Trigger. The Trigger checks matching admissions-related email on its supported polling cadence, updates [`applications.md`](applications.md), and returns a concise status and next-actions overview. On its first relevant run, it can seed the file from relevant existing Gmail threads.

## What the tracker records

For each school and program, the tracker may record the entry term, latest confirmed status, update date, next action, who needs to act, any stated deadline and time zone, missing materials explicitly mentioned, and the source email's subject and date. Unclear or unsupported details are marked as needing confirmation rather than guessed.

## Public repository notice

This repository is public at the owner's request. Anyone can read, copy, fork, or preserve its contents and commit history. The tracker is intentionally limited to basic application status and next-action information. Do not add full email messages, attachments, essays, application IDs, birth dates, passwords, financial details, or other unnecessary personal information. Removing information later cannot guarantee that public copies or forks are removed.

## Automation and safety

The automation uses the connected Gmail and GitHub integrations; GitHub Actions, GitHub Pages, and extra repository permissions are not required for the tracker. It does not reply to colleges, submit application forms, access applicant portals, or make payments. It only updates this repository when a relevant email supports a change.

The source of truth for current entries is [`applications.md`](applications.md).