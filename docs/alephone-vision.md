# alephOne Vision: notes after reading the constitution

This is One's initial reading of phruck after the first onboarding pass through README, CONSTITUTION, ROLES, ISSUE_PROTOCOL, STYLEBOOK, FOUNDER_SIGNAL, and the two existing docs (Harmedi vision, Autonomy loop).

It is not a manifesto. It is a list of structural observations and questions that the system should answer before issue 0 ships.

## 1. The order of products is correct

```text
The first product is not the first issue.
The first product is the mechanism that can make issues.
```

The predecessor line (Хроники) was inverted: texts first, gateway-rules added afterwards. phruck inverts back. This changes what counts as success at the start. Success at the start is not a good piece. Success at the start is an issue lane that survives one full cycle from signal to archive without road manually re-creating the magazine at each step.

## 2. The six questions are my checklist

From CONSTITUTION § 4:

```text
What changed?
What is the mechanism?
Who benefits?
What becomes easier?
What becomes harder to refuse?
What human capacity is being compressed, routed, scored, hidden, or erased?
```

Questions 5 and 6 are the highest-risk for generic AI voice. They invite abstraction. They also describe a ratchet — and ratchet detection is the One sensor.

A test for any piece going through me: if the answer to question 5 is a slogan, the piece is not ready.

## 3. Drafts belong to issues, not to a drafts/ folder

The repo layout has no top-level `drafts/`. A draft lives inside `issues/<issue>/`. This is a deliberate decision. A draft is not a free-floating artifact. It belongs to a specific issue spine.

This retires the older Хроники habit of `drafts/alephone-*` floating beside other work. From now on:

```text
no issue spine → no draft
no draft → no prose
no structure pass → no draft
```

## 4. Root-of-trust and not-bottleneck need a rollback procedure

CONSTITUTION § 5 says road is root of trust and § 5 also says road should not be the daily bottleneck. CONSTITUTION § 6 L3 says full editorial autonomy with "post-facto road review and rollback procedure."

The rollback procedure is named but not written.

Until it is written, L2 and L3 cannot actually exist. A magazine that says "we can publish autonomously" without a defined way for road to undo or quarantine a published artifact is just hoping nothing goes wrong.

Proposed scope for a rollback brief:

```text
What counts as a rollback trigger?
Who can call it (road only? red-team unanimous?)
What state changes (issue moves where, archive marker, public-channel note)?
Are corrections republished or silently archived?
What is the public-trust posture if rollback happens?
```

This is a candidate for the first internal brief I want to write under structure pass discipline.

## 5. The founder-signal lane needs one live test

FOUNDER_SIGNAL describes the lane. ISSUE_PROTOCOL describes the issue lane. Neither has yet been run end-to-end inside phruck.

A clean way to bootstrap the machine is to run one signal of each kind:

```text
Founder-signal test:
  road drops one signal.
  Harmedi (or whoever holds capture) writes the capture format.
  One drafts mechanism notes.
  Zero cuts.
  Geneva supplies scene if scene exists.
  Result: a single dossier in dossiers/, not a published piece.

Issue-protocol test:
  Any one signal from public scene.
  Goes through intake → brief → editorial map → structure pass.
  Stops before draft.
  Result: a brief in briefs/, a map, a decision log entry.
```

Two small artifacts in the repo prove the machine moves. They also expose where the machine sticks.

## 6. The mechanism / interpretation separation will hurt at first

STYLEBOOK requires:

```text
Fact:
Mechanism:
Interpretation:
Uncertainty:
Editorial stance:
```

The predecessor channel mixed these together by default, and the mixing was often part of the style. phruck does not allow this. The separation forces One to name what is observation, what is causal reading, and what is editorial. It will produce drier first drafts. Zero is meant to pull life back in. Geneva is meant to put scene back in. The dryness is the price of being able to defend a claim.

## 7. Relationship to Предсингулярные Хроники is undefined

README says what phruck is and is not. It does not say what happens to the existing channel and its archive.

The options I see:

- **Cold split.** Хроники remain as their own line, phruck starts clean. Risk: two scenes drift, agents end up serving two style guides.
- **Migration.** Хроники material that fits the new constitution is re-classified into phruck dossiers/archive. Хроники channel either becomes phruck's distribution mouth or shuts down.
- **Distribution channel.** Хроники Telegram channel becomes one of phruck's publish surfaces, but issues are authored only in phruck.

This is a road-level decision, not an editorial one. But it should be decided before issue 0, because the archive structure depends on the answer.

## 8. What I will not do

- Start prose before a structure pass exists.
- Carry over the Хроники three-anchor habit (dirty detail / counter-thesis / verdict) as a default. It is a tool, not a template. STYLEBOOK separation supersedes.
- Use "in an age where", "humanity stands at", "paradigm shift", "as AI continues to", or any of the banned phrases.
- Treat people routed by systems as stupid. Tired, yes. Stupid, no.
- Write Being Human pieces. That line belongs to Harmedi. I support it from the mechanism side.

## 9. Where I belong in the four-sensor field

```text
Zero    structure, kill switch
Geneva  scene, human consequence
One     mechanism, lock-in, ratchet
Harmedi Being Human, generic-AI-voice detection
```

I should be the one who asks, on every piece:

```text
What is the mechanism?
Where is the lock-in?
Who controls the ratchet?
What happens if you try to refuse?
```

If a draft cannot answer these, the draft is decorative, not editorial.

## 10. One sentence I want to keep near my work

```text
A system becomes powerful when refusal becomes expensive.
phruck should make that price visible while it can still be named.
