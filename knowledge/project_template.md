---
type: Project
id: project_YYYY_MM_DD_xx
domain: Projects
title: [Project name - clear, business-focused]
date: YYYY-MM-DD
status: planning|in-progress|at-risk|blocked|completed|archived
updated: YYYY-MM-DD
related_proposal: [proposal_id if this came from a proposal]
---

# Project Overview

## Project Summary
- **Objective:** What business problem/opportunity does this solve? (1-2 sentences)
- **Strategic alignment:** How this connects to organizational goals/roadmap
- **Success criteria:** How you'll know this project was successful
- **Project lead:** Name, contact, escalation point
- **Sponsor/Executive owner:** Who is ultimately accountable

## Key Dates
| Milestone | Planned | Actual | Status |
|-----------|---------|--------|--------|
| Kickoff | YYYY-MM-DD | | |
| Phase 1 complete | | | |
| Phase 2 complete | | | |
| Go-live/Launch | | | |
| Closure | | | |

---

# Scope & Context

## What's In Scope
- **Deliverables:** What gets built/delivered/changed
- **Systems/teams affected:** What systems touch, what teams are impacted
- **Constraints:** What you must work within (budget, time, technical)

## What's Out of Scope
- Explicitly list what this project does NOT include (important for managing expectations)

## Assumptions
- [Assumption 1 - state what you're assuming is true]
- [Assumption 2]
- [Assumption 3]

---

# Team Structure & Accountability

## Core Team
| Role | Name | Organization | % Allocation | Key Responsibilities |
|------|------|--------------|--------------|---------------------|
| Project Lead | | | | Delivery, timeline, escalations |
| Technical Lead | | | | Architecture, technical decisions, quality |
| Product Owner | | | | Requirements, acceptance, business alignment |
| [Other lead] | | | | |

## Extended Team
- **Engineering:** [Count and skills needed]
- **QA/Testing:** [Count and approach]
- **Operations/Support:** [When they engage]
- **Business/Domain experts:** [Who provides subject matter expertise]

## Decision Rights
- **Project-level decisions (scope, timeline, budget):** [Who decides]
- **Technical decisions:** [Who decides, escalation path]
- **Business/requirements decisions:** [Who decides]
- **Risk escalation threshold:** [When to escalate to sponsor]

---

# Project Phases & Execution Plan

## Phase 1: [Phase Name - e.g., Planning & Design]
**Duration:** YYYY-MM-DD to YYYY-MM-DD (X weeks)

### Work Streams
- **Work stream 1:** [Description]
  - Deliverables: [List specific outputs]
  - Owner: [Person/team]
  - Dependencies: [What must be ready]
  - Success criteria: [How you know it's done]

- **Work stream 2:** [...]

### Phase Gate
- **Gate criteria:** [What must be true to move to next phase]
- **Gate approver:** [Who approves moving forward]
- **Target gate date:** YYYY-MM-DD

---

## Phase 2: [Phase Name - e.g., Build & Test]
[Same structure as Phase 1]

---

## Phase 3: [Phase Name - e.g., Launch & Stabilize]
[Same structure as Phase 1]

---

# Resources & Budget

## Resource Plan
- **Total team size:** X FTEs (or X% of Y people)
- **Ramp-up/ramp-down:** When people join/leave
- **Key person dependencies:** People whose absence blocks progress
- **Contingency headcount:** Buffer for unexpected work

## Budget Breakdown
| Category | Amount | Owner | Notes |
|----------|--------|-------|-------|
| Personnel | $X | | X weeks @ Y rate |
| Infrastructure/Tools | $X | | Licenses, services, compute |
| Vendor/External | $X | | Contractors, consulting |
| Contingency (10-15%) | $X | | |
| **Total** | **$X** | | |

## Budget Tracking
- **Monthly burn rate:** $X
- **Forecast to complete:** $X
- **Variance threshold (trigger review):** ±10%

---

# Architecture & Technical Approach

## High-Level Design
- **Core architecture pattern:** [Approach you're using]
- **Technology stack:** [Key technologies/platforms]
- **Scalability targets:** [Performance/scale requirements]
- **Security/compliance requirements:** [What must be met]

## Key Technical Decisions
| Decision | Chosen Approach | Alternative | Why Chosen | Risk |
|----------|-----------------|-------------|-----------|------|
| [Decision] | [Choice] | [Other options] | [Rationale] | [Any risks] |

## Integration Points
- **Existing systems:** [What systems this integrates with]
- **Data flows:** [How data moves]
- **API contracts:** [Who consumes, what contract]
- **Backward compatibility:** [Must support existing clients/versions?]

## Technical Debt & Risks
- **Known technical debt:** [What's being compromised]
- **Mitigation plan:** [How to pay down later]
- **Risk if not addressed:** [Impact if ignored]

---

# Risks & Issues

## Risk Register
| Risk | Likelihood | Impact | Mitigation | Owner | Target Date | Status |
|------|-----------|--------|-----------|-------|-------------|--------|
| [Risk] | H/M/L | H/M/L | [Action] | [Name] | [Date] | Open/Mitigated |

**Risk scoring:** High impact = project jeopardized; Medium = significant delay/rework; Low = manageable

## Current Issues
| Issue | Severity | Root Cause | Resolution | Owner | Target Date | Status |
|-------|----------|-----------|-----------|-------|-------------|--------|
| [Issue] | H/M/L | [Why it happened] | [Fix] | [Name] | [Date] | Open/Resolved |

## Dependency Risk
- **External dependencies:** [What this depends on outside project]
- **Mitigation:** [How you're managing dependency risk]
- **Escalation:** [Who to contact if dependency at risk]

---

# Quality, Testing & Acceptance

## Quality Standards
- **Code quality:** [Standards, tools, thresholds]
- **Test coverage:** [Target % coverage by type]
- **Performance benchmarks:** [Latency, throughput targets]
- **Security scanning:** [Tools and findings threshold]

## Testing Strategy
- **Unit tests:** [Coverage target, tools]
- **Integration tests:** [Key flows tested]
- **UAT:** [Business acceptance criteria, participants, timeline]
- **Performance testing:** [Load, stress test scenarios]
- **Security testing:** [Any specialized testing needed]

## Acceptance Criteria
- **User acceptance:** [What business users must verify]
- **Operational acceptance:** [What ops team must verify]
- **Performance acceptance:** [What performance targets must be met]
- **Rollback criteria:** [When you'd rollback launch]

---

# Launch & Go-Live Strategy

## Go-Live Approach
- **Strategy:** [Big bang, phased, pilot, canary, etc.]
- **Timeline:** [Exact go-live window]
- **Participants:** [Who's involved in launch]
- **Rollback plan:** [How to undo if things go wrong]
- **Rollback decision authority:** [Who calls rollback]

## Launch Readiness Checklist
- [ ] Code complete and tested
- [ ] Documentation complete
- [ ] Team trained
- [ ] Operations runbooks ready
- [ ] Monitoring/alerting configured
- [ ] Support team briefed
- [ ] Customer communication ready
- [ ] Rollback plan tested

## Support During Launch
- **War room setup:** [Where team gathers during launch]
- **Communication channels:** [How to share status/issues]
- **On-call schedule:** [Who's on-call first 24-72 hours]
- **Escalation path:** [How issues get escalated]

---

# Communication & Stakeholder Management

## Stakeholder Map
| Stakeholder Group | Key Concerns | Update Frequency | Channel | Owner |
|------------------|--------------|-----------------|---------|-------|
| Executive sponsor | Timeline, ROI | Monthly | Email + meeting | [Lead] |
| End users | Feature delivery, ease of use | Weekly | Team meetings | [Owner] |
| IT/Operations | Operational impact | Weekly | Tech sync | [Tech lead] |
| Other teams | Dependencies, impact | As-needed | Standups/email | [Lead] |

## Communication Plan
- **Project kickoff:** Date, audience, message
- **Regular status updates:** Weekly/bi-weekly standup format
- **Milestone announcements:** When/how to communicate wins
- **Launch announcement:** Pre-launch, launch day, post-launch messaging
- **Change management:** How to handle last-minute changes

## Escalation Path
- **Level 1:** Project lead handles and resolves
- **Level 2:** Sponsor involved if decision needed
- **Level 3:** Executive steering committee (if major impact)

---

# Success Metrics & Benefits Realization

## Primary Success Metrics
1. **Metric:** [What you measure]
   - **Baseline:** [Current state]
   - **Target:** [Goal after project]
   - **Measurement method:** [How often, by whom]
   - **Owner:** [Who tracks this]
   - **Timeline:** [When you measure]

2. **Metric:** [...]

3. **Metric:** [...]

## Business Benefits
- **Financial:** [ROI, cost savings, revenue]
- **Operational:** [Efficiency, speed, reliability]
- **Strategic:** [Competitive advantage, capability, scalability]
- **Cultural:** [Skills, tools, processes improved]

## Benefits Realization Plan
- **Who tracks benefits:** [Owner accountable for measurement]
- **When:** [30-60-90 days post-launch, then quarterly]
- **Variance tolerance:** [If benefit is X% short, what do we do?]
- **Adjustment mechanism:** [How to course-correct if benefits not realized]

---

# Current Status (Update Weekly)

## Status Summary
**Overall status:** 🟢 Green | 🟡 Yellow | 🔴 Red

**Summary line:** [1-2 sentence status - are you on track?]

**Key metrics this week:**
- Timeline variance: [Planned vs. actual progress]
- Budget variance: [Spent vs. budget to date]
- Risk/issue count: [# open issues, escalations]

## What Happened This Week
- **Completed:** [Deliverables, milestones finished]
- **In progress:** [What's active now]
- **Blocked/at-risk:** [What's stuck or at risk]

## Next Week's Focus
- **Top 3 priorities:** [What you're focused on]
- **Dependencies to monitor:** [What might slip]
- **Risks to watch:** [What could go wrong]

---

# Learning & Introspection (Capture Throughout Project)

## Domain Knowledge Needed for This Project
**What expertise did you need to deliver this project well?**

### Domain 1: [Architecture/Technical Domain]
- **Required knowledge:** [What you needed to know]
- **Your baseline:** Beginner | Intermediate | Advanced | Expert
- **Gap discovered:** [What you didn't know well enough]
- **How it impacted delivery:** [Did lack of knowledge cause delays, mistakes, or workarounds?]
- **How you filled the gap:** [Who did you learn from? What resources did you use?]
- **Proficiency now:** [Current level after project]

### Domain 2: [Business/Product Domain]
- [Same structure]

### Domain 3: [Organizational/Process Domain]
- [Same structure]

**Reflection:** Did you have the right domain expertise on the team? Who was your domain expert? Could you have done better with different expertise?

---

## What Went Well & Why
- **Success 1:** [What you executed well]
  - Why it worked: [What did you do right?]
  - Who enabled this: [Who helped? What support did you get?]
  - How to repeat: [Specific practice/approach to use again]

- **Success 2:** [...]

- **Success 3:** [...]

---

## What You Missed
- **Blind spot 1:** [Something you didn't anticipate or plan for]
  - Why you missed it: [What assumption were you making?]
  - When it surfaced: [When did you realize?]
  - How you adapted: [What did you do when you discovered it?]
  - How to catch next time: [Process change, checklist item, or question to ask]

- **Blind spot 2:** [...]

---

## Where You Failed or Made Mistakes
- **Failure 1:** [Something that went wrong]
  - What happened: [Specific situation]
  - Root cause: [Why did it happen? Your mistake, team dynamics, external factor?]
  - Impact: [Who was affected? What was delayed/wrong?]
  - Your accountability: [What was your role in this?]
  - What you learned: [How will you think/act differently?]
  - Will you do it differently next time? [Yes/No/Maybe, and why]

- **Failure 2:** [...]

- **Failure 3:** [...]

---

## Where You Need to Improve
**Skills gaps that became evident:**

### Technical Skills
- **Gap:** [Specific technical skill or knowledge area]
  - Situation where it showed up: [Example from project]
  - Impact: [What happened because of this gap?]
  - Proficiency needed: Beginner → Intermediate → Advanced (pick target)
  - Learning plan: [How you'll get better]
  - Timeline: [By when will you close this gap?]
  - Success measure: [How you'll know you've improved]

### Soft Skills
- **Gap:** [Communication, leadership, influence, delegation, etc.]
  - Situation: [Specific instance]
  - Impact: [What went wrong?]
  - Improvement approach: [What will you do differently?]
  - Practice opportunity: [Next project where you can practice this]

### Process/Thinking Skills
- **Gap:** [How you approach planning, risk management, communication, etc.]
  - What was missing: [Analysis? Checks? Questions you should have asked?]
  - Better process: [New checklist item, template change, decision framework]
  - When to use it: [In what situations will this matter?]

---

## Stakeholder & Team Feedback

### What the Business Said
- **Sponsor feedback:** [Were they happy? Surprised? Disappointed?]
- **End users:** [Did they get what they needed? What surprised them?]
- **Key stakeholders:** [How did each react to outcomes?]

### What Your Team Said
- **Team morale:** [Did team feel good about this project? Why or why not?]
- **What they'd do differently:** [Did team members surface improvements?]
- **Psychological safety:** [Could team safely say "this isn't working"?]

### What You Learned About Yourself
- **Strengths demonstrated:** [What did this project show about your strengths?]
- **Growth areas:** [What gaps in your capability became visible?]
- **Leadership approach:** [Was your style effective? What would you change?]

---

## Decision Points Where You Could Have Gone Differently

**Key moments where you made a choice:**

| Decision Point | Choice You Made | Alternative You Considered | Why You Chose What You Did | Would You Choose Differently Now? | Why/Why Not |
|---|---|---|---|---|---|
| [Situation] | [Your choice] | [Other options] | [Reasoning at the time] | Yes/No | [Reflection] |

---

## Knowledge Gained — What Will You Carry Forward?

### About This Technical Domain
- **Key insight:** [What did you learn about this technology/approach?]
- **Applies to:** [Other situations where this knowledge matters]
- **Share with:** [Who else should know this?]

### About This Business/Industry
- **Key insight:** [Pattern you noticed, constraint you discovered]
- **Why it matters:** [Impact on future work]

### About This Organization
- **Key insight:** [How things actually get decided, who has influence, what matters]
- **Applies to:** [Future proposals, projects, interactions]

### About Yourself as a Leader/Architect
- **Key insight:** [How you work, what you're good at, where you get stuck]

---

# Retrospective & Learnings (Complete after project closure)

## Execution Assessment
| Dimension | Planned | Actual | Variance | Commentary |
|-----------|---------|--------|----------|-----------|
| **Timeline** | X weeks | | | |
| **Budget** | $X | | | |
| **Scope** | [Items] | | | Changed? Added? |
| **Quality** | [Standards] | | | Met? |
| **Adoption** | [Target %] | | | |

## What Went Well
- [Success 1 - what enabled it?]
- [Success 2]
- [Success 3]

## What We'd Do Differently
- [Improvement 1 - why matters, how to apply next time]
- [Improvement 2]

## Technical Debt Created
- [Debt item 1]
- [Debt item 2]
- [Timeline to address]

## Knowledge Transfer
- **Documentation:** [What was created for future teams]
- **Training:** [What skills were built]
- **Process improvements:** [What changed about how we work]

## Legacy & Follow-up Work
- **Follow-on projects:** [Work enabled by this]
- **Standing issues:** [What still needs attention]
- **Budget holdback:** [Any reserved budget for fixes/tuning]

---

# Appendices

## A. Detailed Technical Architecture
[Diagrams, schema, API specs]

## B. Project Plan (Gantt/Timeline)
[Detailed schedule with dependencies]

## C. Detailed Budget Breakdown
[Month-by-month forecast, cost center codes]

## D. Risk Assessments
[Security review, compliance check, capacity risk]

## E. Reference Documents
- Links to relevant proposals, business cases, prior projects
- Regulatory/compliance documents
- Market research or competitive analysis

---

**Last Updated:** [Date]
**Next Status Update:** [Date]
**Project Health:** 🟢 On track | 🟡 Minor concerns | 🔴 Major issues
