# The 200-Client Blueprint

**Goal:** US$10k cumulative net profit in 6 months from one paid mobile app, exiting at R$20k+ líquido/month run-rate.
**Date started:** 2026-08-21
**Frameworks applied:** diagnose, mom-test, monetizing-innovation, traction, money-models, 100m-offers

---

## The strategy in one line

One free app for **solo técnicos de climatização** in Brazil, subscription sold outside the app stores at **R$139/mês via Pix (Asaas)** — reach **260 paying clients (~3 sales per working day at peak)** by month 6. (Target raised from the original 210, and price from R$129, so the goal survives partner commissions, contador fees, pró-labore taxes and the annual-plan discount — see the ramp.)

## Why not a classic paid app

At $4.99 one-time you need 1,100+ new sales every month forever. At R$139/mo you need ~250 humans total to say yes. Going from a $5 price to a $99+/yr price cuts the required audience ~20x — on a 6-month deadline, convincing 200 people is a hustle problem; convincing 1,500/month is a distribution-machine problem you don't have time to build.

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

- **R$139/mês** standard · **R$79/mês founder rate, lifetime, first 30 only** (pre-sale engine)
- **R$1.390/ano** from month 4 (~10% off; effective R$115,80/mês) — annual cash upfront is what funds ads within the 30-day payback rule (money-models). It is a cash-flow tool, not the default: the ramp models **~30% of standard clients on annual by M6** and values them at their effective monthly rate, not R$139.
- Billing via Asaas (Pix + cartão), app unlocks via backend, no purchase links in-app → no store commission, revenue in BRL, no FX/payout lag
- **Store-rules risk (iOS):** removing purchase links does *not* guarantee compliance — Apple's App Review Guidelines (3.1.1 / 3.1.3) can require in-app purchase for single-user subscriptions, and "web-only unlock" apps sometimes pass review and sometimes get rejected. The primary funnel here sells on the web *before* install (pre-sale + partners), which helps but is not a safe harbor. **Contingency:** if Apple blocks the iOS build, enable IAP on iOS at R$169/mês while keeping R$139 on web/Android. **Prerequisite: enroll in Apple's Small Business Program the day the developer account exists** — the 15% rate applies only after SBP approval; Apple's default is 30% in a subscriber's first year, under which even R$169 nets only R$118,30 and this contingency stops being cost-neutral. With SBP approved, at R$169 Apple's 15% cut (R$25,35) is fully covered by the R$30 uplift, so the contingency is roughly cost-neutral per subscriber; the real cost is conversion drag from the higher iOS price. If Apple instead forces price parity at R$139, the 15% cut ≈ R$2,2k/mo at month 6 — that scenario needs ~20 extra clients or a stronger annual push to keep the exit goal.
- Stack: Expo/React Native + Supabase + Asaas

## The ramp

| Month | Paying | Gross/mo | Partner commission | Cumulative gross |
|---|---:|---:|---:|---:|
| M1 | 10 founders | R$790 | — | R$790 |
| M2 | 40 | R$3.760 | — | R$4.550 |
| M3 | 80 | R$9.320 | — | R$13.870 |
| M4 | 130 | R$15.920 | −R$813 | R$29.790 |
| M5 | 195 | R$24.355 | −R$2.638 | R$54.145 |
| M6 | 260 | R$32.740 | −R$5.466 | R$86.885 |

Gross/mo values annual clients at their **effective monthly rate (R$115,80)**, with the annual share ramping 15% → 25% → 30% of standard clients over M4–M6 (the upfront annual cash improves cash flow but is not counted as R$139 recurring). Commission column assumes the partner channel goes live in M4 and partner-attributed clients grow to **60% of standard-rate clients by M6 (~140 actives)**, each paying the 30% rev-share (first 12 months). Net of Asaas ~2%, Simples ~7% (Anexo III via fator R), ~R$400/mo tools, **~R$500/mo contador with full escrituração (see plumbing)**, the **R$1,5k of M3 channel tests** and these commissions → business surplus ≈ **R$63,2k cumulative, ~R$23,4k/mo at M6**.

**What "líquido" means here: founder take-home, not accounting profit.** Fator R requires paying yourself pró-labore ≥28% of revenue (~R$9,2k/mo at M6). That is your own paycheck, not a lost cost — but it carries ~11% INSS plus IRPF (~R$2,3k/mo at M6), while profit distributions on top stay tax-exempt **only if the books prove the profit** (see plumbing). **Founder take-home ≈ R$21,1k/mo at M6** and **cumulative take-home ≈ R$58k ≈ US$10,7k** over the six months — a ~R$1k/mo cushion over the goal with every listed cost paid. At 8% monthly churn, month-6 needs ~80 gross sales to net +65 — ~3–4/working day at peak.

## Month by month

- **M1 wk 1 — validate, zero code.** Interview 15 of 25 sourced técnicos (Mom Test rules — last three jobs, how the orçamento went out, lost-track clients). **Gate: ≥8/15 say "eu sei que perco manutenção", else switch to empreiteiros de pequena obra.**
- **M1 wk 2 — pre-sell.** One-page site, founder pricing, Pix button. **Gate: 10 paid pre-sales before writing the second screen** — these are the 10 founders in the M1 row.
- **M1 wk 3–4 — ship v1.** Orçamento+PDF+WhatsApp only, nothing else; deliver to the 10 founders by the last day of M1. The clock starts on day 1 of M1 — there is no uncounted setup month, so the whole plan is six elapsed months.
- **M2 — retention before growth.** Ship reminders; churn >12%/mo = product problem, fix before traffic. Start channel tests. Target 40.
- **M3 — find the channel.** Bullseye: 3 channels × 2 weeks × R$500. **Gate: ≥5 paying from one channel; cumulative ≥R$13k or change ONE variable.** Target 80.
- **M4 — double down + annual.** First two rev-share partners. Target 130.
- **M5 — scale.** 3–5 partners, referral ("indique um colega, ganhe um mês"), ads only if payback <30 days. Target 195.
- **M6 — hold.** 260 clients, both goals met — commissions, contador and pró-labore taxes paid.

## Channels (bet order)

1. **Rev-share with refrigeração course sellers / técnico influencers** — 30% recurring × 12 months (deducted in the ramp math above). **3–4 partners × 30–40 conversions ≈ the ~140 partner-attributed actives the commission model assumes**; direct channels (pre-sale cohort, Reels, groups, referral) must supply the other half. If partners overdeliver, commissions scale with them (≈ +R$2,4k/mo at M6 if partner actives hit 200) — acceptable, since 70%-margin revenue beats none, but re-run the take-home math before raising spend.
2. Organic Reels/TikTok — the orçamento generated on a real job, PT-BR.
3. WhatsApp/Facebook groups of técnicos.

Pass bar per test: ≥5 paying clients in 2 weeks.

## Kill criteria (non-negotiable)

- End of M1 week 2 without 10 pre-pays → **switch niche, not features**.
- End of M3 below R$13k cumulative → change one variable (price, niche, or channel — never all three).
- End of M4 below R$11k/mo gross → deadline is gone; consciously extend to 9–12 months or add service income. Never drift.

## Plumbing (where líquido is won)

- Skip MEI (R$81k/yr ceiling breaks by M4). Open **ME no Simples Nacional** now. Let the contador pick the CNAE for licensed, non-customizable software / SaaS (likely 6203-1/00, not 6201-5/01, which is *sob encomenda* custom development) and confirm it is Simples-eligible and lands in Anexo III via fator R in your município.
- **Fator R:** pró-labore ≥28% of revenue → Anexo III ~6% vs Anexo V ~15.5%. The pró-labore is your own paycheck, but budget its INSS/IRPF — already deducted in the take-home math above. Even with those taxes, Anexo III + pró-labore beats Anexo V at these revenue levels; confirm with a contador who has SaaS clients.
- Pix via Asaas settles in days, in BRL. Stores are distribution only.
- **Full escrituração contábil from day 1**, not just the livro-caixa: Simples profit distributions above the presumed-profit floor (32% of receita for services) are tax-exempt only when complete accounting books demonstrate the higher real profit. That is why the contador must do full bookkeeping — budget ~R$500/mo for it, already deducted in the take-home math.
- Costs: Apple US$99/yr + Play US$25 + Supabase/EAS/domain ≈ R$400/mo; contador com escrituração completa ≈ R$500/mo; channel tests ≈ R$1.5k once.

## Interview script (M1 week 1)

1. Me conta seu último orçamento — como você mandou?
2. Quantos clientes de instalação você tem no total? Quantos voltaram pra limpeza?
3. Como você lembra quem tá vencendo?
4. Já perdeu serviço porque demorou a responder?
5. O que você usa hoje — papel, WhatsApp, planilha?

---

*Assumes FX ≈ R$5,40. Honest odds: ~1-in-3 for a full-time builder who pre-sells first; the gates exist to reveal early which third you're in.*
