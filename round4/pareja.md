# Round 4 Reflection: Final Project Decision

**Name**: Omar Pareja
**PennKey**: Pareja
**Date**: 2025-11-04

---

## 1. What I Explored Today

_List the projects you seriously considered. Keep it brief._

| Project Name | Source | Key Takeaway (1 sentence) |
|--------------|--------|---------------------------|
| Urban Explorer (events map)  | Round 2/3 (current)  | Technically doable, but cold-start + two-sided marketplace makes it infeasible in 5 weeks without heavy seeding. |
| PriceScope (grocery prices) | R2 Drop (Amber He) | Clear crowd task, real value, easy to pilot with tiny scope (5 items, 1 store) and manual verification. |
| SoundScape (ambient audio map)  | R2 Drop (Mingni/Anika)| Creative and engaging but technically heavy (audio + maps) unless radically simplified. |

_Add more rows if needed_

**Resources I used**:
- [X] Rubric scoring (RUBRIC-PROJECT-VIABILITY.md)
- [X] V2 detailed analyses (reports/v2-analyses/)
- [X] Steelman Analysis pathways (STEELMAN-ANALYSIS.md)
- [X] Group discussions
- [ ] Other: [specify]

---

## 2. My Decision

**Project Name**: PriceScope — Crowdsourced local grocery prices

**Decision type**:
- [ ] STAYING with Round 3 project (same approach)
- [ ] STAYING with Round 3 project (modified approach/scope)
- [X] PIVOTING to different project
- [ ] JOINING another team's project

**If pivoting or adopting someone's idea**:
- Original author (if applicable): Amber He (heamber)
- Original round: R2

---

## 3. Why This Decision

**High-level reasoning** (2-3 paragraphs):

_Explain your thought process. What made you choose this project? What were the key factors? What trade-offs did you consider?_

Urban Explorer scored 16/30 in the V2 analysis—mainly limited by cold-start and two-sided dynamics. Even with Penn-only focus, we would need to proactively seed ~100+ events and secure multiple partner clubs just to make the map useful. That is possible, but the execution risk is high for a 5-week course, and most of the grade would hinge on recruitment rather than demonstrating a clean crowdsourcing loop.

PriceScope, by contrast, has a very clear, verifiable micro-task: submit a price + photo for a specific staple item. It provides immediate utility (cheaper eggs/milk/chicken near me), and we can run a credible MVP with one neighborhood, five staple items, and one or two stores. Quality control can be handled manually at first (photo check + timestamp + location) before automating OCR/geofence. The smaller scope still exercises core course ideas: task design, QC, aggregation, and recruitment tests.

The trade-off is that PriceScope lacks the “flashiness” of a map of events or sounds. But it’s measurably useful, easier to recruit for (everyone shops), and much more robust to a small pilot. It’s the highest probability of working with real users within 5 weeks.

**What convinced me**:
- Simple, high-signal crowd task that’s easy to explain and complete.
- MVP can be shipped in days using forms + manual verification.
- Clear success metrics (coverage on 5 items, verified entries/week).

**What concerns me** (and how I'll address it):
- Item normalization (sizes/brands) → Start with fixed SKUs and fixed sizes for 5 staples; standardize to unit price later.
- Spam/incorrect photos → Require photo + store selection + timestamp; manual review + rate limiting; flag/reject flow.

---

## 4. What I'm Building

**One-sentence project description**:
A lightweight, crowdsourced price checker that shows the cheapest nearby option for five staple grocery items based on verified shopper submissions.

**MVP Scope** (3-4 core features only):

1. **Submit Price (with photo)**: Simple form to submit item, size, store, and a receipt/shelf-tag photo.
2. **Verify & Aggregate**: Manual photo check; store a verified entry; compute most recent verified price per store.
3. **Search & Compare**: A tiny results page listing the lowest verified price nearby for each staple item.
4. **Reputation Lite**: Track contributor counts and show a simple “Trusted” badge after N verified submissions.
**What I'm explicitly NOT building** (to keep scope realistic):
- Full OCR pipeline (manual verification only for MVP).
- City-wide coverage (campus-adjacent neighborhood only).
- Complex gamification or full leaderboards (badge only after Week 2).

---

## 5. Week 1 Validation

**The specific test I'll run Week 1**:

_Be concrete. Not "social media" but "Post in r/UPenn and 3 class Slacks on Monday at 10am"_

- **Where**: Penn student group chats (CIS/NETS GroupMes), r/UPenn, 2 class Slacks, and 2 campus food Discords; in-person ask at Fresh Grocer & Trader Joe’s near campus.
- **When**: Monday–Wednesday (Nov 10–12) 10:00–14:00 for in-store; posts go live Monday 10:00 and Wednesday 18:00.
- **What**: “Help Penn find the cheapest eggs/milk/bread/chicken/rice this week — snap a shelf-tag or receipt and submit this 20-second form.”
- **Success metric**: ≥ 60 verified submissions (≥12 per item) from ≥ 25 unique contributors within 72 hours; coverage from 2 stores minimum.

**If Week 1 test fails, I will**:
- [X] Pivot to: [alternative approach]
- [X] Use MTurk/paid participants
- [ ] Try different recruitment channel: [specify]
- [ ] Simplify the task to: [easier version]
- [ ] Other: [specify]

---

## 6. **Tentative** Team (Optional, Only If You Already Have An Idea)

At this stage, you are not expected to have formed teams, however if you already have an idea of who you intend to work with, you may indicate it here.

**Team members**:

1. Omar (pareja) - PM / data design / recruitment
2. [Name] ([PennKey]) - [Primary role]
3. [Name] ([PennKey]) - [Primary role] _(optional)_
4. [Name] ([PennKey]) - [Primary role] _(optional)_

**Team status**:
- [ ] Same team from Round 3
- [ ] New team formed during Round 4
- [X] Solo (will find teammates later)
- [ ] Joining an existing team

---

## 7. Reflection

**Most valuable part of Round 4**:
Using the rubric to translate “cool idea” into execution risk and to force a scope that guarantees real users

**Biggest surprise**:
How much two-sided marketplaces collapse without a seeding plan; simple single-sided tasks win in 5 weeks.

**One thing I'd tell future students about Round 4**:
Pick the idea that makes it easiest to run a Week 1 test—not the one that sounds most impressive.

---

## Commitment

**I commit to**:
- [X] Building the MVP scope above (3-4 features maximum)
- [X] Running a concrete Week 1 validation test
- [X] Pivoting if Week 1 shows <20% success
- [X] Meeting with instructor if I hit major blockers

**Signature**: _________Omar________________ **Date**: ______Nov 8_______

---

## Submission

1. Save as `round4/[your-pennkey].md`
2. Submit via pull request
3. Deadline: [Instructor will specify]
