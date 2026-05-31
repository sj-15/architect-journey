# Contributing Guide — Sourav Jana Knowledge Repositories

This guide defines standards for all knowledge management repositories.

---

## 📝 Commit Message Convention

Using **Conventional Commits** format:

```
<type>(<scope>): <description>

[optional body]
```

### Types

| Type | Use For |
|---|---|
| `docs` | Adding or updating notes, READMEs, templates |
| `feat` | New topic added, new case study, new pattern |
| `fix` | Correcting wrong information, fixing code example |
| `refactor` | Restructuring existing content |
| `progress` | Updating progress logs, trackers |
| `review` | Monthly/weekly review entries |
| `chore` | Repo structure, gitignore, tooling |

### Scope Examples

| Scope | Repo |
|---|---|
| `concurrency` | java-backend-playground |
| `system-design` | system-design |
| `cap-theorem` | architecture-notes |
| `sliding-window` | dsa-patterns |
| `behavioral` | interview-prep |
| `progress` | architect-journey |

### Examples

```bash
docs(concurrency): add CompletableFuture chaining patterns
feat(system-design): add Twitter feed design case study
fix(cap-theorem): correct AP system examples
progress(june): update week 2 daily logs
review(monthly): add June 2026 monthly review
feat(sliding-window): add variable-size window template
docs(transactions): add Spring @Transactional self-invocation pitfall
```

---

## 📅 Daily Workflow

### Morning (before work)
```
1. Open progress-log/YYYY-MM.md
2. Review today's calendar events
3. Set top 3 goals for the day
```

### During Study
```
1. Take notes directly in relevant repo file
2. Stage changes as you go: git add -p
```

### Night (before sleep)
```bash
# Update progress log
vim architect-journey/progress-log/2026-06.md

# Stage and commit
git add .
git commit -m "progress(june): day N — [topic studied]"
git push

# Check GitHub streak
```

---

## 🏷️ Labels Strategy

### Priority Labels
| Label | Color | Meaning |
|---|---|---|
| `priority-critical` | 🔴 Red | Must complete this phase |
| `priority-high` | 🟠 Orange | Complete this month |
| `priority-medium` | 🟡 Yellow | Complete this quarter |
| `priority-low` | 🟢 Green | Backlog — do eventually |

### Type Labels
| Label | Color |
|---|---|
| `learning` | Blue |
| `weekly-goal` | Purple |
| `monthly-goal` | Purple |
| `dsa` | Teal |
| `system-design` | Teal |
| `java` | Teal |
| `career` | Pink |
| `phase-1` | Gray |
| `phase-2` | Gray |

---

## 🗂️ GitHub Project Board Columns

```
Backlog → This Month → This Week → In Progress → Review → ✅ Completed
```

**Rules:**
- Max 5 items in "In Progress" at once
- "This Week" gets populated every Sunday night
- "Completed" is never deleted — it's your evidence of growth

---

## 📌 Milestones

| Milestone | Target Date | Criteria |
|---|---|---|
| Phase 1 Complete | Nov 2026 | LeetCode 1900+, 6 case studies, AWS CCP |
| Interview Ready (Mid-tier) | Sep 2026 | DSA + 3 system designs + Java concurrency |
| AWS Certified | Sep 2026 | Cloud Practitioner passed |
| Interview Ready (Top-tier) | Jan 2027 | All phase targets met |

---

## 🗃️ Repository Naming Convention

```
[domain]-[purpose]
```

| Repo | Pattern |
|---|---|
| `architect-journey` | meta-growth |
| `java-backend-playground` | language-domain |
| `system-design` | domain-focused |
| `architecture-notes` | domain-notes |
| `dsa-patterns` | domain-patterns |
| `interview-prep` | purpose-domain |

Real project repos (not part of this system):
```
[project-name]           — e.g., distributed-url-shortener
[project-name]-frontend  — if separated
```
