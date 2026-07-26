# Knowledge Base Structure Reference

Visual guide to your enterprise architecture knowledge base setup.

---

## Directory Structure

```
📁 knowledge/
│
├─ 📄 personal_knowledge_base.okf
│  └─ Main index with all indices and quick links
│
├─ 📄 QUICK_START.md ⭐ START HERE
│  └─ 5-minute getting started guide
│
├─ 📄 STRUCTURE_REFERENCE.md (this file)
│  └─ Visual reference for the whole setup
│
├── TEMPLATES & GUIDES
│  ├─ 📄 proposal_template.md
│  │  └─ Copy this for each new proposal
│  ├─ 📄 project_template.md
│  │  └─ Copy this for each new project
│  ├─ 📄 ea_templates_usage_guide.md
│  │  └─ Section-by-section guidance
│  └─ 📄 introspection_and_learning_guide.md
│     └─ How to learn from your work
│
├── PROPOSALS (organized by date & topic)
│  ├─ 📁 2026-07_example_api_modernization/
│  │  └─ 📄 proposal_api_modernization.okf ⭐ EXAMPLE
│  │
│  ├─ 📁 2026-08_your_first_proposal/
│  │  └─ 📄 proposal_your_topic.okf
│  │
│  └─ 📁 [YYYY-MM_topic]/
│     └─ 📄 proposal_[topic].okf
│
├── PROJECTS (organized by date & topic)
│  ├─ 📁 2026-07_example_api_modernization/
│  │  └─ 📄 project_api_modernization.okf ⭐ EXAMPLE
│  │
│  ├─ 📁 2026-08_your_first_project/
│  │  └─ 📄 project_[topic].okf
│  │
│  └─ 📁 [YYYY-MM_topic]/
│     └─ 📄 project_[topic].okf
│
└── LEARNINGS (quarterly & annual summaries)
   ├─ 📄 Q3_2026_learnings.md
   ├─ 📄 Q4_2026_learnings.md
   └─ 📄 2026_annual_retrospective.md
```

---

## File Types Explained

### 📄 .okf files (Your core work)
- **What:** Individual proposals and projects
- **Format:** YAML frontmatter + Markdown content
- **Purpose:** Searchable, versionable record of each piece of work
- **How often:** One per proposal/project (dozens over your career)

### 📄 .md files (Guides & templates)
- **What:** Templates, guides, and documentation
- **Format:** Markdown with clear structure
- **Purpose:** Reference material to help you use the system
- **How often:** Reference as needed; create learnings summaries quarterly

---

## Proposal Lifecycle

```
1. DRAFT → Create proposal_[topic].okf
           Fill in business context, solution, analysis
           Fill in "Learning & Introspection" section
           ↓
2. REVIEW → Share with stakeholders
            Gather feedback
            Update based on input
            ↓
3. APPROVED → Change status to "approved"
              Create related project_[topic].okf
              Update personal_knowledge_base.okf index
              ↓
4. EXECUTION → Project starts
               Reference proposal for context
               ↓
5. RETROSPECTIVE → Fill retrospective section of proposal
                   Document what you learned
                   Archive for future reference
```

---

## Project Lifecycle

```
1. PLANNING → Create project_[topic].okf from template
              Link to approved proposal
              Fill phases, team, resources
              ↓
2. PHASE 1 → Execute Phase 1
             Weekly Friday: Fill "Current Status" section
             Weekly Friday: Fill "Learning & Introspection" 
             ↓
3. PHASE 2 → Continue pattern (weekly updates + introspection)
     ↓
4. PHASE 3 → Continue pattern
     ↓
5. PHASE 4 → Continue pattern
     ↓
6. COMPLETION → Fill "Retrospective" section
                Analyze what happened vs. planned
                Extract learnings
                Complete learning entry in personal_knowledge_base.okf
                ↓
7. ARCHIVE → Move to "Completed Projects" section
             Reference for future similar work
```

---

## Where Each Section Lives

### PROPOSAL FILE Structure

```
proposal_[topic].okf
│
├─ YAML Frontmatter (metadata)
│
├─ Executive Summary (decision-makers read this)
├─ Business Context (problem statement, stakeholders)
├─ Proposed Solution (what you're recommending)
├─ Trade-off Analysis (why this vs. alternatives)
├─ Risk & Mitigation (what could go wrong)
├─ Implementation Plan (phased approach)
├─ Resource Requirements (team, budget)
├─ Success Metrics (how you'll measure)
├─ Communication Plan (who knows what when)
│
├─ ⭐ Learning & Introspection ⭐ (domain knowledge, blind spots, gaps)
│
├─ Decision & Next Steps (what's being asked for)
└─ Retrospective (fill after execution)
```

### PROJECT FILE Structure

```
project_[topic].okf
│
├─ YAML Frontmatter (metadata + link to proposal)
│
├─ Project Overview (what, why, success criteria)
├─ Scope & Context (what's in/out)
├─ Team Structure (who decides what)
├─ Phases & Execution (roadmap with gates)
├─ Resources & Budget (team + money)
├─ Quality & Testing (standards, acceptance)
├─ Launch Strategy (how you go live)
│
├─ ⭐ Learning & Introspection ⭐ (domain knowledge, blind spots, failures, skill gaps)
│   ├─ Fill this WEEKLY (not just at end)
│   ├─ Weekly: What went well, what I missed, where I failed
│   └─ Weekly: What do I need to improve
│
├─ Current Status (update EVERY Friday)
│   ├─ Overall status (🟢/🟡/🔴)
│   ├─ This week accomplishments
│   ├─ What's blocked
│   └─ Metrics update
│
└─ Retrospective (fill at project end)
   ├─ What happened vs. planned
   ├─ What went well & why
   ├─ What you'd do differently
   ├─ Technical debt created
   └─ Knowledge gained
```

---

## The Heart of the System: Learning & Introspection

This is what makes this system different from generic project tracking.

### In Every Proposal:
```
Learning & Introspection Section
├─ Domain Knowledge Assessment
│  ├─ What domain expertise was required?
│  ├─ My baseline proficiency (Beginner → Expert)
│  ├─ Gaps I identified
│  ├─ How that impacted the proposal
│  └─ How I'm filling the gap
│
├─ What I Got Right
│  └─ (Don't be modest—name your good calls)
│
├─ What I Missed
│  ├─ Blind spots I didn't anticipate
│  ├─ Why I made wrong assumptions
│  └─ How to catch it next time
│
└─ Where I Need to Improve
   ├─ Technical skills gaps
   ├─ Soft skills gaps
   └─ Process/thinking gaps
```

### In Every Project:
```
Learning & Introspection Section (FILL WEEKLY + AT END)
├─ Domain Knowledge Needed
│  ├─ What expertise is required?
│  ├─ My proficiency in each domain
│  ├─ Gaps discovered during project
│  └─ How I'm filling gaps
│
├─ What Went Well & Why
│  └─ Successes + what enabled them
│
├─ What I Missed
│  ├─ Blind spots during execution
│  └─ How to catch next time
│
├─ Where I Failed or Made Mistakes
│  ├─ Honest assessment of what went wrong
│  ├─ Root cause & my role
│  ├─ Impact on stakeholders
│  └─ What I'll do differently
│
└─ Where I Need to Improve
   ├─ Technical skill gaps
   ├─ Soft skill gaps
   └─ Process/thinking gaps
```

---

## Weekly Discipline

Every Friday (10-15 minutes):

### If you have an active project:

1. **Update "Current Status" section**
   ```
   ├─ Overall status: 🟢/🟡/🔴
   ├─ Summary of the week
   ├─ What shipped
   ├─ What's blocked
   └─ Metrics update
   ```

2. **Update "Learning & Introspection" section**
   ```
   ├─ What went well this week & why
   ├─ What did I miss
   ├─ Where did I fail
   └─ Where do I need to improve
   ```

3. **Update main index**
   - Go to `personal_knowledge_base.okf`
   - Update project status
   - Note any changes

**Total time:** 10-15 minutes

---

## Monthly Discipline

End of month (1 hour):

1. **Review all active proposals & projects**
   - Read your weekly status updates
   - Look for patterns (what's repeating?)
   - What domain knowledge gaps keep showing up?
   - What skill gaps are limiting you?

2. **Update your Learning Archive**
   - Go to `personal_knowledge_base.okf` → "Learning Archive"
   - Capture 3-5 key learnings from the month
   - What will you focus on next month?

3. **Plan for next month**
   - What skill will you develop?
   - What will you study?

---

## Quarterly Discipline

End of quarter (2-3 hours):

1. **Deep review of all proposals/projects from quarter**
   - Read all retrospectives
   - Synthesize patterns across work
   - What are your biggest learnings?

2. **Write Quarterly Learning Summary**
   - Create: `Q[N]_[YEAR]_learnings.md`
   - Capture learnings, patterns, insights
   - What's your skill development for next quarter?

3. **Update main index**
   - Add link to quarterly summary
   - Move completed projects to "Completed" section
   - Review all proposals to see which became projects

---

## Annual Discipline

End of year (4-5 hours):

1. **Review entire year's work**
   - Read all proposals and projects
   - Read all learning summaries
   - How has your thinking evolved?

2. **Write Annual Retrospective**
   - Create: `[YEAR]_annual_retrospective.md`
   - Biggest learnings about domain, organization, yourself
   - How has your capability grown?
   - What will be your focus next year?

3. **Plan next year**
   - What major initiatives are you tackling?
   - What domains do you need to develop?
   - How will you measure your growth?

---

## Search & Reference Strategy

### Finding past work:

**"I faced this problem before, what did I decide?"**
```
→ Go to personal_knowledge_base.okf
→ Search "Proposals Index" for topic
→ Open the proposal file
→ Read "Proposed Solution" + "Trade-off Analysis"
→ Read "Retrospective" to see what actually happened
```

**"What did I learn about cloud architecture?"**
```
→ Go to personal_knowledge_base.okf
→ Find all proposals/projects related to cloud
→ Read "Learning & Introspection" in each
→ Extract patterns across multiple files
```

**"What organizational patterns have I discovered?"**
```
→ Go to personal_knowledge_base.okf
→ Read quarterly learning summaries
→ Search for "organizational" or "stakeholder" themes
→ Synthesize what you've learned
```

---

## File Naming Quick Reference

### Proposals
```
✅ proposals/2026-08_cloud_migration/proposal_cloud_migration.okf
✅ proposals/2026-09_data_warehouse/proposal_data_warehouse.okf
❌ proposals/proposal_1.okf (no date or topic)
❌ proposals/MyProposal.okf (not descriptive)
```

### Projects
```
✅ projects/2026-08_cloud_migration/project_cloud_migration.okf
✅ projects/2026-09_data_warehouse/project_data_warehouse.okf
❌ projects/project_1.okf (no date or topic)
❌ projects/MyProject.okf (not descriptive)
```

### Learning Summaries
```
✅ Q3_2026_learnings.md
✅ 2026_annual_retrospective.md
❌ Learnings.md (which quarter/year?)
❌ Annual.md (not specific)
```

---

## What NOT to Store Here

- ❌ Meeting notes (go in meeting notes, then reference here)
- ❌ Code/technical details (go in code repo, reference here)
- ❌ Ongoing status updates (those go in your project tracking tool)
- ❌ Day-to-day decisions (only major initiatives belong here)

**What TO store here:**
- ✅ Proposals (thinking stage)
- ✅ Projects (execution stage)
- ✅ Learning summaries (retrospectives & quarterly reviews)
- ✅ Decision history (why we chose this approach)
- ✅ Patterns & insights (what you learned)

---

## Quick Checklist: Is My Setup Right?

After you've created your first proposal or project, check:

- [ ] File is in `proposals/YYYY-MM_[topic]/` or `projects/YYYY-MM_[topic]/` folder
- [ ] File name is `proposal_[topic].okf` or `project_[topic].okf`
- [ ] YAML frontmatter has metadata (id, date, status)
- [ ] Proposal has "Learning & Introspection" section with content
- [ ] Project has "Learning & Introspection" AND "Current Status" sections
- [ ] I can find the file by browsing the folder structure
- [ ] I've added an entry to `personal_knowledge_base.okf` index
- [ ] I understand what each section means (read the guides if not)

If you check all these boxes, you're set up correctly!

---

## The Goal

After 1 year of using this system consistently:

✅ You have 10-15 completed proposals and projects documented  
✅ You can see patterns in what works and what doesn't  
✅ You can point to specific places where introspection changed your approach  
✅ You have a searchable archive you reference constantly  
✅ Your thinking has visibly improved  
✅ People ask YOU for advice because they see your depth of thinking  

**That's when you know it's working.**

---

**Start with the QUICK_START.md file. Read it this week. Create your first proposal or project next week.**

You've got this! 🚀
