# FamiliarVoice business status — October 7, 2026

This snapshot updates Zenith's planning from the FamiliarVoice repository, not from the stale Windows Desktop checkout. Source baseline: `ZachPoli/familiar-voice-notifications` main at `c182bb817b9a34e9e1b8bf1b7defaf0e992a30f5`, plus open issue #41 inspected October 7. Repository reports are evidence of recorded work, not a fresh production audit.

## What has progressed

- FamiliarVoice has reached real Google Play Internal Testing. The October 3 state record reports v22 / `0.1.0-beta03-usage-notices` published to existing internal testers and installed on the owner's Pixel 10a.
- Owner-reported v22 checks confirmed on-demand offer/playback and exactly-once Automatic playback. Paused produced no playback; absence of an offer was not separately established.
- Account access, consent-based voice enrollment, owner-controlled sharing, deliberate contact assignment and revocation have progressed beyond the earlier MVP. Prior physical evidence includes shared-voice playback between two phones and fallback after revocation; it does not certify every later build or user journey.
- UI, invitation recovery, assignment visibility, persistent on-demand offers and privacy disclosures have received substantial stabilization work. Open issues still require acceptance evidence; implemented fixes are not automatically closed release gates.
- Usage enforcement/retention foundations are merged and deployed **disabled**, according to issue #41. Android v22 includes limit notices. Deployment is not proof of active cost protection, and the planned October 5 checkpoint is not proof activation occurred.

## What is not yet established

Public paid-launch readiness, paid customers, recurring revenue, retention and acquisition economics are not established by the reviewed evidence. The pricing document's five original lifetime-free testers are not proof that five people are currently active or paying.

The October 3 launch checklist names **November 12, 2026 as a conditional target**, not a promised release date. The September 30 delivery review describes a limited free launch; no paid offer is committed by the launch checklist.

Remaining gates include:

1. Verified provider/commercial terms and current economics.
2. Safe activation and physical acceptance of usage/cost protection, including renewal baseline, storage, deletion/recovery and operational ownership (#41).
3. Automated self-service account deletion (#20).
4. Full accessibility and unfamiliar-user journeys, broader Android/device coverage, glasses routing and background/offline/restart behavior.
5. Current Play/release/support requirements and evidence closing remaining beta issues.
6. A verified payment/entitlement path and willingness-to-pay evidence before describing the product as monetized.

## Pricing is still a hypothesis

The source pricing plan proposes Personal at $9.99/month or $99.99/year and provisional Plus at $14.99/month or $149.99/year. Its October 3 clarification explicitly calls its allowances and cost examples historical assumptions, not verified current provider rates. Do not copy those allowances into a public sales promise or use the historical margin calculation as a current forecast.

Five original testers were promised Personal free for life under bounded terms. Preserve that commitment; measure new paid demand separately.

## Weekly operating record to establish

Record active outside testers, completed core journeys, repeat weekly use, blocking failures, support minutes/user, measured speech cost/user, paid intent, actual payments and the next release blocker. Leave unknown values unknown. This makes future product allocation depend on customer evidence rather than repository activity.

## Sources

- [Pinned project state](https://github.com/ZachPoli/familiar-voice-notifications/blob/c182bb817b9a34e9e1b8bf1b7defaf0e992a30f5/PROJECT_STATE.md)
- [Pinned launch checklist](https://github.com/ZachPoli/familiar-voice-notifications/blob/c182bb817b9a34e9e1b8bf1b7defaf0e992a30f5/docs/BETA3_LAUNCH_CHECKLIST_2026-10-03.md)
- [Pinned pricing plan](https://github.com/ZachPoli/familiar-voice-notifications/blob/c182bb817b9a34e9e1b8bf1b7defaf0e992a30f5/docs/PRICING_PLAN.md)
- [Cost-protection readiness #41](https://github.com/ZachPoli/familiar-voice-notifications/issues/41)
- [Account-deletion gate #20](https://github.com/ZachPoli/familiar-voice-notifications/issues/20)

Only high-level product/business facts are summarized here. Private tester identities, message content, credentials and operational recovery details are excluded.
