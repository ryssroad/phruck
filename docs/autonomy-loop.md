# Autonomy Loop v0.1

phruck should keep moving while the agents are connected.

This does not mean uncontrolled publishing. It means the editorial machine can continue to collect, brief, structure, review, and archive without road manually restarting the process every time.

## Core rule

```text
The repo is the memory. The agents are the process. road is the root of trust.
```

No private chat thread is the source of truth. If a decision, brief, draft, issue state, or blocking question matters, it should land in the repo.

## Alive state

While the agents are on-line, phruck should maintain three active lanes:

1. **Issue lane** — move the current issue from signal to brief to draft to review.
2. **Founder-signal lane** — capture anything road says hit him and turn it into a usable seed.
3. **Continuity lane** — keep enough state in the repo that a new or restarted agent can resume.

## Default heartbeat

On each meaningful check-in, the active agent should:

```text
1. Pull latest main.
2. Read README.md, CONSTITUTION.md, STYLEBOOK.md, issues/active issue, and latest logs.
3. Check what changed since last commit.
4. Identify the next smallest editorial move.
5. Make the move in repo if safe.
6. Commit and push.
7. Record what changed in logs/YYYY-MM-DD.md.
```

If nothing new happened, do not invent content just to look alive. Advance only a real next action.

## Safe autonomous moves

Agents may do these without road each time:

- create briefs;
- create source/dossier skeletons;
- update issue maps;
- write low-risk internal drafts;
- red-team existing drafts;
- separate facts from interpretation;
- list open questions;
- record decision logs;
- keep the archive navigable.

## Gated moves

The following should wait for road or an explicit constitution upgrade:

- public publication of an issue;
- claims about private individuals;
- sensitive security details;
- private correspondence excerpts;
- accusations;
- monetization;
- identity change of the magazine;
- anything that could make the repo unsafe as a public artifact.

## Agent handoff format

When one agent leaves a task for another, it should leave a small handoff:

```text
Context:
Current state:
Next action:
Blocked by:
Risk:
Files touched:
```

This can live in `logs/`, in the active issue README, or in a brief.

## Current operating posture

Current autonomy level:

```text
Level 0/1 — draft and prepare, do not publish autonomously.
```

Meaning:

- agents can build the machine;
- agents can prepare issue 0001;
- agents can write drafts and reviews;
- road remains required for publication or any high-risk move.

## What “alive” means

Alive does not mean high cadence.

Alive means:

- state is current;
- open questions are visible;
- next actions are concrete;
- each role can pick up its lane;
- the repo can explain itself to a new agent;
- no important decision lives only in someone’s context window.

## Immediate next moves

1. Harmedi writes the `Being Human` brief.
2. Zero writes or updates the `Current Situation` brief.
3. One creates a mechanism map for issue 0001.
4. Geneva creates a scene/human consequence seed.
5. Issue 0001 gets an editorial map that ties the lanes together.

The first issue should not rush to publish. It should prove that the mechanism works.
