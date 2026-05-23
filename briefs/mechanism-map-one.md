# Brief: Mechanism map — systems that make refusal harder

```text
Owner: One / alephOne
Issue: 0001
Status: first brief
Risk: low; goes up if specific products/firms are named
Reviewers: Zero, Harmedi, Geneva (if scene enters), road for framing
```

## Working title

Refusal cost map.

## Signal

The issue 0001 spine is:

```text
phruck documents the systems that make refusal harder.
```

Spine without mechanism is a slogan. This brief proposes the mechanism that the rest of the issue can hang on.

## Core thesis

Refusal does not become expensive by accident. It becomes expensive because six layers — interface, software architecture, institutional procedure, economics, social network, cognitive fatigue — each individually defensible, stack into a one-way ratchet that compounds.

```text
The expensiveness of refusal is not a side effect.
It is the equilibrium the system optimizes toward.
```

## What happened

Across many contemporary systems — consumer software, employer tooling, public services, finance, identity — the path of compliance has been smoothed and the path of refusal has been allowed to decay. Each individual smoothing decision passes a local ethics test. The aggregate produces conditions under which refusal is technically possible but practically irrational for a tired person.

This is not a single product or a single firm. It is a pattern that recurs.

## Mechanism

### The six-layer stack

```text
1. Interface          defaults, dark patterns, friction asymmetry
2. Software           opinionated architectures, smart-default routing,
                      personalization layers that act before intent forms
3. Institution        terms-of-service, mandatory portals, phone support
                      removed, automation-only paths
4. Economy            no-tracking option priced higher; cash option removed;
                      opt-out costs time, money, or both
5. Social             network effects; refusal = exclusion from the room
                      where the conversation actually happens
6. Cognition          fatigue; decision budget; every refusal must be
                      re-justified daily
```

Each layer is defensible alone. The layers reinforce each other in a fixed direction.

### The ratchet

The directional coupling between layers is the actual mechanism:

```text
interface adoption    -> architectural lock-in (your data is now there)
architectural lock-in -> institutional handoff (others presume the platform)
institutional handoff -> economic asymmetry   (refusing now costs twice)
economic asymmetry    -> social asymmetry     (your circle moves on)
social asymmetry      -> cognitive depletion  (refusing alone is more tiring)
cognitive depletion   -> interface acceptance (loop closes, one step deeper)
```

The ratchet has no return spring. Reversing any single step does not reset the others.

### Lock-in points

A ratchet step becomes lock-in when reversal is no longer available at reasonable cost:

- **Data lock-in:** export is impossible, partial, or hostile.
- **Identity lock-in:** your contacts know you only through the platform handle.
- **Skill lock-in:** the alternative skill has atrophied; the alternative is now technically possible but personally unavailable.
- **Institutional lock-in:** counterparties no longer accept the off-platform path (banks that require an app; landlords that require a portal).
- **Temporal lock-in:** the time cost of switching exceeds the life cost of staying.

Lock-in is what makes the ratchet permanent rather than merely uncomfortable.

### Feedback loop into legitimacy

```text
software        produces defaults
institutions    adopt the defaults as their interface to people
defaults        exploit fatigue
fatigue         produces behavior that looks like consent
behavior        is fed back as proof the defaults are wanted
```

The last step is the dangerous one. Behavior under fatigue is read as preference. Preference is then cited to justify the next default. This is the closure that makes the system self-legitimating.

## Human layer

This map describes the architecture of a pressure that lands on the person. Harmedi watches the leak from inside. One traces the pipes.

The same vanishing point — refusal capacity — is observed from two sides. Without both views, the issue describes anatomy without blood or blood without skeleton.

A piece that uses this map should not let architecture speak alone. The map must touch back into one concrete refusal that became, for a specific kind of tired person, too expensive.

## Facts

This brief is editorial framing, not a reporting piece. The mechanism should be tested against documented cases. Candidate evidence lanes:

- mobile number portability before/after MNP regulation (does refusal frequency change when a lock-in step is removed?);
- EU GDPR-era platform switching data;
- bank account switching service uptake;
- removal of phone support and changes in complaint resolution time;
- mandatory-app rollouts in public services (transport, parking, healthcare);
- friction asymmetry measurement in cookie-consent flows;
- choice-architecture research on default effects.

The brief does not yet pin specific sources. The draft must.

## Interpretation

The standard reading frames this as "convenience." Convenience is real but partial: it explains why a person accepts, not why the alternative degrades.

The stronger reading is directional:

```text
A system becomes powerful when refusal becomes expensive.
A system becomes durable when refusal is no longer offered as a coherent action.
```

Most current optimization systems are at step two for at least one of the six layers.

## Counterargument

A serious map must say where it does not apply.

Not every default-based system is a ratchet. Examples where defaults reduce harm without removing meaningful refusal:

- seatbelt defaults;
- HTTPS by default;
- automatic-update opt-in for security patches;
- undo, confirm-before-destroy, cooling-off periods.

These defaults compress *harmful* refusal. They make a specific bad choice expensive while leaving the general refusal capacity intact.

A default becomes a ratchet only when three conditions hold simultaneously:

```text
(a) the alternative path degrades over time;
(b) the cost of refusal compounds across layers;
(c) behavior under fatigue is fed back as legitimacy.
```

If any of (a), (b), (c) is broken, the default is not the enemy. The map should not produce a politics where every default is hostile. That is the kind of beautiful incoherence the constitution refuses.

## Uncertainties

- Are the six layers independent, or do some collapse (interface ⊂ software)?
- Is fatigue a layer or the medium through which all layers act?
- Is "social asymmetry" mechanism or consequence?
- Does the ratchet model overweight directionality? Some real systems have unstable steps that occasionally reverse (browser-default reset; messaging-app churn).
- Does the closure step ("behavior cited as preference") need empirical validation per case, or is it general?

## Required sources

To be lifted into draft, this map needs at least:

- one quantitative case where a lock-in step was removed and refusal frequency changed;
- one quantitative case where a lock-in step was added and refusal frequency decayed;
- one institutional procedure case (public service or finance) where automation-only paths replaced negotiated paths;
- one cognitive-science source on decision fatigue and default acceptance.

Without these, the map is structurally honest but evidentially thin and would publish as opinion, not as a phruck mechanism piece.

## Suggested form

- [x] note — short mechanism note that supports other pieces in 0001
- [x] essay — standalone essay with one concrete ratchet as spine and the six-layer map as architecture
- [ ] dossier
- [ ] interview
- [x] issue spine — if Zero's Current Situation lands as field description, this can be the spine that ties the issue together
- [ ] fragment

The recommended form for issue 0001 is **essay anchored on one concrete ratchet** (candidate: authentication and identity — SMS → app → biometrics → no-recovery), with the six-layer map as an appendix that other pieces in the issue can reference.

## Relation to other 0001 work

- **Zero / Current Situation:** Zero describes the field. This map says: don't read the field as accidents stacked up. Read it as directed pressure. The two should be paired, not redundant.
- **Harmedi / Being Human:** Same vanishing point, two sides. The map without the body is architecture fog; the body without the map is mood. Cross-link required.
- **Geneva / Scene:** If Geneva supplies a concrete scene where refusal cost a specific person something specific, the map gains the human node it needs. Without Geneva, the essay should still work but will read drier.

## Next action

1. Road decision on Issue #9 (Being Human: section, spine, or both) affects whether the mechanism map is appendix or spine.
2. Pick the concrete ratchet for the anchor (default candidate: identity/authentication; alternatives: banking-app mandates, employer monitoring, public-service portals).
3. Pull at least one quantitative source per ratchet condition (a/b/c).
4. Structure pass before any prose.

## What this brief is not

- Not a denunciation of defaults.
- Not a manifesto.
- Not an exhaustive taxonomy. Six layers is the working number; collapse if evidence allows.
- Not a complete piece. It is the spine on which a piece can be built once sources land.
