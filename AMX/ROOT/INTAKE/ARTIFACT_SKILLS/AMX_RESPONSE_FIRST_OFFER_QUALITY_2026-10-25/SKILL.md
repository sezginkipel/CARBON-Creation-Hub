---
name: amx-response-first-offer-quality
description: "Improve existing PRI/iSCOPE commercial offer quality when a run produces no qualified buyer question or request for details. Use the existing offer-quality standard, current buyer evidence, offer/pricing gates, and the actual inbound reply record. Do not create a new sales pipeline, score system, worker, or outreach quota."
---

# AMX Response-First Offer Quality Skill

**Lifecycle:** OWNER-DIRECTED CATEGORY A SKILL CANDIDATE / READY FOR GOVERNANCE REVIEW. Runtime adoption, benchmark promotion, and outcome acceptance are not yet proven.

## Objective

Produce at least one attributable, human, interested-party response that asks for information, explanation, scope, proof, sample output, or fit details about a specific offer. This is an offer-quality acceptance signal, **not a sale**. A decline, opt-out, out-of-office notice, automated response, bounce, support message, or unrelated reply does not satisfy it.

Do not penalize send volume or the conversion ratio as a worker score. Do not claim success from sends, opens, drafting, price, tool activity, or raw replies. Do not use another large batch of the same weak approach as the learning response.

## Trigger

Apply after any commercial execution run that has no qualifying response, and during every subsequent response-quality check while the Owner's Category A acceptance remains open. The existing Owner-directed Category A directive is active until the response criterion is evidenced and independently read back.

## Workflow

1. **Anchor the exact cohort.** Read the actual scheduler/task/run identities when a scheduled run exists; distinguish them from a post-run interactive continuation. Read the existing offer/claim record, sent message/thread, current Inbox and Junk Email evidence, and last run receipt. Do not invent a run ID or attribute prior sends to a run that did not send them.
2. **Count incoming first.** For the run window and the attributed send cohort, deduplicate by conversation and recipient. Record unique external offers sent, actual delivery/bounce evidence when available, incoming external messages through the observation cutoff, distinct human replies, and distinct qualifying interested-offer questions. Inspect the actual received message, not just the subject or the word "reply." Keep an immature/no-reply cohort open; no response is not proof of a copy or price cause.
3. **Classify each inbound event separately.**
   - **QUALIFIED_OFFER_INTEREST:** a human interested party asks a question about the specific offer, requests scope or proof/sample details, or asks how the stated deliverable/acceptance works.
   - **DECLINE_OR_OPTOUT:** not accepted as quality success.
   - **AUTO_REPLY_OR_OUT_OF_OFFICE**, **BOUNCE_OR_DELIVERY_FAILURE**, **SUPPORT_OR_ADMIN_ROUTE**, and **UNRELATED_MESSAGE:** not accepted as quality success.
   - Neutral/referral/role-routing responses may be useful learning but do not satisfy the threshold unless the source actually shows offer-specific interest and a request for clarification.
   Preserve existing lifecycle enum/value rules; report this quality classification in the existing receipt rather than inventing a new ledger lifecycle status.
4. **Acquire a non-duplicate skill from evidence.** Identify what was learned from the new reply/no-reply evidence and from relevant existing research. State the changed behavior for the next run, focus areas, source, falsifier/counter-evidence, and acceptance test. Record **learned**, **applied**, and **behaviorally verified** as distinct states. A newly written skill or prompt is not proof that a worker used it; do not invent skill badges/ranks or alter the governed benchmark registry.
5. **Requalify the next executable opportunity.** iSCOPE owns opportunity discovery/qualification; PRI owns external commercial propositions. Verify the recipient's economic role (buyer/client/employer, licensee/acquirer, vendor/supplier, platform/route provider, support/admin, or unknown), decision authority and appropriate route. Distinguish public fact from pain hypothesis, consequence, urgency, budget and purchase intent. State a falsifier for the pain hypothesis. Do not assume a job title or adjacent capability proves budget authority.
6. **Engineer one buyable offer.** In buyer language, state one concrete finished result, what is included/excluded, available proof/sample, dependency/access, turnaround, and a buyer-visible acceptance condition. Do not sell internal AMX/AI architecture or a catalogue. Do not charge for a list of defects or provide bespoke diagnosis/implementation blueprints as an unpaid teaser. Give a representative, prebuilt/synthetic sample when useful; it must demonstrate the deliverable rather than ask the prospect to do the diagnosis.
7. **Remove avoidable response friction.** Use one context-specific, source-backed fact and one bounded outcome, and one low-friction interest CTA that asks whether the recipient wants a specific sample/scope/acceptance detail. Do not make the first reply require the buyer to document their whole process or perform unpaid discovery. Avoid generic "workflow pilot" wording unless it is the buyer's actual buying language. Keep the message concise (normally 50–90 words; an evidence-backed reason may justify more). Short copy is not a substitute for the right buyer, offer, proof or route.
8. **Respect commercial gates.** Before any send, PRI must reread the current source/thread, suppression and dedupe state, offer owner, existing contact route, price basis, capacity, acceptance terms and payment route. For South African offers, apply the current rule of 50% of a defensible comparable low-end benchmark only after scope/comparator and delivery economics are verified. If relevance/authority is unverified, qualify first and price second. Never silently reprice or mass-resend an existing offer; preserve the original sent version and wait states.
9. **Run an honest next-step test.** The next run must name the skill/behavior it will use, exact offer/recipient cohort and why this is different from the failed approach before sending. Do not send unless the existing PRI authority and contact gates pass. After sending, read actual inbox results and source thread again. If no qualifying reply exists, preserve the new learning evidence, change the next test materially, and keep Category A open.

## Current evidence baseline (2026-10-25; not a general benchmark)

- Current reviewed cohort: 12 unique offer messages to 12 recipients, sent 2026-10-20 through 2026-10-21.
- The existing Outlook Inbox contains one associated response in that cohort: Forest Energy's automated out-of-office message received 2026-10-21T04:49:36Z.
- Qualified interested-party responses in this cohort: 0.
- Inbox arrivals during Flight 3 run b6c9f421-40e4-8331-b64b-867436ec0655 (2026-10-25T13:15:56Z–13:39:45Z): 0. The flight made no commercial sends during that window, so this is not an offer-level conversion denominator.
- Existing opportunity records for these offers remain in their current governed states; most are OFFERED / WAITING_FOR_BUYER_RESPONSE / HOLD_ACCEPTANCE_OF_UNRECONCILED_OFFER. Forest Energy is SUBMITTED and waiting for a non-automated buyer response. Preserve existing source keys, versions, lifecycle, and no-follow-up controls.
- Historical predecessor evidence: 11 human/external reply threads among 450 outbound-originated threads (2.44%); 0 of 270 templated YES-CTA threads had a recovered human reply, versus 11 of 180 non-YES threads (6.11%). This cohort predates the current FIRST BREATH regime; targeting, route, maturity and offer mix confound causal attribution. Do not claim the CTA caused the difference.

## Evidence informing the skill

- Existing governing source: AMX/ROOT/INTAKE/CATEGORY_A_INTENTION_TO_OFFER_EXECUTION_ADDENDUM_A_20261019.md (current blob read 2026-10-25: b7c8e78769cff8cafc97b3e79899b09ee9ce4dfc). This source already requires buyer role, sourced fact, pain hypothesis/falsifier, finished outcome, proof, scope/acceptance, pricing, payment route and attribution. The current gap is enforcement/readback, not a need for a second sales system.
- Gong's 2026 executive-sales research says emails over 100 words reply less often in its studied executive cohort, and recommends an offer of value rather than a meeting or discovery-work ask: https://www.gong.io/blog/do-execs-really-reply-to-cold-email-here-s-what-the-data-says
- Gong Labs' CTA analysis of 304,174 emails found an interest CTA performed best for cold emails in its analyzed dataset; this supports testing a low-friction offer-interest CTA, not claiming universal causality: https://www.gong.io/blog/this-surprising-cold-email-cta-will-help-you-book-a-lot-more-meetings
- Sales.co's 2026 analysis of 1,288,605 sent emails classified raw, automated, human and interested replies separately; its dataset reports 0.70% human first responses and 0.24% interested responses. It is a vendor cohort, a benchmark only, and not directly comparable with AMX's cohorts: https://sales.co/research/cold-email-response-rates

## Acceptance and evidence state

Category A acceptance remains **OPEN** until the existing authorized receipt route contains at least one source-backed QUALIFIED_OFFER_INTEREST attributable to a specific offer/thread, followed by independent source readback. That event proves only an interested offer-specific response, not acceptance, contract, invoice, payment or settlement, and not causality of one copy element.

Every failed run must leave a durable readback showing:
- the actual run/task/shared-wake IDs available for that run, separately;
- the send cohort and unique recipients actually attributable to it;
- total inbound arrivals, human replies and qualifying offer-specific interest;
- exact source/thread evidence and the categories of excluded responses;
- the new non-duplicate skill/learning, focus areas, and behavior changed for the next run;
- offer/recipient choice, owner/mandate, before/after state, blockers and next action;
- the existing receipt destination and independent readback result.

Use only the existing Root Intake, opportunity ledger, thread, skill estate and current mandates. No new worker, CRM, response tracker, queue, scoring authority, rank/badge mutation or payment ledger.
