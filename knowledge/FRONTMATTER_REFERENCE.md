---
id: frontmatter_reference
type: Guide
title: YAML Frontmatter Reference for Proposals & Projects
date: 2026-07-26
---

# YAML Frontmatter Reference

The YAML frontmatter (the section between `---` and `---` at the top of each file) contains metadata that makes your files searchable, organized, and properly structured.

---

## Proposal Frontmatter

```yaml
---
type: Proposal
id: proposal_YYYY_MM_DD_xx
domain: Proposals
title: [Clear, concise title - focus on business outcome]
date: YYYY-MM-DD
status: draft|review|approved|rejected|archived
created_at: YYYY-MM-DDTHH:MM:SSZ
updated_at: YYYY-MM-DDTHH:MM:SSZ
---
```

### Field Explanations

| Field | Format | Example | Why |
|-------|--------|---------|-----|
| **type** | String | `Proposal` | Identifies this as a proposal (for searching/filtering) |
| **id** | `proposal_YYYY_MM_DD_xx` | `proposal_2026_07_26_01_api_modernization` | Unique identifier; date ensures chronological order; xx = counter if multiple same day |
| **domain** | String | `Proposals` | Links to your domain in personal_knowledge_base.okf |
| **title** | String | `Modernize Legacy API Architecture` | Business-focused, searchable title |
| **date** | YYYY-MM-DD | `2026-07-26` | When the proposal was created |
| **status** | One of: draft, review, approved, rejected, archived | `draft` | Current state of proposal |
| **created_at** | ISO 8601 timestamp | `2026-07-26T14:30:00Z` | When file was created (helps with archiving) |
| **updated_at** | ISO 8601 timestamp | `2026-07-26T16:45:00Z` | Last time file was updated |

---

## Project Frontmatter

```yaml
---
type: Project
id: project_YYYY_MM_DD_xx
domain: Projects
title: [Project name - clear, business-focused]
date: YYYY-MM-DD
status: planning|in-progress|at-risk|blocked|completed|archived
updated: YYYY-MM-DD
related_proposal: [proposal_id]
---
```

### Field Explanations

| Field | Format | Example | Why |
|-------|--------|---------|-----|
| **type** | String | `Project` | Identifies this as a project (for searching/filtering) |
| **id** | `project_YYYY_MM_DD_xx` | `project_2026_07_26_01_api_modernization` | Unique identifier matching the proposal it came from |
| **domain** | String | `Projects` | Links to your domain in personal_knowledge_base.okf |
| **title** | String | `API Modernization - REST + Event Streaming` | Project name, clear and searchable |
| **date** | YYYY-MM-DD | `2026-07-26` | When project was initiated (kickoff date) |
| **status** | One of: planning, in-progress, at-risk, blocked, completed, archived | `in-progress` | Current project state |
| **updated** | YYYY-MM-DD | `2026-07-27` | Last date status was updated (update weekly on Friday) |
| **related_proposal** | proposal_id | `proposal_2026_07_26_01_api_modernization` | Links back to the proposal that created this project |

---

## Status Values Reference

### For Proposals:
- **draft** → Still writing, not ready to present
- **review** → Shared with stakeholders, waiting for feedback
- **approved** → Greenlit! Ready to become a project
- **rejected** → Decision made to not proceed (keep for learning)
- **archived** → No longer relevant, but keeping for reference

### For Projects:
- **planning** → In Phase 0 (not yet executing)
- **in-progress** → Actively executing (update every Friday)
- **at-risk** → On track but watching closely (key risks surfacing)
- **blocked** → Cannot proceed (waiting on external dependency)
- **completed** → Project finished, retrospective done
- **archived** → Old project, reference only

---

## ID Naming Convention

### Why This Matters:
IDs allow you to:
- Find any file quickly (alphabetical/chronological order)
- Link files together (proposal → project)
- Track patterns over time (what you've done when)

### Proposal ID Format:
```
proposal_YYYY_MM_DD_##_[topic-slug]

Examples:
✅ proposal_2026_07_26_01_api_modernization
✅ proposal_2026_08_15_02_cloud_security
✅ proposal_2026_08_15_03_data_governance (if 2 proposals same day)

❌ proposal_01_api (no date)
❌ proposal_api_modernization (unclear date order)
❌ proposal_2026_7_26 (month/day not zero-padded)
```

**Format breakdown:**
- `proposal_` — Type indicator
- `YYYY_MM_DD` — Date (zero-padded, chronological order)
- `##` — Counter (01, 02, 03... for same day)
- `_topic-slug` — URL-safe topic name (optional, but helpful)

### Project ID Format:
```
project_YYYY_MM_DD_##_[topic-slug]

Examples:
✅ project_2026_07_26_01_api_modernization
✅ project_2026_08_15_02_cloud_security

❌ project_01_api (no date)
❌ project_api_modernization (unclear date order)
```

**Matching pattern:** Project ID should match the related proposal ID to link them.

---

## Linking Proposals & Projects

When a proposal gets approved and becomes a project, link them:

### In the Project frontmatter:
```yaml
related_proposal: proposal_2026_07_26_01_api_modernization
```

### In the Project "Project Overview" section:
```markdown
## Approved Proposal
See: `proposals/2026-07_example_api_modernization/proposal_api_modernization.okf`

For business context, stakeholder analysis, and decision rationale.
```

This creates traceability from execution back to the original thinking.

---

## Date Handling

### When to update dates:

**created_at:** Set once, never change
```yaml
created_at: 2026-07-26T14:30:00Z  # When you created the file
```

**updated_at (Proposals):** Update every time you edit the file
```yaml
updated_at: 2026-07-26T16:45:00Z  # Last edit time
```

**updated (Projects):** Update every Friday
```yaml
updated: 2026-07-27  # Most recent status update (YYYY-MM-DD)
```

**date:** Set once, don't change
```yaml
date: 2026-07-26  # Original date (proposal created / project started)
```

---

## Common Frontmatter Mistakes

### ❌ Mistake 1: Missing `type` field
```yaml
---
id: proposal_2026_07_26_01
domain: Proposals
title: My Proposal
```

**Why it matters:** Without `type`, you can't filter/search by Proposal vs. Project

**Fix:**
```yaml
---
type: Proposal
id: proposal_2026_07_26_01
```

---

### ❌ Mistake 2: Inconsistent date format
```yaml
date: 2026/07/26        # Wrong format
date: 07-26-2026        # Wrong format
date: 2026-7-26         # Wrong format (month/day not zero-padded)
```

**Why it matters:** Non-standard formats don't sort chronologically

**Fix:**
```yaml
date: 2026-07-26        # YYYY-MM-DD (ISO 8601)
```

---

### ❌ Mistake 3: Changing the `date` field
```yaml
date: 2026-07-26        # Original proposal creation date
# ... months later ...
date: 2026-12-15        # DON'T CHANGE THIS
```

**Why it matters:** The date should represent when the work started, not when you last edited it

**Fix:**
```yaml
date: 2026-07-26              # Original (never changes)
updated_at: 2026-12-15T10:00Z # Update this instead
```

---

### ❌ Mistake 4: Non-standard status values
```yaml
status: in_progress     # Wrong (use hyphens, not underscores)
status: inprogress      # Wrong (use hyphens)
status: active          # Wrong (not in standard list)
```

**Why it matters:** Can't reliably query/filter if status values are inconsistent

**Fix:**
```yaml
status: in-progress     # Use standard values only
```

---

### ❌ Mistake 5: Forgetting to link proposal to project
```yaml
# In project file, forget to add:
related_proposal: proposal_2026_07_26_01_api_modernization
```

**Why it matters:** You lose the connection between thinking phase and execution phase

**Fix:**
```yaml
type: Project
id: project_2026_07_26_01_api_modernization
related_proposal: proposal_2026_07_26_01_api_modernization
```

---

## Copy-Paste Templates

### Use These to Create New Files

**For a new PROPOSAL:**
```yaml
---
type: Proposal
id: proposal_YYYY_MM_DD_##_[topic]
domain: Proposals
title: [Business outcome focused title]
date: YYYY-MM-DD
status: draft
created_at: YYYY-MM-DDTHH:MM:SSZ
updated_at: YYYY-MM-DDTHH:MM:SSZ
---
```

**For a new PROJECT:**
```yaml
---
type: Project
id: project_YYYY_MM_DD_##_[topic]
domain: Projects
title: [Project name]
date: YYYY-MM-DD
status: planning
updated: YYYY-MM-DD
related_proposal: proposal_YYYY_MM_DD_##_[topic]
---
```

---

## Quick Checklist

Before you create a new file, verify:

- [ ] `type` field is present (Proposal or Project)
- [ ] `id` follows naming convention (proposal_YYYY_MM_DD_##_topic)
- [ ] `date` is in YYYY-MM-DD format
- [ ] `status` is one of the standard values
- [ ] Timestamps use ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
- [ ] Project has `related_proposal` field linking back
- [ ] Fields are exactly as shown (no typos like `updated_at` vs `updated`)

---

## Why Metadata Matters

Good frontmatter enables:
- **Searching:** "Show me all proposals from Q3 2026"
- **Linking:** "Here's the project that came from this proposal"
- **Archiving:** "What proposals did I write 2 years ago?"
- **Tracking:** "Am I in planning, at-risk, or blocked?"
- **Consistency:** Everyone uses the same structure

**Invest 2 minutes in correct frontmatter. Save 2 hours later when you're searching for that proposal from last year.**
