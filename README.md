🪙 Jar — Swarna Sankalp

Goal-Based Savings & Adaptive Pacing Engine

Turn Jar's existing savings products into personalized, purpose-driven saving journeys.





Product Requirements Document · v1.0 · 6 September 2026

🎯 Executive Summary

Jar has already solved the problem of making gold saving accessible.

Swarna Sankalp focuses on the next problem:

Why should I save now?

How much should I save?

What should I do when my ability to save changes?

Swarna Sankalp is proposed as a personalization and intelligence layer over Jar's existing savings products — not as a separate savings instrument.

Core Proposition

Goal-based savings + adaptive contribution pacing + user-controlled redemption

Area

Definition

Primary users

Existing and prospective Jar savers with a personal, family, cultural, or financial goal

Primary value

Make saving purposeful, affordable, adaptive, and easier to sustain

Commercial value

Create higher-intent pathways into gold, physical gold, and jewellery

Evidence status

Public product/strategy alignment + product hypotheses; internal Jar capabilities require validation

💡 Product Thesis

Jar's existing ecosystem already supports flexible savings cadences such as daily, weekly, monthly and instant saving, alongside digital gold and physical/jewellery pathways.

The opportunity is therefore not to recreate saving. It is to make existing saving mechanisms:

More personalized → More goal-oriented → More sustainable

Three Product Layers

Layer

Role

🪔 Cultural occasions

Emotional differentiation

🧠 Adaptive pacing

Intelligence

🛍️ Redemption

Optional commerce

The product should deepen the user's relationship with Jar without turning goal completion into an aggressive sales funnel.

Positioning: Swarna Sankalp — Goal-Based Savings & Adaptive Pacing Engine for Jar.

🚨 Problem Statement

Users may understand the value of saving but still struggle with three questions:

Why should I save now? · How much should I save? · What happens when my ability to save changes?

Current Friction

Swarna Sankalp Response

Saving feels abstract or repetitive

Purpose-led goals tied to personal, family and cultural milestones

Users may not know a realistic contribution

Target + date translated into a required saving rate

Fixed contributions can become difficult

Adaptive contribution recommendation + optional pause/slowdown

Missing contributions feels like failure

Recovery through increase, date extension, or target reduction

One cadence may not fit everyone

Recommend daily / weekly / monthly / instant

Users may not know what to do after completion

User-controlled redemption or continuation options

🏗️ Product Architecture

┌───────────────────────────────────────────────┐
│              1. MOTIVATION                    │
│       What am I saving for?                    │
│       Goal templates + custom goals            │
└───────────────────────┬───────────────────────┘
                        ↓
┌───────────────────────────────────────────────┐
│              2. PLANNING                      │
│       How much do I need?                      │
│       Target + date + saving rate              │
└───────────────────────┬───────────────────────┘
                        ↓
┌───────────────────────────────────────────────┐
│           3. RECOMMENDATION                   │
│       How much should I save?                   │
│       Contribution + cadence                   │
└───────────────────────┬───────────────────────┘
                        ↓
┌───────────────────────────────────────────────┐
│           4. ADAPTIVE PACING                  │
│       Can I afford that today?                  │
│       Context-aware contribution               │
└───────────────────────┬───────────────────────┘
                        ↓
┌───────────────────────────────────────────────┐
│             5. RECOVERY                       │
│       I fell behind — what now?                │
│       Increase / extend / reduce               │
└───────────────────────┬───────────────────────┘
                        ↓
┌───────────────────────────────────────────────┐
│              6. PROGRESS                      │
│       Am I on track?                           │
│       Progress + projection + nudges           │
└───────────────────────┬───────────────────────┘
                        ↓
┌───────────────────────────────────────────────┐
│             7. REDEMPTION                     │
│       What can I do when I reach it?           │
│       Continue / digital gold / physical gold  │
│       / jewellery / gifting                    │
└───────────────────────────────────────────────┘

👤 Personas & Use Cases

Persona

Example Goal

Likely Need

🪔 Purpose-driven saver

Maa ke Liye Gold

Emotional motivation + simple plan

🎁 Festival planner

Rakhi / Dhanteras

Deadline-based plan + gifting intent

💍 Milestone saver

Wedding / education

Longer horizon + flexible cadence

🔄 Habit saver

Emergency gold reserve

Sustainable recurring contributions

📈 Irregular-income saver

Personal gold goal

Weekly/instant cadence + adaptive pacing

🛣️ End-to-End User Journey

Discover Swarna Sankalp from the home feed, savings area, goal prompt, or cultural moment.

Select a suggested goal or create a custom goal.

Set target amount and target date.

Choose or accept a recommended savings cadence.

Understand the required contribution and why it was recommended.

Start saving using an existing Jar savings mechanism.

Adapt as behavior/context changes.

Recover if behind schedule instead of receiving a generic failure message.

Track progress with projected completion and lightweight nudges.

Complete the goal and choose whether to continue or explore relevant redemption options.

⚙️ Functional Requirements

8.1 Goal Creation

Provide culturally relevant templates such as:

Maa ke Liye Gold

Rakhi

Dhanteras

Wedding

Family milestone

Emergency gold

Custom goal

Users can define:

Custom goal name

Target amount

Target date

Optional description

Optional recipient / purpose

Users can also edit the target amount and target date after creation.

8.2 Savings Cadence Recommendation

Support:

Daily · Weekly · Monthly · Instant

Recommendation should consider:

Saving frequency

Consistency

Goal horizon

User-declared context

The user can always override the recommendation.

🧠 8.3 Adaptive Contribution Engine

Core Logic

Target + Deadline
       ↓
Required Saving Rate
       ↓
Behavior / Context Signals
       ↓
Recommended Contribution

Example System Responses

Scenario

System Response

Normal capacity

“₹100 today keeps you on track.”

Lower recent capacity

“₹40 today is enough; we’ll adjust the next contribution.”

Missed contribution

“You’re ₹200 behind. Spread the recovery over 5 days?”

Goal becomes unrealistic

“Would you prefer to extend the date or reduce the target?”

Stable monthly pattern

“Switch to ₹1,500 monthly?”

💰 8.4 Savings Affordability Signal

Replace “Liquidity Stress” with “Savings Affordability Signal.”

The signal should describe confidence in a recommendation, not diagnose the user's financial condition.

Data Maturity

Version

Inputs

V1

Jar savings history, missed contributions, recent contribution size, cadence consistency, goal behavior

V2

User-declared income cycle and savings flexibility

V3

Consented external financial data where legally and technically appropriate

Every recommendation should be explainable in plain language.

🔄 8.5 Goal Recovery Engine

Recovery Option

When to Show

Outcome

Increase contribution

User can plausibly save more

Reach original target/date

Extend date

Required rate is too high

Preserve target with lower pressure

Reduce target

Goal is no longer realistic

Preserve momentum with smaller goal

Pause / slow down

User explicitly needs flexibility

Protect trust and long-term habit

🔀 8.6 Plan Switch

Offer cadence changes when behavior suggests a better fit.

“Daily saving seems difficult this month. Switch from ₹100/day to ₹700/week?”

“You usually have more capacity after payday. Move your monthly saving date?”

Never switch a plan without user confirmation.

📊 8.7 Progress & Nudges

Show:

Current progress

Target amount

Target date

Projected completion

Nudges should:

Use positive reinforcement rather than guilt

Trigger around missed contributions

Surface upcoming deadlines

Recognize meaningful cultural moments

Allow reduced notification frequency or opt-out

🛍️ 8.8 Redemption & Commerce

At high completion or goal completion, surface relevant options without forcing a purchase.

Potential choices:

Continue saving

Digital gold

Physical gold / coin

Jewellery

Gifting

Another supported action

Redemption should reflect goal intent where appropriate.

⚠️ Do not hard-code an 85% completion trigger. Validate optimal timing experimentally.

🤖 Data & ML Requirements

Data Maturity Roadmap

Version

Data Source

Purpose

V1

Jar-native behavior

Personalize plan and pacing without external data

V2

User-declared context

Improve affordability-aware recommendations

V3

Consented external data

More precise cash-flow-aware recommendations

Recommendation Inputs

Target amount and remaining target

Remaining days and required saving rate

Historical contribution amount and frequency

Recent missed-contribution pattern

Goal completion trajectory

Cadence preference and plan-switch history

User-declared flexibility / income cycle

Model / Rules Approach

MVP should begin with deterministic rules and transparent scoring before introducing a complex ML model.

Candidate objective:

Predict a sustainable contribution level that maximizes goal adherence without materially increasing missed contributions.

Evaluate:

Calibration · Stability · Fairness · Recommendation acceptance · Downstream goal progress

🛡️ Trust, Safety & Compliance

Swarna Sankalp should:

❌ Never encourage borrowing to meet a savings target

❌ Never present a recommendation as financial advice or guarantee

🔐 Obtain appropriate consent before external financial data use

🎛️ Give users control over target, date, cadence, contribution and redemption

🚫 Avoid manipulative urgency or guilt-based nudges

🏷️ Distinguish product facts from estimates, projections and hypotheses

⚖️ Validate regulatory, privacy, data-retention and consent requirements before launch

📈 Analytics & Event Tracking

Event

Key Properties

Why It Matters

goal_created

goal_type, target, date

Activation

plan_recommended

cadence, amount

Recommendation exposure

plan_accepted

cadence, amount

Recommendation acceptance

contribution_made

amount, cadence, goal_id

Actual saving

contribution_missed

expected_amount, days_late

Adherence / recovery

plan_switched

from, to, reason

Cadence personalization

recovery_started

option

Recovery behavior

goal_completed

duration, amount

Outcome

redemption_viewed

option

Commerce intent

redemption_completed

option, value

Commerce conversion

📐 KPI Framework

⭐ North Star Metric

Successful Goal Progress Rate

Percentage of active goal users who remain on track toward their intended goal.

Metric

Definition

Purpose

Goal activation rate

Goal creators / eligible users

Initial adoption

Saving adherence

Actual contribution / recommended contribution

Plan fit

D30 / D60 / D90 retention

Goals active at interval

Sustained engagement

Goal completion rate

Completed / started goals

End outcome

Incremental savings

Treatment savings − control savings

Causal product impact

Savings Sustainability Score

Consistency + misses + recovery + withdrawals

Sustainable behavior

Redemption conversion

Completed redemption / eligible goal users

Optional commerce outcome

🧪 Experimentation Framework

Test:

Goal-led onboarding vs. generic savings entry

Adaptive contribution recommendations vs. static recommendations

Daily / weekly / monthly cadence recommendation logic

Recovery options — increase vs. extend date vs. reduce target

Redemption timing and presentation

Primary Causal Metric

Incremental savings, rather than relying only on engagement or completion.

📌 Business Impact Hypotheses

Hypothesis 1

Purpose-driven goals increase activation and sustained saving behavior.

Hypothesis 2

Adaptive pacing reduces missed contributions and improves goal retention.

Hypothesis 3

Better goal completion creates higher-intent opportunities for physical gold and jewellery exploration.

Hypothesis 4

Personalized cadence increases contribution sustainability versus a one-size-fits-all cadence.

⚠️ Exact completion rates, gold spreads, physical-gold margins and revenue uplift must not be presented as established facts unless supported by Jar's internal data or primary evidence.

🚀 MVP Roadmap

Phase

Scope

Success Criteria

V1 — Goal Layer

Goal creation, templates, target/date, cadence recommendation, progress, basic rules-based pacing

Activation + adherence improve vs. control

V2 — Adaptive & Recovery

Savings Affordability Signal, plan switch, recovery engine, user-declared context

Lower missed contributions + higher successful progress

V3 — Intelligent & Commerce

Advanced modeling, consented external context, personalized redemption

Incremental savings + validated commerce lift without trust degradation

⚠️ Risks & Mitigations

Risk

Impact

Mitigation

External data unavailable

Adaptive model lacks broader cash-flow context

Start with Jar-native data

Over-optimization for commerce

Trust erosion

Keep redemption user-controlled

Recommendations feel intrusive

Lower adoption

Explain inputs + offer override

Users over-save temporarily

Poor sustainability

Optimize for adherence, not maximum daily amount

Cultural goals become gimmicky

Low long-term value

Keep culture as motivation; intelligence as core

Unsupported performance claims

Credibility risk

Label hypotheses + run controlled experiments

Loan/savings interaction

Financial trust / regulatory risk

Never recommend borrowing

🔍 Assumptions & Open Questions

Assumptions to Validate

Jar can expose sufficient savings behavior data for V1.

Existing savings products can be represented under a common goal abstraction.

Users will understand and accept adaptive contribution recommendations.

Goal-based journeys can integrate into the current home/feed experience.

Open Questions

Does Jar already have an internal goal engine?

Which savings products can currently attach to a goal?

What user-level transaction/savings data is available?

Does Jar support consented financial-data integration?

What are current digital-gold, physical-gold and jewellery conversion funnels?

Which redemption surfaces are already available?

What regulatory/compliance constraints apply?

Which segments have the highest retention and contribution sustainability?

🏁 Final Product Direction

Don't build another savings product.

Build an intelligence layer that helps people save sustainably for things that matter.

The strongest product story is:

Goals + Behavioral Intelligence + Adaptive Pacing

Cultural goals provide the motivation layer.

Adaptive pacing and recovery provide the core product innovation.

Physical gold and jewellery provide an optional, user-controlled commerce layer.

🧩 Example Goal Scenarios

Scenario

Goal

Recommendation

Adaptive Behavior

🎂 Maa's birthday

₹7,500 by Oct 15

₹82/day

Reduce today's amount if capacity falls and recalculate

🎁 Rakhi gifting

₹3,000 by Aug 18

₹100/week or ₹15/day

Switch cadence based on preference

🛟 Emergency gold

₹20,000 over 6 months

Monthly plan

Prioritize sustainability over aggressive catch-up

🔄 Missed contributions

₹10,000 target

Recovery plan

Spread deficit across remaining periods

🏆 Goal completed

₹7,500 reached

Redemption choices

Continue saving, digital gold, physical gold/coin, jewellery/gifting where supported

🪙 Swarna Sankalp

A goal isn't just a number. It's something worth saving for.

Jar — Swarna Sankalp · Product Requirements Document · v1.0 · Discussion-ready working PRD
