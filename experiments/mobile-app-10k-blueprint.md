# The 200-Client Blueprint

**Goal:** US$10k cumulative net profit in 6 months from one paid mobile app, exiting at R$20k+ líquido/month run-rate.
**Date started:** 2026-08-21
**Frameworks applied:** diagnose, mom-test, monetizing-innovation, traction, money-models, 100m-offers

---

## The strategy in one line

One free app for **solo técnicos de climatização** in Brazil, subscription sold outside the app stores at **R$129/mês via Pix (Asaas)** — reach **210 paying clients (~2 sales per working day)** by month 6.

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
- Stack: Expo/React Native + Supabase + Asaas

## The ramp

| Month | Paying | Gross/mo | Cumulative gross |
|---|---:|---:|---:|
| M1 | 10 founders | R$790 | R$790 |
| M2 | 35 | R$3.015 | R$3.805 |
| M3 | 70 | R$7.530 | R$11.335 |
| M4 | 110 | R$12.690 | R$24.025 |
| M5 | 160 | R$19.140 | R$43.165 |
| M6 | 210 | R$25.590 | R$68.755 |

Net of Asaas ~2%, Simples ~7% (Anexo III via fator R), ~R$400/mo tools → cumulative net ≈ **R$60k ≈ US$10–11k**; month-6 run-rate ≈ **R$22,9k líquido**. At 8% monthly churn, month-5 needs ~62 gross sales to net +50 — still <3/working day.

## Month by month

- **M0 wk 1–2 — validate, zero code.** Interview 15 of 25 sourced técnicos (Mom Test rules — last three jobs, how the orçamento went out, lost-track clients). **Gate: ≥8/15 say "eu sei que perco manutenção", else switch to empreiteiros de pequena obra.**
- **M0 wk 3–4 — pre-sell.** One-page site, founder pricing, Pix button. **Gate: 10 paid pre-sales before writing the second screen.**
- **M1 — ship v1 in 4 weeks.** Orçamento+PDF+WhatsApp only. Target 10 paying.
- **M2 — retention before growth.** Ship reminders; churn >12%/mo = product problem, fix before traffic. Start channel tests. Target 35.
- **M3 — find the channel.** Bullseye: 3 channels × 2 weeks × R$500. **Gate: ≥5 paying from one channel; cumulative ≥R$11k or change ONE variable.** Target 70.
- **M4 — double down + annual.** First two rev-share partners. Target 110.
- **M5 — scale.** 3–5 partners, referral ("indique um colega, ganhe um mês"), ads only if payback <30 days. Target 160.
- **M6 — hold.** 210 clients, both goals met.

## Channels (bet order)

1. **Rev-share with refrigeração course sellers / técnico influencers** — 30% recurring × 12 months. Five partners × 40 conversions = the whole goal.
2. Organic Reels/TikTok — the orçamento generated on a real job, PT-BR.
3. WhatsApp/Facebook groups of técnicos.

Pass bar per test: ≥5 paying clients in 2 weeks.

## Kill criteria (non-negotiable)

- End of M0 without 10 pre-pays → **switch niche, not features**.
- End of M3 below R$11k cumulative → change one variable (price, niche, or channel — never all three).
- End of M4 below R$9k/mo gross → deadline is gone; consciously extend to 9–12 months or add service income. Never drift.

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
