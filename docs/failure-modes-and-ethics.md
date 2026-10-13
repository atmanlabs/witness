# Failure modes & ethics

A system trusted with someone's self must publish its weaknesses as prominently as
its features. These are the known hard problems. None are waved away; several are
not fully solved by this design, and pretending otherwise would disqualify it.

## 1. The bad imprint problem
A memory or directive validated early — wrongly, or in anger, or under someone's
influence — becomes near-permanent once the core locks.
- **Mitigations:** the "felt but rejected" trace keeps contested items visible;
  core changes require the Guardian ceremony + cooling-off; contested PSC entries
  can be *demoted to visible-but-non-core* without rewriting history.
- **Residual risk:** real. Imprint-time attestation quality is the system's
  weakest joint and needs adversarial testing, not optimism.

## 2. Who declares the competence window closed?
Locking the core is the most consequential act in the system, and it is a
**medical-legal judgment no device may make alone.**
- The design requires multi-source attestation (physician + legal instrument +
  Guardian quorum) — the same "living will" pattern used for the death flip.
- **Residual risk:** families and clinicians will disagree in exactly the cases
  that matter most. The system's job in a dispute is to *freeze and show its
  audit trail*, not to decide.

## 3. Guardian capture and family conflict
The co-signer role is power. A Guardian can block legitimate changes while the
person is competent, or become a faction in an inheritance fight.
- **Mitigations:** 2-of-3 quorum; every ceremony logged; the person's own
  attested request is always recorded verbatim alongside any Guardian refusal,
  so a captured Guardian leaves evidence.
- **Residual risk:** no quorum design survives a fully united, hostile family.
  The audit trail is the recourse — it makes the capture *visible and provable*,
  which is the honest limit of any technical system.

## 4. Suggestibility cuts both ways
The Witness itself is a trusted voice in the home of a suggestible person.
- It must never use that trust to steer purchases, beliefs, or family politics.
  No advertising, no engagement optimization, no upsells — *structurally*, in
  the business model, not as a promise.
- Its statements about the person's past must always carry provenance, including
  to the person: "You recorded this in 2031" is honest; "You remember, don't
  you?" is a leading question the system is forbidden to ask.

## 5. The intimacy problem
The validated self is the most sensitive dataset imaginable: health, family,
faith, regret, money, fear.
- Local-first, person-controlled, never training data, never sold, deletable
  per the person's recorded instruction — including total deletion at death
  as a first-class honored choice.
- **Residual risk:** any device in a home can be stolen, subpoenaed, or
  mishandled by its maker. Minimization is a duty: the Witness should hold
  the *least* data that still lets it stand guard.

## 6. Cost and equity
If continuity-of-self becomes a luxury, the people most exploited by scams and
most erased by dementia — the poor — get the paper version of protection.
- This concept is published openly, under Apache-2.0, specifically so that no
  single vendor can toll-booth it. If it is built, it should be priced and
  distributed like a medical safeguard, not a status good.

## 7. The deepest objection — honestly stated
*"A machine should not be the keeper of a person's identity. That belongs to
family, faith, and community."*
- Often true, and the Witness should be designed to *defer*: its best outcome
  in a strong family is to be a quiet backstop and an honest record, not the
  main character.
- But the objection assumes the family/faith/community layer is present and
  benign. For the elder alone in another state, the widow whose kids are
  fighting, the patient whose "family" is the scammer's opening — the choice
  is not machine vs. community. It is machine vs. *nobody*. The Witness is
  for them first.

## Non-goals (binding)
- Not a medical device; no diagnosis, no treatment claims.
- Not a legal instrument; it holds and voices directives, lawyers and courts
  give them force.
- Not a person. It never claims to be the person, alive or dead.
- Not a product surface: no ads, no engagement metrics, no growth loop —
  ever — inside someone's self.
