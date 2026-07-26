---
id: ea_templates_usage_guide
domain: Proposals and Projects
title: Enterprise Architect Template Usage Guide
date: 2026-07-26
---

# Using Proposal & Project Templates for Enterprise Architecture

This guide explains how to effectively use the Proposal and Project templates to build your enterprise architecture practice.

---

## Why These Templates Matter for Enterprise Architects

### Enterprise Architect's Role
As an enterprise architect, you're responsible for:
- **Strategic alignment:** Ensuring technical work serves business goals
- **Holistic thinking:** Seeing across systems, teams, and timelines
- **Risk management:** Identifying and mitigating technical and organizational risks
- **Governance:** Ensuring standards, compliance, and quality
- **Stakeholder communication:** Translating between technical and business worlds

### How Templates Enable This
These templates force you to think like an EA from the beginning:
1. **Business-first thinking** — Every proposal starts with business impact, not technology
2. **Stakeholder management** — Explicit identification of who decides, who is affected, who resists
3. **Risk thinking** — Systematic identification and mitigation of threats
4. **Strategic alignment** — Connecting work to organizational goals
5. **Measurable outcomes** — Defining success clearly before starting

---

## When to Use Each Template

### Use the PROPOSAL Template When:
- ✅ Proposing a new initiative (technology, process, organizational change)
- ✅ Evaluating "how should we approach this?" questions
- ✅ Seeking approval/budget/prioritization for work
- ✅ Making a case for a significant decision
- ✅ Documenting trade-offs between approaches
- ✅ Getting stakeholder buy-in on an idea

**Not for:** Status updates, small bug fixes, routine operational changes

### Use the PROJECT Template When:
- ✅ Executing a multi-week/multi-month initiative
- ✅ Work requiring cross-functional coordination
- ✅ Anything with dependencies, risks, or multiple phases
- ✅ Building something that others will use/operate
- ✅ Work where budget, timeline, or scope is significant
- ✅ Tracking progress and outcomes for retrospective

**Not for:** One-off tasks, simple operations, minor maintenance

### Relationship Between Them:
```
PROPOSAL → Approved? → becomes a PROJECT → Completed? → Retrospective fed back to proposals
```

---

## Section-by-Section Usage Guide

### PROPOSAL Template

#### Executive Summary
**Why it matters:** Decision-makers rarely read the full proposal. This section is your entire argument in 1 page.

**How to write it:**
- Start with the business problem in plain English (no jargon)
- State your solution in one sentence
- Quantify the impact (30% cost reduction, 2 weeks faster, reduce risk by X%)
- Be honest about what it costs and how long it takes

**Common mistake:** Leading with technology ("We need Kubernetes") instead of business value ("We can reduce infrastructure costs by 30%").

---

#### Business Context / Problem Statement
**Why it matters:** You must prove this problem is real and worth solving.

**How to fill it:**
- **What:** Be specific. "Slow reporting" is too vague. "Weekly report takes 6 hours; we need it in 30 minutes" is specific.
- **Why it matters:** Connect to business consequences. "This delays decision-making by 5 days, costing ~$X in delayed actions."
- **Current state:** Show data. Show pain. Show that people care.

**Enterprise Architect question to ask yourself:** "Does this align with organizational strategy? Does the executive sponsor care about this problem?"

---

#### Stakeholders & Influencers
**Why it matters:** Your proposal's success depends on getting the right people in the room and understanding what they care about.

**How to fill it:**
- **Decision-maker:** Find THE person who can say yes. Not the committee, not the sponsor's report. The actual decision-maker.
- **Resistors:** Honest self-assessment. Who will push back? Why? How will you address their concern?
- **Allies:** Who benefits most? Who should you loop in early?

**Enterprise Architect question:** "Have I talked to all the stakeholders? Do I understand their real concerns (not just stated ones)?"

---

#### Proposed Solution / Architecture Overview
**Why it matters:** This is where you demonstrate architectural thinking.

**How to fill it:**
- Don't overwhelm with details. 3-4 sentences should explain what you're doing.
- Explain HOW it works, not just WHAT you're building.
- Call out integration points (where does this touch other systems?).
- State your design principles explicitly. They explain your trade-offs.

**Enterprise Architect depth:**
- This is where you show you understand the existing architecture
- Explain how this integrates into the tech landscape
- Call out where this changes/improves the architecture

---

#### Trade-off Analysis
**Why it matters:** You've always got options. Showing you considered them (and why you chose) builds credibility.

**How to fill it:**
- Generate 2-3 realistic alternatives (don't strawman)
- Compare apples-to-apples on dimensions that matter
- Be honest about trade-offs (if your solution is cheaper, it might be slower or require more skills)
- Explain why you chose what you chose

**Enterprise Architect question:** "Would I still recommend this if budget increased by 50%? If timeline doubled? If we could hire specialists? This question reveals whether you're recommending based on real constraints or just defaults."

---

#### Risk & Mitigation
**Why it matters:** Every proposal has risks. Pretending yours doesn't makes you look inexperienced.

**How to fill it:**
- Think through: Technical risks (will this tech work at our scale?), organizational risks (do we have the skills?), business risks (will users adopt it?), schedule risks (are timelines realistic?)
- For each risk, name a real mitigation. "Hope we don't hit this" isn't a mitigation.
- Assign someone accountable for watching each risk.

**Enterprise Architect thinking:** "What could derail this? What assumptions could be wrong? What would break this?"

---

#### Implementation Plan
**Why it matters:** This is where you go from vision to execution. Vague plans fail.

**How to fill it:**
- Break into phases that make sense (typically 3-5)
- Each phase has a clear gate ("we know we can move forward because...")
- Name the owner for each phase (not "engineering" — a specific person)
- Each phase has success criteria (how do you know it's done?)

**Enterprise Architect level:** Phase gates are your leverage. They're decision points where you can adapt, adjust, or stop if things aren't going right.

---

#### Resource Requirements & Budget
**Why it matters:** Good ideas fail when under-resourced. Showing you've thought through what's actually needed builds confidence.

**How to fill it:**
- Be realistic about headcount and skills needed
- Break budget into meaningful categories (infrastructure, labor, vendor, contingency)
- Show you understand what % of each person's time this needs
- Include contingency (typically 10-15%)

**Enterprise Architect thinking:** "Do we have these resources available? If not, what do we deprioritize? What's the opportunity cost?"

---

#### Success Metrics & Measurement
**Why it matters:** You can't improve what you don't measure. Clear metrics at the start prevent arguments about success later.

**How to fill it:**
- Define success before you start (not after)
- Metrics should be business metrics, not activity metrics
- Specify measurement method (not just "we'll measure it") — who measures, how often, by what tool
- Include both leading indicators (is this on track?) and lagging indicators (did we actually achieve the goal?)

**Common mistake:** "We'll measure adoption" without saying HOW (login counts? Feature usage? User surveys?).

---

#### Decision & Next Steps
**Why it matters:** Proposals end with someone making a decision. Make the ask clear.

**How to fill it:**
- Your recommendation should be one clear sentence
- Lay out the decision options (Approved, Approved with conditions, Rejected, Deferred)
- If approved, immediately name next steps so momentum doesn't stall
- If rejected, make clear what feedback you'll incorporate

**Enterprise Architect level:** After rejection, update your knowledge base with "Why was this rejected? What would it take to make it approvable next time?" This is how you learn.

---

### PROJECT Template

#### Project Overview
**Why it matters:** Clarity on what success looks like, who's in charge, and what the stakes are.

**How to fill it:**
- Objective: One sentence that answers "Why are we doing this?" not "What are we building?"
- Success criteria: 2-3 concrete things that must be true when done
- Project lead: If unclear who's accountable, the project will have unclear accountability everywhere
- Strategic alignment: Connect to organizational strategy (see if it connects to the Proposals that approved this)

**Enterprise Architect question:** "If this project's budget tripled, would we still do it? If it took 2x longer, would we still do it? If both? This tells you if this is a 'must do' or just 'nice to do'."

---

#### Scope & Context
**Why it matters:** Projects fail because scope creeps. Defining what's in/out prevents that.

**How to fill it:**
- **In scope:** Specific deliverables and systems touched
- **Out of scope:** Explicitly list things people might expect but that aren't included
- **Assumptions:** Name what you're assuming is true. If an assumption breaks, stop and replan.

**Enterprise Architect thinking:** Each "out of scope" item should have a reason. Not because you don't want to do it, but because:
- It's someone else's responsibility
- It would require different skills/time
- It's future work
- It's lower priority than what's in scope

---

#### Team Structure & Decision Rights
**Why it matters:** Ambiguous accountability creates chaos.

**How to fill it:**
- Core team roles and names (not placeholders)
- Each role with % allocation (so people know expectations)
- Decision rights spelled out: Who decides what types of decisions?
  - Technical decisions? Product owner? Tech lead? Consensus?
  - Scope changes? Project lead? Sponsor?
  - Risk escalation? When do you loop in sponsor?

**Enterprise Architect level:** Clarity here prevents a LOT of conflict mid-project. When everyone knows who decides what, decisions get made faster.

---

#### Project Phases & Execution Plan
**Why it matters:** This is your roadmap. It shows how you're going from start to finish.

**How to fill it:**
- Break into 3-5 phases that make sense for your project
- Each phase has work streams (parallel work within the phase)
- Each work stream has deliverables and success criteria
- Phase gates define when you're ready to move to the next phase

**Enterprise Architect depth:** This is where you show how you're de-risking. Early phases typically focus on proving assumptions. Later phases assume those assumptions are confirmed.

Example structure:
- **Phase 1: Planning & Design** — Understand requirements, validate approach, design solution (goal: confirm we're building the right thing)
- **Phase 2: Build & Test** — Build, test, integrate (goal: prove we can build it)
- **Phase 3: Launch & Stabilize** — Launch to production, monitor, fix issues (goal: prove it works in production)

---

#### Quality, Testing & Acceptance
**Why it matters:** Defining quality upfront prevents disputes about whether the project succeeded.

**How to fill it:**
- Quality standards: Specific metrics or thresholds (not just "high quality")
  - Example: "Test coverage ≥80%", "Page load time ≤2s", "Zero critical security findings"
- Testing strategy: What gets tested, how, by whom
- Acceptance criteria: What must be true for business to accept (not just engineering)
- Rollback criteria: When would you decide to rollback launch

**Enterprise Architect thinking:** This is where you codify non-functional requirements (performance, security, scalability, reliability). These are often overlooked but are critical to EA work.

---

#### Launch & Go-Live Strategy
**Why it matters:** How you launch determines whether your project succeeds or fails.

**How to fill it:**
- Strategy: Big bang (flip the switch all at once), phased (department by department), pilot (test with one group first), canary (small % of users)
- Each approach has trade-offs:
  - Big bang: Quick, clear, but highest risk if something breaks
  - Phased: Lower risk per phase, but longer overall and more complex
  - Pilot/canary: Lowest risk, but requires more operational sophistication
- Rollback plan: How to undo the launch if things go wrong (and when you'd trigger it)

**Enterprise Architect decision:** The launch strategy should be chosen based on risk tolerance and your ability to operate the system in parallel states.

---

#### Current Status (Weekly Update)
**Why it matters:** This is your weekly standup written down. It keeps everyone aligned.

**How to fill it:**
- Overall status: 🟢 Green (on track) | 🟡 Yellow (minor concerns) | 🔴 Red (major issues)
- Variance: Are you on schedule? On budget?
- This week: What shipped? What's active? What's blocked?
- Next week: Top 3 priorities
- Risks to monitor: What could go wrong?

**Discipline:** Update this every Friday. It takes 15 minutes. It prevents surprises.

---

#### Retrospective (After Completion)
**Why it matters:** The goal is to learn so you do the next project better.

**How to fill it:**
- Honest assessment: What did you plan vs. what actually happened?
- What went well: Name it so you can repeat it
- What you'd do differently: Be honest about what didn't work
- Technical debt created: Did you take shortcuts? Name them and commit to paying down
- Follow-on work: What did this enable? What still needs to happen?

**Enterprise Architect growth:** This is where you build wisdom. Read past retrospectives when planning new projects.

---

## Enterprise Architect Usage Pattern

### The Cycle
1. **Quarter starts:** You see problems/opportunities. You write PROPOSALS.
2. **Proposals reviewed/approved:** Approved ones become PROJECTS.
3. **Projects execute:** Weekly status updates, phase gates, decision-making.
4. **Project completes:** Retrospective captures learnings.
5. **Retrospective informs:** Next quarter's proposals build on what you learned.

### This is How You Build EA Credibility
- **Proposals show:** Strategic thinking, business acumen, holistic view
- **Projects show:** Execution discipline, risk management, team leadership
- **Retrospectives show:** Learning, humility, commitment to continuous improvement

---

## Common Mistakes to Avoid

### Mistake 1: Making Proposals Too Technical
❌ "We need to migrate to a microservices architecture using Kubernetes."
✅ "We need to reduce deployment time from 4 hours to 30 minutes so we can respond to customer issues faster. This reduces customer churn and support costs by ~$X."

**Fix:** Start with business impact. Add technical details in appendices.

---

### Mistake 2: Understating Risks
❌ "No significant risks." (Nobody believes this.)
✅ "Key risks: (1) We've never used this tech stack at scale, (2) We don't have hiring pipeline for the new skills, (3) Current architecture may not support this performance."

**Fix:** Show you've thought hard about failure modes. Shows maturity.

---

### Mistake 3: Vague Success Metrics
❌ "We'll measure adoption."
✅ "We'll measure adoption via: (1) Feature usage (min. X uses/month by month 3), (2) User satisfaction (NPS ≥40 by month 2), (3) Team efficiency (X% faster deployments by month 1)."

**Fix:** Define measurement method upfront. Make it specific.

---

### Mistake 4: Not Getting Stakeholder Buy-In Early
❌ Write proposal in a vacuum, present fully formed.
✅ Get key stakeholders' input at the proposal stage. Update based on feedback. Then present.

**Fix:** The best proposal is one informed by people who have to live with the consequences.

---

### Mistake 5: Project Status Updates Without Context
❌ "Week 5: X% complete. Backend 60%, frontend 40%, testing 30%."
✅ "Week 5: Completed Phase 1 gate criteria. Backend 60% (on track), frontend 40% (2 days behind due to API changes), testing 30% (will catch up in Phase 2). Risk: API changes added ~1 week. Mitigation: Added resources to frontend."

**Fix:** Show variance AND mitigation. Show you're managing, not just reporting.

---

## How to Apply These to Enterprise Architecture Growth

### Month 1-2: Get Comfortable with the Templates
- Write 2-3 proposals, even for small ideas. Get feedback.
- Use the project template for current work. Adjust as needed.
- Build muscle memory around structured thinking.

### Month 3-4: Deepen Strategic Alignment
- Link proposals back to organizational strategy and roadmap
- Start showing how proposals build on each other
- Use retrospectives to find patterns in what works/doesn't

### Month 5-6: Improve Risk & Trade-off Analysis
- Spend more time on trade-off analysis
- Make it a habit to list out 3 alternatives
- Build credibility by showing you've considered different approaches

### Month 6-12: Lead with Enterprise Thinking
- Use proposals to show holistic thinking (across systems, teams, time)
- Use projects to show execution rigor
- Use retrospectives to demonstrate learning and adaptation

### Year 2+: Build an Organizational Asset
- Your proposal archive becomes a resource: "How did we approach this before?"
- Your project retrospectives become a knowledge base
- You're now the person others ask: "How should we approach this?"

---

## Quick Start Checklist

**This week:**
- [ ] Read through both templates
- [ ] Identify one current or upcoming proposal to capture
- [ ] Identify one project to track
- [ ] Customize templates for your organization (adjust terminology, add/remove sections)
- [ ] Share templates with your team

**Next week:**
- [ ] Write your first proposal using the template
- [ ] Get feedback from sponsor/key stakeholder
- [ ] Update based on feedback

**Following weeks:**
- [ ] Execute your first project tracked in the template
- [ ] Update project status weekly
- [ ] Complete retrospective when done

---

**Remember:** These templates are tools for thinking, not just forms to fill out. The discipline of filling them out (clearly, honestly, thoroughly) is where the value lives.
