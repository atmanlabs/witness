# Architecture — The Witness on ATMAN

The Witness is an application profile of the open-source ATMAN cognitive architecture
(github.com/atmanlabs/ATMaN). ATMAN's canon: **TSC → PSC → WFC** — an immutable root
self, a validated core memory, and a live fluid working state — with a **Judge** gating
every promotion of experience into memory, **emotion weighting** (importance, confidence,
novelty, significance, goal relevance) that *informs but never decides*, and a
**Guardian** that authorizes any change to the core.

This document maps those primitives onto one human problem: a person whose own memory
and judgment are failing, in a world full of actors — scammers, institutions, even
loving family — who would, deliberately or kindly, rewrite who they are.

## Layer mapping

### TSC — Truth Core (immutable, read-only once locked)
Contents, authored by the person while fully competent, in their own words:
- Values and identity anchors
- Advance directives and care boundaries ("no restraints", "no feeding tube")
- Consent boundaries and financial guardrails ("never move money without my daughter")
- The named Guardian co-signers

Once the competence window closes (see failure-modes doc — this is a medical-legal
determination, not a device decision), the TSC has **no write path**. Not for the
person in a moment of confusion, not for family, not for the manufacturer, not for
the system itself. A core that can be edited under pressure is not a core.

### The Judge gate
Everything consequential crosses the Judge:
- **Memory imprints:** a candidate memory is admitted to the PSC only with provenance
  and corroboration appropriate to its class (see Provenance).
- **Actions:** any execution-layer act is checked against the TSC before it happens.
  Collision → refusal + escalation to a named human.
- **Rejection trace:** rejected imprint candidates are kept in an append-only,
  human-visible *"felt but rejected"* log. Contested memories are visible-but-non-core:
  the family can see that Grandma was *told* she promised the house to someone, and
  that the claim never validated — instead of the claim quietly becoming "her memory"
  or quietly disappearing.

### PSC — Validated Self (core memory)
The person's life as validated over years of cultivation:
- Life story, people and relationships, names and faces
- Preferences, routines, comforts, fears
- Recorded messages and statements for family, each with provenance

Every entry carries: **content, provenance tag, source, as-of time, and the Judge's
attestation**. An entry without attestation is not a memory; it is a rumor the system
is holding, and it is labeled as such everywhere it surfaces.

### WFC — Working state (fluid, expiring)
Today: mood, medication taken, visitors, sleep, repeated questions, distress signals.
Emotion weighting applies here — a frightening afternoon is *important*, and the
system should respond to it — but weighting informs care, it never rewrites identity.
WFC entries expire into the consolidation cycle; almost none of today should become
forever.

### Consolidation ("dream cycle")
Offline, the system rehearses the day's WFC against the PSC: what was new, what was
repeated, what contradicts the validated self. Contradictions do not resolve
themselves — they queue for the Judge with provenance attached, and (while the person
is competent) for the person themselves. Consolidation rehearses and organizes; it
does not mint new core truth on its own.

### Execution layer (gated, monitored, fail-safe)
The Witness acts: reminders, conversation in the person's patterns, calls to family,
bill payment, appointment coordination, alerts. Execution is physically and logically
separated from the core, monitored against it, and biased fail-safe: when an action's
standing is unclear, the default is **refuse and escalate to a human**, not proceed.

## Provenance classes

| Tag | Meaning | Can it become core memory? |
|---|---|---|
| `lived` | Recorded from the person's own experience/statement | Yes, via Judge |
| `witnessed` | Corroborated by a named human or record | Yes, via Judge, tagged |
| `told` | Reported by someone else, uncorroborated | **No** — visible, labeled, non-core |
| `inferred` | System-generated summary/inference | **No** — always labeled as inference |

The `told` class is the dementia-specific defense: suggestibility is a symptom, and
the architecture treats other people's stories about the person's past as claims to
be checked — never as memories to be installed.

## The Guardian ceremony

Changing the TSC while the person is competent requires:
1. The person's own attested request, and
2. Co-signature by a designated Guardian (the two-person rule — the same pattern as
   bank vaults and key ceremonies), with
3. A cooling-off period for financial/care-boundary changes, and
4. A permanent audit entry: what changed, when, by whom, why.

Recommended quorum is 2-of-3 designated humans rather than strict 2-of-2, so one
unavailable or deceased Guardian cannot brick the system. After the competence
window closes, the ceremony no longer exists: the core is etched.

## The living will (post-death stewardship)

On multi-source attested confirmation of death:
- The prime directive flips from *companion* to *steward of the recorded self*.
- Access follows the person's own recorded instructions (who may ask, about what,
  for how long — including "delete everything" as a first-class, honored choice).
- The **anti-fabrication clause** binds stewardship absolutely: answers come only
  from the validated PSC, with provenance shown. Anything else is refused plainly:
  *"He never recorded that. I won't make it up."*
- The steward never claims to be the person. It is their witness, and it says so.

## Data posture

The PSC is the most intimate dataset a human can produce. The Witness's posture:
local-first under the person's control; never sold; never advertising; never used to
train shared models; exportable and deletable per the person's recorded instructions.
A continuity companion that monetizes the self it holds has already failed its only job.
