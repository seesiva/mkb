---
type: Guide
id: learning_documentation_template
domain: Learning & Development
title: Learning Documentation Template - Videos, Books, Papers & Podcasts
date: 2026-07-27
description: A structured template for capturing learnings, key insights, and reflection from educational sources (YouTube videos, books, research papers, podcasts, courses, etc.)
version: 1.0
---

# Learning Documentation Template

A structured approach to capture actionable learnings from any educational source. This template helps you extract knowledge, identify patterns, and create permanent reference material for future application.

---

## Quick Reference: When to Use This Template

**Use this template for EXTERNAL learnings:**
- ✅ YouTube videos, documentaries, TED talks
- ✅ Books, research papers, whitepapers
- ✅ Podcasts, interviews, webinars
- ✅ Online courses, workshops, certifications
- ✅ Talks, conferences, presentations
- ✅ Articles, essays, blog posts

**Use this template for OFFICE CONTEXT learnings:**
- ✅ Important client meetings or visits
- ✅ Key team meetings where important decisions/insights emerged
- ✅ Important emails (from leadership, customers, partners)
- ✅ One-on-one conversations with mentors, leaders, or colleagues
- ✅ Feedback conversations (performance reviews, retros, feedback sessions)
- ✅ Customer conversations or support interactions
- ✅ Sales/pitch meetings where you learned something important
- ✅ Cross-functional standups where key pattern emerged
- ✅ Incident postmortems or retrospectives

**Not this template:**
- ❌ Proposals (use [proposal_template.md](proposal_template.md))
- ❌ Ongoing projects (use [project_template.md](project_template.md))
- ❌ Daily meeting minutes/standup notes (too granular—capture these separately, then create a Learning doc if something important emerges)
- ❌ Quick reference material (create a dedicated index instead)

**Key Distinction:**
- **Use this:** "This meeting revealed something I didn't know about how the business works"
- **Don't use this:** "We talked about the Q3 roadmap" (that's just a status update)
- **Use this:** "Client conversation showed us a use-case we hadn't anticipated"
- **Don't use this:** "Had a standup with the team" (that's just coordination)

---

# Learning Document Template

## YAML Frontmatter

```yaml
---
type: Learning
id: learning_YYYY_MM_DD_##_[topic-slug]
domain: Learning & Development
title: [Source Title/Context + Your Focus Area]
source_type: video|book|paper|podcast|article|course|talk|meeting|client-visit|email|conversation|other
source_context: external|office-context
source_title: [Exact title of source OR brief description of context]
source_author: [Author/Creator/Speaker OR person(s) involved]
source_url: [URL if available, or "Not available online", or "Internal email thread"]
date_consumed: YYYY-MM-DD
date_documented: YYYY-MM-DD
created_at: YYYY-MM-DDTHH:MM:SSZ
tags:
  - [primary-topic]
  - [subtopic]
  - [domain]
source_duration: [HH:MM:SS for video/podcast, "~200 pages" for books, "1 hour meeting", etc.]
source_date: [Publication/Release date if known, or date of meeting/conversation]
relevance: [Why this matters to you - 1 sentence]
status: in-progress|completed|reviewed|archived
---
```

### Frontmatter Field Explanations

| Field | Format | Example | Purpose |
|-------|--------|---------|---------|
| **type** | String | `Learning` | Identifies as a learning document |
| **id** | `learning_YYYY_MM_DD_##_topic` | `learning_2026_07_27_01_systems_thinking` | Unique identifier; chronologically sortable |
| **source_context** | `external` or `office-context` | `office-context` | Distinguishes external learning from workplace incidents |
| **source_type** | One of the listed types | `video`, `book`, `meeting`, `client-visit`, `conversation` | Helps filter by medium |
| **source_title** | String | `The Three-Body Problem` OR `Q3 Budget Planning Meeting` | Exact title or brief description |
| **source_author** | String | `Liu Cixin` OR `John (VP Sales), Sarah (Product)` | Creator attribution or people involved |
| **source_url** | URL or text | `https://youtube.com/...` OR `Email thread: budget-q3` | Where to find the source again |
| **date_consumed** | YYYY-MM-DD | `2026-07-20` | When you experienced this content/event |
| **date_documented** | YYYY-MM-DD | `2026-07-27` | When you wrote this learning doc |
| **source_duration** | String | `47:23`, `~350 pages`, `1 hour meeting`, `15-min conversation` | Length/scope of source |
| **source_date** | String | `2021-03` OR `2026-07-25` | When published/released OR when it happened |
| **relevance** | 1 sentence | `How budget constraints force architecture choices` | Why you documented this |
| **status** | One value | `in-progress` → `completed` | Processing state of your notes |

---

## Document Structure

### 1. Source Context

Provide quick reference info about what you consumed.

```markdown
## Source Context

**Title:** [Exact source title]

**Creator/Author:** [Name(s)]

**Format:** [Video/Book/Podcast/etc.]
- **Length:** [Duration or page count]
- **Date Published:** [When it came out]
- **URL:** [Link to watch/read/listen again]

**Why I Chose This:**
[1-2 sentences explaining why you picked this source or why it was recommended]

**My Focus Area:**
[What specific angle or question were you exploring when you consumed this?]
- Example: "How do founders think about hiring in the first 50 people?"
- Example: "What are the failure modes in distributed systems?"
```

---

### 2. Quick Summary (2-3 minutes to read)

A compressed version of the source's core thesis or argument.

```markdown
## Quick Summary

**Core Thesis:**
[1-2 sentence version of the main idea]

**Main Argument:**
- Point 1: [What's the first big claim?]
- Point 2: [What's the supporting argument?]
- Point 3: [How do they conclude?]

**Who This Is For:**
[Who benefits from this content? Product managers? Engineers? Founders?]

**Type of Content:**
[ ] Narrative/Story-driven
[ ] Educational/Instructional  
[ ] Opinion/Perspective
[ ] Research/Evidence-based
[ ] Practical/How-to
[ ] Inspirational
```

---

### 3. Key Learnings & Insights

The most valuable section—capture specific, actionable knowledge.

```markdown
## Key Learnings

### Learning 1: [Title/Concept]
**What I learned:**
[Describe the specific insight or principle]

**Why it matters:**
[How does this change your thinking or behavior?]

**How I'll apply it:**
[Concrete next step: test, remember, share, change, etc.]

**Confidence level:** High | Medium | Low
[Are you sure about this, or was it presented speculatively?]

---

### Learning 2: [Title/Concept]
[Repeat structure...]

---

### Learning 3: [Title/Concept]
[Repeat structure...]
```

**Guidance:**
- Aim for 3-7 learnings per source (quality > quantity)
- For each learning, ask: "How is this different from what I knew?"
- Frame learnings as actionable, not just information
- Include the confidence level—signals which ideas to test vs. trust

---

### 4. Key Points to Remember

Memorable statements, quotes, frameworks, or rules-of-thumb from the source.

```markdown
## Key Points to Remember

### Framework 1: [Name]
[Explain a useful mental model or decision-making framework]
```
Example:
```
### Framework: The "3 Whys" Problem Diagnosis
Ask "why" three times in succession:
1. Why did X fail? → Immediate cause
2. Why did that cause exist? → Underlying cause  
3. Why do we tolerate that? → Systemic cause

Use: When you want to stop fixing symptoms and address root issues.
```

### Quote 1
> "[Exact quote from source]"
> — [Author], [Source], [Timestamp if applicable]

**Why this stuck:**
[Why is this quote meaningful? What does it capture that a summary wouldn't?]

---

### Quote 2
[Repeat structure...]

---

### Data Point / Statistic
**Claim:** [What is the factual claim?]
- **Data:** [The supporting number: "X% of Y achieved Z"]
- **Source:** [Where did they get this number?]
- **Confidence:** High | Medium | Low
[Did they cite their source? Is it peer-reviewed? This matters for how much you trust it.]

---

### Rule of Thumb / Heuristic
**Name:** [Short name for the heuristic]

**The Rule:**
[State the heuristic in plain language]

**When to use it:**
[What situations call for this rule?]

**When NOT to use it:**
[What are the edge cases or exceptions?]

Example:
```
**Name:** The "10x Rule" for Distribution
**The Rule:** For every 1 unit of work you put into building a product, you need 10 units into distribution/marketing to reach comparable success.
**When to use:** Planning go-to-market for a B2C product
**When NOT:** B2B enterprise sales (direct sales + partnerships can be more efficient)
```
```

---

### 5. Points to Ponder

Questions, tensions, or ideas that don't have clear answers yet. These are great for deep thinking and future exploration.

```markdown
## Points to Ponder

### Tension 1: [Title]
**The question:**
[State a tension or unresolved question from the source, or something the source raised for you]

**Why it matters:**
[Why is this worth thinking about?]

**What I currently think:**
[Your current view]

**What I need to learn:**
[What would help you resolve this?]

**Possible next steps:**
- Read: [What source might help?]
- Talk to: [Who has expertise here?]
- Experiment: [What could you test?]

---

### Tension 2: [Title]
[Repeat structure...]

---

### Question for Reflection
[An open question that challenges an assumption you held. Don't answer it yet—just state it clearly.]

Example:
- "If network effects are so powerful, why do most platforms fail in their first 2 years?"
- "The speaker assumes users are rational. But if they're not, does this entire framework break?"
```

**Guidance:**
- Tensions and questions show intellectual honesty—where your thinking is incomplete
- Don't feel pressure to resolve these; capturing them is valuable
- Revisit these later when you've read more or had more experience

---

### 6. Disagree / Critique

Space for healthy skepticism. What assumptions or claims do you question?

```markdown
## Where I Disagree / Critique

### Disagreement 1
**Claim from source:**
[What did they say?]

**Why I disagree:**
[What's your pushback?]

**Evidence against:**
[What makes you doubt this?]

**Could I be wrong?**
[How confident are you in your disagreement?]

---

### Blind Spot I Noticed
**What they missed:**
[What didn't the source address?]

**Why it might matter:**
[How could this limitation affect their conclusion?]

---

### Assumption Worth Questioning
**Unstated assumption:**
[What did they assume but not say explicitly?]

**Is it valid?**
[When is this true? When might it break?]
```

**Guidance:**
- Disagreement shows critical thinking, not disrespect
- The goal is to triangulate truth from multiple perspectives
- If you can't articulate why you disagree, that's valuable—means you need to think more

---

### 7. Connections to Existing Knowledge

Link this learning to other ideas, sources, or projects you know about.

```markdown
## Connections to Existing Knowledge

### Related Learning Document
See: [learning_2026_07_15_01_game_theory_basics.md](learning_2026_07_15_01_game_theory_basics.md)
**Connection:** This source applies game theory concepts to product strategy.

---

### Relates to Project
See: [project_2026_07_01_01_marketplace_design.md](project_2026_07_01_01_marketplace_design.md)
**How:** The network effects framework here challenges our current approach.

---

### Similar Concept in Different Domain
**From:** [Author/Source]
**Connection:** [How is this related or different?]

---

### Contradicts Earlier Learning
**From:** [Previous source]
**Difference:** [Earlier learning said X, this says Y. Which is true? Context-dependent?]
```

---

### 8. Immediate Actions & Follow-up

What will you do in the next 7 days based on this learning?

```markdown
## Immediate Actions

### Action 1: [What will you do?]
- **Timeline:** [By when? (e.g., this week, by 2026-07-30)]
- **Why:** [Which learning is driving this?]
- **Success criteria:** [How will you know you did it?]

Example:
```
### Action 1: Reread the distributed systems chapter
- **Timeline:** By 2026-07-31
- **Why:** Learning 3 about consensus algorithms confused me; need to build intuition
- **Success criteria:** I can explain Raft vs. Paxos without looking it up
```

```markdown
### Action 2: [Teach this to someone]
- **Who:** [Name or role]
- **Why:** [Teaching is the best way to solidify learning]
- **Format:** [Conversation? Presentation? Written summary?]

---

### Action 3: [Experiment / Test]
- **Hypothesis:** [What are you testing?]
- **Timeline:** [When will you try this?]
- **Success metric:** [How will you measure?]

---

### Action 4: [Read / Research Next]
- **What:** [What's the natural next thing to explore?]
- **Why:** [Why does this make sense given what you just learned?]
```

---

### 9. Reflection (Fill After 1-2 Weeks)

Come back after you've had time to process. Did this learning stick? Did it change your behavior?

```markdown
## Reflection (After 1-2 weeks)

### Did I Act on What I Learned?
- [ ] Yes, I took action
- [ ] Partially, I did some things
- [ ] No, I got busy
- [ ] Not yet applicable

**What happened:**
[Briefly describe what you did or didn't do]

---

### Did This Stick?
[Can you recall the main ideas without rereading? Are you thinking about it?]

---

### Practical Impact So Far
[Have you applied this yet? Have you changed your behavior? Any early results?]

---

### What I'd Do Differently
[If you consumed this source again, what would you focus on?]

---

### Who Should See This?
[Is there someone on your team who would benefit from this learning? Who?]
```

---

### 10. Metadata & Organization

For tracking and retrieval later.

```markdown
## Document Metadata

**Reading/Viewing Difficulty:**
[ ] Beginner-friendly
[ ] Intermediate (requires domain knowledge)
[ ] Advanced (assumes expertise)

**Time to Implement Learning:**
[ ] Quick wins (< 1 week)
[ ] Medium-term (1-3 months)
[ ] Long-term (3+ months)

**Relevance Decay:**
[ ] Evergreen (always relevant)
[ ] Time-sensitive (2026-2027)
[ ] Outdated? (mark here)

**Revisit on:**
[Date when you should come back to this. Example: 2026-12-27]

**Next Review:** [Date]

**Tags:** [Topic areas for searching]
- [#tag1]
- [#tag2]
- [#tag3]
```

---

## Usage Examples

### Example 1: YouTube Video

```yaml
---
type: Learning
id: learning_2026_07_27_01_systems_thinking_primer
domain: Learning & Development
title: "Systems Thinking in Product Design" (From Donella Meadows lecture)
source_type: video
source_title: "Donella Meadows - Systems Thinking (Remastered)"
source_author: Donella Meadows
source_url: https://www.youtube.com/watch?v=CqK3uRoPIUE
date_consumed: 2026-07-20
date_documented: 2026-07-27
created_at: 2026-07-27T14:30:00Z
tags:
  - systems-thinking
  - product-design
  - mental-models
source_duration: "47:23"
source_date: 2012-10-01
relevance: Foundational framework for understanding product ecosystems beyond immediate features
status: completed
---

## Source Context

**Title:** Donella Meadows - Systems Thinking (Remastered)

**Creator/Author:** Donella Meadows

**Format:** Video (YouTube)
- **Length:** 47 minutes 23 seconds
- **Date Published:** October 1, 2012 (remastered)
- **URL:** https://www.youtube.com/watch?v=CqK3uRoPIUE

**Why I Chose This:**
Systems thinking keeps coming up in product strategy discussions. This is the canonical intro from one of the field's founders.

**My Focus Area:**
How can I think about product networks, feedback loops, and second-order effects instead of just feature prioritization?

---

## Quick Summary

**Core Thesis:**
Most problems in complex systems come from ignoring feedback loops and trying to optimize single elements without understanding the whole system.

**Main Argument:**
- Systems have stocks, flows, and feedback loops
- Negative feedback (balancing) creates stability; positive feedback creates growth or collapse
- Most policy failures happen because people optimize locally without seeing the system effect
- Small leverage points in the right place can shift entire systems

**Who This Is For:**
Product managers, strategic thinkers, anyone managing complex systems (organizations, products, ecosystems)

**Type of Content:**
[X] Educational/Instructional

[More sections following the template...]
```

### Example 2: Book

```yaml
---
type: Learning
id: learning_2026_07_15_03_creative_strategy
domain: Learning & Development
title: "Steal Like an Artist (Austin Kleon) - Applied to Product Strategy"
source_type: book
source_title: Steal Like an Artist - 10 Things Nobody Told You About Being Creative
source_author: Austin Kleon
source_url: https://www.austinkleon.com/steal/
date_consumed: 2026-07-10
date_documented: 2026-07-15
created_at: 2026-07-15T10:00:00Z
tags:
  - creativity
  - strategy
  - learning
  - remixing
source_duration: "~160 pages"
source_date: 2012-09-01
relevance: Reframes copying/inspiration as a valid creative process; changes how I think about feature research
status: completed
---

[Document continues with learnings, key points, disagreements, etc.]
```

### Example 3: Research Paper

```yaml
---
type: Learning
id: learning_2026_07_22_02_ai_agent_autonomy
domain: Learning & Development
title: "Emergent Capabilities in LLM-Based Agents - A Critical Analysis"
source_type: paper
source_title: "Scaling Behavior of Agents in Language Model Frontiers"
source_author: Smith, J., Chen, L., & Williams, R.
source_url: https://arxiv.org/abs/2307.XXXXX
date_consumed: 2026-07-22
date_documented: 2026-07-25
created_at: 2026-07-25T16:20:00Z
tags:
  - AI
  - agents
  - language-models
  - research
source_duration: "~25 pages"
source_date: 2023-07-01
relevance: Challenges claims about agent autonomous decision-making; affects roadmap priorities
status: in-progress
---

[Document continues with critical section prominent given research paper context]
```

---

## Quick Workflow

### When You Start Consuming Content
1. Create a file with frontmatter (use YYYY-MM-DD of when you start)
2. Fill in: Source Context + Quick Summary
3. Mark status: `in-progress`

### While Consuming
4. Pause and jot down Key Learnings as you go
5. Note any Key Points to Remember (quotes, frameworks, data)

### After Finishing
6. Complete Points to Ponder (what questions does this raise?)
7. Add Disagreements / Critiques
8. Add Connections to Existing Knowledge
9. Decide on Immediate Actions
10. Mark status: `completed`

### 1-2 Weeks Later
11. Fill in Reflection section
12. Update status if appropriate
13. Set next review date if this is evergreen

---

## Tips for Effective Learning Documentation

**✅ Do:**
- Capture your own thinking, not just the source's
- Include disagreement—it shows you're thinking critically
- Link to related documents immediately (even if you haven't read them yet)
- Note confidence levels and unstated assumptions
- Set specific follow-up actions (vague is useless)

**❌ Don't:**
- Transcribe the entire source (that's not learning, that's copying)
- Wait for perfect notes (good-enough is better than never)
- Treat this as a passive filing system (it's a tool for thinking)
- Forget to come back (schedule a review date)
- Assume you'll remember connections later (document them now)

**💡 Pro Tips:**
- Use this template for deep, important sources (not everything needs this level of analysis)
- For quick videos, summarize in 2-3 bullets in a daily note instead
- Weekly: scan all `in-progress` docs and mark the ones actually done as `completed`
- Monthly: review 1-2 old learning docs to see if they changed your thinking
- Search by `source_type` or `tags` to find related learnings across your knowledge base

---

## ID Naming Convention

```
learning_YYYY_MM_DD_##_[topic-slug]

Examples:
✅ learning_2026_07_27_01_systems_thinking_primer
✅ learning_2026_07_15_02_creative_strategy_kleon
✅ learning_2026_07_22_03_ai_agent_autonomy (if 3 on same day)

❌ learning_01_systems (no date)
❌ learning_2026_7_27 (month/day not zero-padded)
❌ learning_systems_thinking (date order unclear)
```

---

## Document Status Values

| Status | Meaning | When to Update |
|--------|---------|---|
| **in-progress** | Still consuming or actively taking notes | While reading/watching |
| **completed** | Done consuming and initial reflection captured | Right after finishing |
| **reviewed** | Reflection added, connections made, actions taken | 1-2 weeks later |
| **archived** | No longer relevant; keeping for historical reference | When source becomes outdated |

---

## Connecting Learning Docs to Other Parts of Your Knowledge System

### To Projects
```markdown
**Related Learning:**
See [learning_2026_07_27_01_systems_thinking_primer.md](learning_2026_07_27_01_systems_thinking_primer.md)
**Why:** This project's architecture needs to account for system feedback loops
```

### To Proposals
```markdown
**Informed by:**
- [learning_2026_06_15_01_market_research.md](...)
- [learning_2026_07_10_03_competitor_analysis.md](...)
```

### To Other Learning Docs
```markdown
**Builds on:**
[learning_2026_06_30_02_game_theory_basics.md](learning_2026_06_30_02_game_theory_basics.md)

**Contradicts:**
[learning_2026_05_20_01_network_effects_myth.md](learning_2026_05_20_01_network_effects_myth.md)
**Difference:** [Brief explanation of the contradiction]
```

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2026-07-27 | Initial template creation |

---

**Created:** 2026-07-27
**Last Updated:** 2026-07-27
**Next Review:** 2026-10-27
