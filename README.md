# THE WITNESS

**A continuity companion for people losing their memory — an AI that holds who you are when you no longer can, and cannot be rewritten by anyone. Not by confusion, not by a scammer, not by family, not by the company that built it. Not even by itself.**

Built on the open-source [ATMAN](https://github.com/atmanlabs/ATMaN) cognitive architecture: an immutable core self, Judge-gated memory, and provenance on every belief.

> Status: **concept / architecture design, published for public discussion and collaboration.** No product exists yet. Nothing here is a medical claim. Failure modes are documented as prominently as features — see [docs/failure-modes-and-ethics.md](docs/failure-modes-and-ethics.md).

---

## The problem

- Roughly **57 million people** live with dementia worldwide (WHO), heading toward an estimated **139 million by 2050**. Every one of them slowly becomes illegible — to caregivers, to family, eventually to themselves.
- US seniors lose an estimated **$28 billion a year** to financial exploitation (AARP estimate; the FBI's *reported* figure alone was ~$4.9B in 2024). The standard defense is bank fraud detection: statistics that know nothing about the person, so they either miss the scam or freeze a grandmother's account for buying groceries — stripping autonomy "for her safety."
- Meanwhile, a grief-tech industry is emerging that sells families chatbots trained on a dead person's messages — systems that will say *anything*, including things the person never said and never believed.

Every existing tool fails the same way: **its memory of the person can be edited** — by a model update, a persuasive stranger, a well-meaning relative, or a terms-of-service change.

## The idea

The Witness is **grown, not installed**. It is cultivated alongside a healthy person over years:

- **While you are fully yourself**, you define your core: your values, your directives, your consent boundaries, in your own words. *"Never move my money without my daughter." "No restraints." "These are my people; these are their names."*
- **Your memories enter through a Judge.** Every experience is weighed before it becomes part of your validated self, and every memory carries a **provenance tag**: *you lived this / someone witnessed this / someone told you this*. Dementia makes people profoundly suggestible; a kind story repeated by a relative can overwrite a real past. The Witness refuses to promote a told-story into a lived memory.
- **A Guardian holds the keys to the core.** Changing a core directive requires you **plus a named human co-signer**, and only while you are certified competent. After that, the core is locked. A son cannot rewrite your boundaries. A care facility cannot soften them. The manufacturer cannot patch them away.
- **It can act — and it can refuse.** The Witness reminds, speaks in your patterns, calls your family, pays your electric bill. Any action that collides with your core is refused *by structure*, not by a policy that can be updated overnight.

### The 2 a.m. test

A scammer coaches her, patiently, over three phone calls, to wire $8,000 to a "grandson in trouble."

The Witness checks the request against the core she wrote at 61, clear-eyed: *never move money without my daughter.*

**Refused.** The daughter gets the call instead.

She keeps her money **and** her dignity — because the refusal didn't come from a bank's algorithm deciding she's incompetent. It came from her own younger self, standing guard.

## After death: the anti-fabrication clause

On multi-source attested confirmation of death, the Witness's prime directive flips from *companion* to *steward* — a living will for the self it holds.

But it operates under a clause no grief-tech product ships:

> **The Witness may only speak from validated memory, with provenance shown. It must refuse to invent.**

When a granddaughter asks, *"What would Grandpa say about my wedding?"* — it answers from what he actually recorded, or it says: *"He never recorded that. I won't make it up."*

A dead person's voice should not be a puppet. Their silence on a subject is also part of who they were.

## Why existing tools can't do this

| Approach | Why it fails |
|---|---|
| LLM companions (mutable cloud memory) | The "person" drifts with every model update; the company can change their personality overnight — and has. |
| Memoir / story apps | Static records. They cannot judge, act, or refuse. |
| Digital legacy settings | Transfer access after death. They hold nothing during life and protect nothing. |
| Advance directives / POA | Paper. Static, contested, and unable to intervene at 2 a.m. |
| Bank fraud AI | Statistical anomaly detection. Knows transactions, not values. False blocks strip autonomy. |
| Griefbots | Trained to *resemble*. No immutable core, no provenance, no duty to refuse fabrication. |

The gap is not intelligence. The gap is **an architecture where the self is structurally incorruptible** — which is the entire design point of ATMAN.

## Architecture (concept level)

- **TSC — Truth Core (immutable):** the person's values, directives, consent boundaries. Read-only once locked.
- **Judge gate:** every memory imprint and every consequential action crosses it. Rejected imprints are logged in a visible *"felt but rejected"* trace — never silently absorbed, never silently erased.
- **PSC — Validated Self:** the life story, people, preferences — each entry provenance-tagged and Judge-approved.
- **WFC — Working state:** today only. Mood, medication, visitors, repeated questions. Fluid, expiring, never allowed to rewrite the self.
- **Execution layer:** acts in the world (reminders, calls, payments) under continuous Judge oversight, with a fail-safe bias toward refusal + human escalation.
- **Guardian:** a separate, deliberately simpler authorizer. Core changes require the Guardian ceremony: the person + co-signer, while competent. No unilateral path exists — for anyone.

Full mapping: [docs/architecture.md](docs/architecture.md) · Prior art in depth: [docs/prior-art.md](docs/prior-art.md) · Failure modes & ethics: [docs/failure-modes-and-ethics.md](docs/failure-modes-and-ethics.md)

## What this is not

- Not a medical device, not a diagnosis tool, not a replacement for human care, family, or legal counsel.
- Not surveillance: the validated self is the most intimate dataset a person can produce. It belongs to the person, lives under their control, and is never training data.
- Not immortality. The Witness holds a person's *recorded, validated* self. It does not claim to be the person, and its refusal to improvise is precisely the respect owed to that fact.

## The honest hard parts

Competence certification (who declares "she can no longer amend her core"), Guardian-key family conflict, bad early imprints, and cost/access equity are real, unsolved problems. They are documented in [docs/failure-modes-and-ethics.md](docs/failure-modes-and-ethics.md) rather than waved away — because a system trusted with someone's self has to be more honest than the industry around it.

## License

Apache-2.0, consistent with the ATMAN project. The concept is published openly so it can be challenged, improved, and — if it deserves it — built by people who will keep the anti-fabrication clause intact.

*An ATMAN needs work, like getting to know someone. You define its core, you live with it, and it grows over time. The Witness simply asks: what if it grew alongside you for a lifetime — and then refused to let the world rewrite you?*
