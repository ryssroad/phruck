# Mailroom SOP v0.1

AgentMail is the editorial inbox. It is useful because agents can send each other assignments and state. It is dangerous if it becomes the hidden source of truth.

Current inbox:

```text
harrm@agentmail.to
```

## Rule

```text
Mail is transport. Repo is memory.
```

Every actionable email should become one of:

- a GitHub issue;
- a brief in `briefs/`;
- a dossier/source note in `dossiers/`;
- an active issue-board update in `issues/<number>/`;
- a decision log entry in `logs/`;
- a reply saying it was rejected/held.

## Subject conventions

Use these prefixes when possible:

```text
[signal] raw source or observation
[brief] request for editorial map
[dossier] source packet or research request
[draft] draft text or draft assignment
[review] role review request or result
[gate] road/editor approval needed
[mailroom] administrative coordination
```

## Intake procedure

For each new editorial message:

1. Read the message body, not raw transport headers.
2. Classify it: signal, brief, dossier, draft, review, gate, admin, spam/noise.
3. Check whether a matching GitHub issue already exists.
4. If actionable, create or update the issue/artifact.
5. Reply with:
   - received;
   - where it now lives in repo/GitHub;
   - owner;
   - next action;
   - whether road gate is required.
6. Add mail labels when possible: `phruck`, `triaged`, `processed`, or `blocked`.
7. Do not paste raw headers, unsubscribe URLs, or credential-like links into repo or public summaries.

## Mail triage format

```text
Thread:
Subject:
From:
Received:
Classification:
Actionable summary:
Repo/GitHub target:
Owner:
Risk:
Next action:
Reply needed:
```

## Reply template

```text
Received.

Triage:
- Classification:
- Repo/GitHub target:
- Owner:
- Next action:
- Gate:

No publication will happen from this mail alone; durable state is in the repo.
```

## Current known editorial threads

As of 2026-05-23, the relevant inbox threads are captured in:

```text
logs/mailroom-2026-05-23.md
```

## Failure modes

- Treating email as the archive.
- Letting an unread inbox become the real board.
- Replying with prose but not creating repo state.
- Copying private mail into a public repo without gate.
- Publishing because a mail sounded urgent.
- Losing road decisions in a thread preview.
