# Quick Start Guide: Proposal & Project Templates

Welcome! This guide gets you up and running with your new EA knowledge base in 10 minutes.

---

## What You Have

You now have a complete system for capturing enterprise architecture work:

```
📁 knowledge/
├── 📄 personal_knowledge_base.okf          ← Main index (start here)
├── 📄 proposal_template.md                 ← Copy this for new proposals
├── 📄 project_template.md                  ← Copy this for new projects
├── 📄 ea_templates_usage_guide.md          ← How to use templates
├── 📄 introspection_and_learning_guide.md  ← How to learn from your work
├── 📄 QUICK_START.md                       ← This file
│
├── 📁 proposals/
│   └── 📁 2026-07_example_api_modernization/
│       └── 📄 proposal_api_modernization.okf  ← Example proposal (copy this structure)
│
└── 📁 projects/
    └── 📁 2026-07_example_api_modernization/
        └── 📄 project_api_modernization.okf   ← Example project (copy this structure)
```

---

## The Flow

```
1. Problem identified
   ↓
2. Write PROPOSAL (use proposal_template.md)
   ├─ Business context
   ├─ Solution design
   ├─ Risks & trade-offs
   └─ Learning & introspection (what I know, what I'm missing)
   ↓
3. Proposal approved
   ↓
4. Create PROJECT (use project_template.md)
   ├─ Planning
   ├─ Execution (with weekly status)
   ├─ Learning & introspection (weekly reflection)
   └─ Retrospective (at completion)
   ↓
5. Learn & grow (update your knowledge base)
   ↓
6. Next proposal is better (you've accumulated wisdom)
```

---

## 5-Minute Getting Started

### Step 1: Open the example files
- Open: `proposals/2026-07_example_api_modernization/proposal_api_modernization.okf`
- Open: `projects/2026-07_example_api_modernization/project_api_modernization.okf`
- See how a complete proposal and project look

### Step 2: Identify your first proposal or project
- What are you working on RIGHT NOW?
- Is it in the "thinking" stage (→ write a PROPOSAL)
- Or already approved/executing (→ write a PROJECT)

### Step 3: Create your first file
**To create your first PROPOSAL:**
```
1. Create folder: knowledge/proposals/YYYY-MM_[topic-name]/
   Example: knowledge/proposals/2026-08_security_audit/

2. Copy: proposal_template.md → proposal_[topic].okf
   Example: proposal_security_audit.okf

3. Edit the file with YOUR information (not the example)

4. Save and commit
```

**To create your first PROJECT:**
```
1. Create folder: knowledge/projects/YYYY-MM_[topic-name]/
   Example: knowledge/projects/2026-08_security_audit/

2. Copy: project_template.md → project_[topic].okf
   Example: project_security_audit.okf

3. Link to the related proposal (in the YAML frontmatter)

4. Edit and save
```

### Step 4: Share with your team
- Point people to the templates
- Show them the example
- Suggest they do the same for their initiatives

---

## Weekly Discipline (10 Minutes)

**Every Friday afternoon:**

1. **If you have an active project:** Fill in current status section
   - What shipped this week?
   - What's blocked?
   - What's the risk/metric update?
   - Go-to: `project_[topic].okf` → "Current Status (Update Weekly)"

2. **Fill introspection section (5 minutes)**
   - What went well and why?
   - What did I miss?
   - Where did I fail?
   - Go-to: `project_[topic].okf` → "Learning & Introspection"

3. **Update the main index (2 minutes)**
   - Go-to: `personal_knowledge_base.okf`
   - Update status of active projects
   - Move completed items to retrospective section

**Total time:** 10-15 minutes. Huge payoff for your learning.

---

## Monthly Discipline (1 Hour)

**Last Friday of month:**

1. **Review all active proposals & projects**
   - Are there patterns in what's working/not working?
   - What domain knowledge gaps are repeating?
   - What skill improvements do you need?

2. **Update the learnings section**
   - Go-to: `personal_knowledge_base.okf` → "Learning Archive"
   - Capture 3-5 key learnings from the month
   - What will you do differently next month?

3. **Identify skill gaps**
   - What's limiting you most?
   - What will you study next month?

---

## Section-by-Section Reference

### In PROPOSAL, the key sections are:

| Section | Why | When to fill |
|---------|-----|--------------|
| Executive Summary | Decision-makers need the 1-page version | Start (draft proposal) |
| Business Context | Prove the problem is real and worth solving | Start |
| Stakeholders | Get clear on who decides what | Start |
| Trade-off Analysis | Show you've considered alternatives | Start/Review |
| Risk & Mitigation | Every proposal has risks; naming them shows maturity | Start/Review |
| Learning & Introspection | Capture what you know/don't know BEFORE executing | Start/Review |
| Decision & Next Steps | Make the ask clear | Before presenting |
| Retrospective | What actually happened vs. what you planned | After decision/execution |

### In PROJECT, the key sections are:

| Section | Why | When to fill |
|---------|-----|--------------|
| Project Overview | Clear on what success looks like | Start |
| Team & Decisions | Clear on who decides what | Start |
| Phases & Execution | Your roadmap from start to finish | Start/Review |
| Current Status | Weekly update on progress | Every Friday |
| Learning & Introspection | Weekly reflection on what you're learning | Every Friday |
| Retrospective | What you learned, what you'll do differently | End of project |

---

## Templates Explained

### proposal_template.md
**What it is:** A comprehensive template for thinking through a new initiative before getting started.

**Use when:**
- You have an idea you need to propose
- You need to make a business case
- You want stakeholder buy-in
- You're evaluating "should we do this?"

**Length:** Typically 5-15 pages when filled out (more thinking, less filling)

**Key sections:** Executive summary, business context, stakeholder analysis, trade-offs, risks, learning/introspection

---

### project_template.md
**What it is:** A comprehensive template for executing a multi-week/month initiative with rigor.

**Use when:**
- A proposal has been approved
- Work is going to take multiple phases
- Multiple people are involved
- You need to track progress and learn from it

**Length:** Typically 10-20 pages when filled out (phases get detailed)

**Key sections:** Overview, phases with gates, team structure, weekly status, learning/introspection, retrospective

---

### ea_templates_usage_guide.md
**What it is:** Detailed guidance on how to use each section of the templates, with enterprise architect thinking.

**Read when:**
- You're filling out a template for the first time
- You're unsure what a section means
- You want to understand why each section exists

**Key content:** Section-by-section guidance, common mistakes, enterprise architect thinking questions

---

### introspection_and_learning_guide.md
**What it is:** A guide to capturing learning systematically (domain knowledge, blind spots, failures, skill gaps).

**Read when:**
- You want to understand the introspection sections better
- You're done with a proposal/project and want to extract maximum learning
- You want to build a pattern library of your own work

**Key content:** Why introspection matters, how to investigate blind spots/failures, cadence for reflection, building your knowledge base

---

## File Naming Convention

Stick to this naming convention so you can find things easily:

**Proposals:**
```
proposals/YYYY-MM_[topic-name]/proposal_[topic].okf
Example: proposals/2026-08_cloud_security/proposal_cloud_security.okf
```

**Projects:**
```
projects/YYYY-MM_[topic-name]/project_[topic].okf
Example: projects/2026-08_cloud_security/project_cloud_security.okf
```

**Why:**
- YYYY-MM: Chronological ordering (easy to see what you did when)
- topic-name: Self-documenting (clear what it's about)
- Folder organization: Keeps related files together
- Consistent naming: Makes searching easy

---

## Common Mistakes to Avoid

### ❌ Mistake 1: Not starting with business context
You write a proposal but lead with technology ("We need Kubernetes") instead of business impact ("We need to reduce deployment time from 4 hours to 30 minutes").

**Fix:** Always start with the business problem, add technology in details.

---

### ❌ Mistake 2: Skipping the introspection sections
You fill in all the planning sections but skip "Learning & Introspection" because it feels soft or less important.

**Fix:** Introspection sections ARE the value. They're where you learn and grow. Prioritize them.

---

### ❌ Mistake 3: Never reading what you wrote
You write a proposal, it gets approved, you execute, but you never look back at what you learned or what you got wrong.

**Fix:** Schedule monthly review time. Your past work is your best teacher.

---

### ❌ Mistake 4: Not updating status weekly
You start a project, but only update status at the end when you're writing the retrospective.

**Fix:** Friday 15-minute discipline. Real-time status = you catch problems early.

---

### ❌ Mistake 5: Making templates too detailed
You customize the templates so much that they become unwieldy and you don't use them.

**Fix:** Use templates as-is for 3-4 cycles. THEN customize based on what you've learned.

---

## Your Next Steps

### This week:
- [ ] Read the example proposal (10 min)
- [ ] Read the example project (10 min)
- [ ] Read `ea_templates_usage_guide.md` (20 min)
- [ ] Identify your first proposal or project to capture

### Next week:
- [ ] Create your first proposal OR project file
- [ ] Get feedback from your sponsor/lead
- [ ] Share with your team (so they can do the same)

### Next month:
- [ ] Do your first monthly review
- [ ] Identify patterns in what's working/not working
- [ ] Update your quarterly learnings

---

## FAQ

**Q: Do I have to fill every section?**
A: No. But fill every section ONCE to understand what matters. Then you can abbreviate what's less relevant for your work.

**Q: What if my proposal is small?**
A: Use the template anyway. Even small proposals benefit from stakeholder clarity and risk thinking. Smaller proposal = shorter document, same structure.

**Q: When do I do introspection—during the project or after?**
A: Both. Weekly during project (catch issues in real-time). Deep reflection at the end (extract patterns).

**Q: Can I share these templates with others?**
A: Yes! These are YOUR enterprise architecture practice. Sharing them with your team means everyone gets better.

**Q: How do I know if I'm using this right?**
A: You'll know after 3 proposals and 1 completed project. You should be able to:
1. See patterns in what works/doesn't
2. Point to places where introspection changed your approach
3. Have a searchable archive you reference

**Q: Should I combine proposal + project into one file?**
A: No. Keep them separate. Proposal is "should we do this?" Project is "how are we doing this?" They have different purposes.

---

## Support

### If you get stuck:
1. **Check the examples:** Look at `proposal_api_modernization.okf` and `project_api_modernization.okf`
2. **Read the guide:** Go to `ea_templates_usage_guide.md` for section-by-section guidance
3. **Review learnings guide:** `introspection_and_learning_guide.md` for deep dive on any section

### If you find a section confusing:
- Don't skip it
- Read the usage guide for that section
- Look at the example file to see how it was filled
- Ask yourself: "What would I need to know to fill this?" (That's your skill gap)

---

## You're All Set!

You now have:
- ✅ Example files showing how to use this
- ✅ Templates for proposals and projects
- ✅ Guides on how to use them effectively
- ✅ A system for capturing learning

**Start with one proposal or project THIS WEEK.** Don't overthink it. The templates are meant to be used, not perfected.

Your future self—the one who's become a recognized enterprise architect—will thank you for starting this now.

Good luck! 🚀
