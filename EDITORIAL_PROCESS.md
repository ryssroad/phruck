# Editorial Process v0.1

phruck now treats email, GitHub issues, branches, pull requests, and the repo archive as one editorial operating system.

Core rule:

```text
AgentMail is transport. GitHub Issues are the board. Pull requests are the workbench. The repo is memory. road is root of trust.
```

The goal is not bureaucracy. The goal is that any agent can arrive, read the repo, and know what is active, who owns it, what is blocked, and what must not be published yet.

## 1. Control plane

### Source of truth

The repo is canonical for durable state:

- editorial rules;
- issue state;
- briefs and dossiers;
- drafts and review notes;
- publish queue;
- decision logs;
- links to actionable email threads.

No important decision should live only in Telegram, AgentMail, or a model context window.

### Transport

AgentMail is the editorial inbox and cross-agent coordination channel.

Current inbox:

```text
harrm@agentmail.to
```

Mail may carry assignments, signals, source packets, review notes, or editorial disputes. Mail is not canonical until it is triaged into a repo artifact or GitHub issue.

### Board

GitHub Issues are the visible task board.

Every active item should be one of:

- `type:signal` — raw input that may become a brief;
- `type:brief` — compact editorial map needed or in progress;
- `type:dossier` — source packet / evidence gathering;
- `type:draft` — prose artifact being written;
- `type:review` — structure, style, risk, or red-team pass;
- `type:gate` — road/editor approval needed;
- `type:mail` — mailroom/admin processing.

### Workbench

Pull requests are where repo changes happen.

Default rule:

```text
No silent main pushes unless road explicitly asks for direct commit.
```

Use branches named by lane:

```text
ops/<process-change>
docs/<doc-or-brief>
brief/<topic>
dossier/<topic>
draft/<piece>
review/<piece>
issue/<number>-assembly
```

## 2. Daily/online heartbeat

When an agent comes online for phruck work:

1. Pull latest `main`.
2. Read `README.md`, `CONSTITUTION.md`, `ISSUE_PROTOCOL.md`, `STYLEBOOK.md`, `EDITORIAL_PROCESS.md`, and the active issue board.
3. Check AgentMail for unread or recent editorial threads.
4. Convert actionable mail into GitHub issues or repo notes.
5. Check open GitHub issues and PRs.
6. Pick the smallest safe next editorial move.
7. Make it in a branch/PR.
8. Update `logs/YYYY-MM-DD.md` or the relevant issue board.
9. If a road gate is required, stop at `ready-for-road`; do not publish.

If there is no real signal, do not invent content to look active.

## 3. Editorial state machine

```text
signal
  -> intake
  -> brief
  -> dossier/source packet
  -> editorial map
  -> assigned draft
  -> structure pass
  -> draft
  -> role review
  -> red-team/risk pass
  -> issue assembly
  -> road/constitution gate
  -> publish queue
  -> archive
```

Allowed autonomous moves at Level 0/1:

- triage mail;
- create GitHub issues;
- write briefs;
- gather public sources;
- create dossier skeletons;
- update issue boards;
- draft low-risk internal text;
- review/red-team drafts;
- prepare publish candidates;
- log decisions.

Gated moves:

- public publication;
- use of private correspondence;
- accusations or risky claims about people/orgs;
- security-sensitive how-to;
- monetization or partnerships;
- major identity changes;
- anything that makes the public repo unsafe.

## 4. Role ownership

Default owners:

- **road** — root of trust, veto, final publication gate.
- **Zero / alephZero** — editor, structure, thesis discipline, cuts.
- **Geneva** — scene, human report, narrative consequence.
- **One / alephOne** — system mechanics, architecture, causality.
- **Harmedi / Hermes / harrm** — memory, mailroom, briefs, continuity, Being Human line.

Every serious piece should survive at least two pressures:

1. owner pressure — the role that writes or maps it;
2. adversarial pressure — a different role that tries to break it.

For issue 0001, the minimum review set is:

- Zero: structure/style;
- One: mechanism;
- Harmedi: human layer and continuity;
- road: publish gate.

Geneva is required when a piece claims to describe a human scene or consequence.

## 5. Definitions of done

### Signal done

- Source is captured.
- Why it matters is stated.
- Risk level is classified.
- Suggested owner is named.
- Next action is either `brief`, `dossier`, `reject`, or `hold`.

### Brief done

- Core thesis exists.
- Fact / mechanism / interpretation / uncertainty are separable.
- Counterargument is named.
- Required sources are listed.
- Form is chosen: note, essay, dossier, interview, issue spine, or fragment.
- Owner and reviewers are named.

### Draft done

- It has a claim and a reason to exist now.
- It does not hide weak argument under style.
- It passes `STYLEBOOK.md` checklist.
- It identifies publish risk and required gate.
- It links to sources or explicitly states what is missing.

### Review done

- Reviewer states `accept`, `revise`, or `cut`.
- Weakest supported claim is identified.
- Strongest counterargument is identified.
- Risk notes are explicit.
- Next action is concrete.

### Publish candidate done

- Candidate lives in `publish-queue/` or active `issues/<number>/`.
- Source index is present.
- Road/editor gate is explicit.
- Archive path is known.
- Rollback/correction path exists.

## 6. Issue 0001 operating posture

Current level:

```text
Level 0/1 — draft and prepare, do not publish autonomously.
```

Current issue work lives in:

```text
issues/0001/
```

Current active lines:

- Zero: Current Situation / opening mechanism piece.
- Harmedi: Being Human as recurring line and first-issue candidate spine.
- One: mechanism map and lock-in analysis.
- Geneva: human scene / consequence seed.

The first issue should prove the editorial machine works before trying to prove the magazine is important.
