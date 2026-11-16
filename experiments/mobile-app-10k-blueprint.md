# The 200-Client Blueprint

**Goal:** US$10k cumulative net profit in 6 months from one paid mobile app, exiting at R$20k+ líquido/month run-rate.
**Date started:** 2026-08-21
**Frameworks applied:** diagnose, mom-test, monetizing-innovation, traction, money-models, 100m-offers

---

## The strategy in one line

One free app for **solo técnicos de climatização** in Brazil, subscription sold outside the app stores at **R$129/mês via Pix (Asaas)** — reach **250 paying clients (~2–3 sales per working day)** by month 6. (Target raised from 210 to 250 so the goal still holds after paying partner commissions — see the ramp.)

## Why not a classic paid app

At $4.99 one-time you need 1,100+ new sales every month forever. At R$129/mo you need ~200 humans total to say yes. Going from a $5 price to a $99+/yr price cuts the required audience ~20x — on a 6-month deadline, convincing 200 people is a hustle problem; convincing 1,500/month is a distribution-machine problem you don't have time to build.

## Why this niche

| Criterion | Climatização | Beleza | Motoristas de app | Personal trainers |
|---|---|---|---|---|
| Money per job | R$150–800 | R$30–120 | R$20–40 | R$80–200 |
| Software penetration | Very low | Saturated | Low, no WTP | Saturated |
| Phone-first workflow | Yes | Yes | Yes | Partly |
| Reachable community | Huge (courses/influencers) | Fragmented | Won't pay | Influencer-gated |
| Can charge R$99+/mo | Yes | Hard | No | Yes |

Incumbents (Auvo, Field Control, Produttivo) price for companies with teams; the solo técnico is the underserved beachhead.

## The product (three features, nothing else)

1. **Orçamento in 60 seconds** → branded PDF over WhatsApp.
2. **Automatic manutenção reminders** — every split needs cleaning ~every 6 months; the app remembers and drafts the client WhatsApp message. *This feature is the business:* it makes the user money, which justifies the price. Pitch: *"Você instalou 84 aparelhos este ano. 31 estão vencidos pra limpeza. Isso é R$4.650 parado."*
3. **Recebíveis** — who owes, what's paid, month total.

## Pricing

- **R$129/mês** standard · **R$79/mês founder rate, lifetime, first 30 only** (pre-sale engine)
- **R$1.290/ano** from month 4 — annual cash upfront is what funds ads within the 30-day payback rule (money-models)
- Billing via Asaas (Pix + cartão), app unlocks via backend, no purchase links in-app → no store commission, revenue in BRL, no FX/payout lag
- **Store-rules risk (iOS):** removing purchase links does *not* guarantee compliance — Apple's App Review Guidelines (3.1.1 / 3.1.3) can require in-app purchase for single-user subscriptions, and "web-only unlock" apps sometimes pass review and sometimes get rejected. The primary funnel here sells on the web *before* install (pre-sale + partners), which helps but is not a safe harbor. **Contingency:** if Apple blocks the iOS build, enable IAP on iOS at R$159/mês (grossing up Apple's 15%) while keeping R$129 on web/Android; if ~40% of subs end up on iOS IAP, that costs ≈ R$1.6k/mo at month 6 — absorbed by the raised 250-client target.
- Stack: Expo/React Native + Supabase + Asaas

## The ramp

| Month | Paying | Gross/mo | Partner commission | Cumulative gross |
|---|---:|---:|---:|---:|
| M1 | 10 founders | R$790 | — | R$790 |
| M2 | 40 | R$3.660 | — | R$4.450 |
| M3 | 80 | R$8.820 | — | R$13.270 |
| M4 | 130 | R$15.270 | −R$774 | R$28.540 |
| M5 | 190 | R$23.010 | −R$2.477 | R$51.550 |
| M6 | 250 | R$30.750 | −R$5.108 | R$82.300 |

Commission column assumes the partner channel goes live in M4 and partner-attributed clients grow to **60% of standard-rate clients by M6**, each paying the 30% rev-share (first 12 months). Net of Asaas ~2%, Simples ~7% (Anexo III via fator R), ~R$400/mo tools **and these commissions** → cumulative net ≈ **R$64k ≈ US$11–12k**; month-6 run-rate ≈ **R$22,5k líquido com comissões pagas** — the R$20k/month goal holds. At 8% monthly churn, month-5 needs ~70 gross sales to net +60 — ~3/working day.

## Month by month

- **M0 wk 1–2 — validate, zero code.** Interview 15 of 25 sourced técnicos (Mom Test rules — last three jobs, how the orçamento went out, lost-track clients). **Gate: ≥8/15 say "eu sei que perco manutenção", else switch to empreiteiros de pequena obra.**
- **M0 wk 3–4 — pre-sell.** One-page site, founder pricing, Pix button. **Gate: 10 paid pre-sales before writing the second screen.**
- **M1 — ship v1 in 4 weeks.** Orçamento+PDF+WhatsApp only. Target 10 paying.
- **M2 — retention before growth.** Ship reminders; churn >12%/mo = product problem, fix before traffic. Start channel tests. Target 40.
- **M3 — find the channel.** Bullseye: 3 channels × 2 weeks × R$500. **Gate: ≥5 paying from one channel; cumulative ≥R$13k or change ONE variable.** Target 80.
- **M4 — double down + annual.** First two rev-share partners. Target 130.
- **M5 — scale.** 3–5 partners, referral ("indique um colega, ganhe um mês"), ads only if payback <30 days. Target 190.
- **M6 — hold.** 250 clients, both goals met with commissions paid.

## Channels (bet order)

1. **Rev-share with refrigeração course sellers / técnico influencers** — 30% recurring × 12 months (this payout is deducted in the ramp math above). Five partners × 40–50 conversions ≈ the partner share of the goal.
2. Organic Reels/TikTok — the orçamento generated on a real job, PT-BR.
3. WhatsApp/Facebook groups of técnicos.

Pass bar per test: ≥5 paying clients in 2 weeks.

## Kill criteria (non-negotiable)

- End of M0 without 10 pre-pays → **switch niche, not features**.
- End of M3 below R$13k cumulative → change one variable (price, niche, or channel — never all three).
- End of M4 below R$11k/mo gross → deadline is gone; consciously extend to 9–12 months or add service income. Never drift.

## Plumbing (where líquido is won)

- Skip MEI (R$81k/yr ceiling breaks by M4). Open **ME no Simples Nacional** now, CNAE 6201-5/01.
- **Fator R:** pró-labore ≥28% of revenue → Anexo III → ~6% vs ~15.5%. Confirm with a contador who has SaaS clients.
- Pix via Asaas settles in days, in BRL. Stores are distribution only.
- Costs: Apple US$99/yr + Play US$25 + Supabase/EAS/domain ≈ R$400/mo; channel tests ≈ R$1.5k once.

## Interview script (M0)

1. Me conta seu último orçamento — como você mandou?
2. Quantos clientes de instalação você tem no total? Quantos voltaram pra limpeza?
3. Como você lembra quem tá vencendo?
4. Já perdeu serviço porque demorou a responder?
5. O que você usa hoje — papel, WhatsApp, planilha?

---

*Assumes FX ≈ R$5,40. Honest odds: ~1-in-3 for a full-time builder who pre-sells first; the gates exist to reveal early which third you're in.*
