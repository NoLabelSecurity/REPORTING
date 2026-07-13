# 📁 Reports Directory

> This directory contains automatically maintained project reports generated and updated by Gemini throughout the development lifecycle.
>
> Each report has a single responsibility to keep documentation organized, prevent duplication, and provide quick access to project information.

---

# Reports

| Report | Description |
|---------|-------------|
| **PROJECT.md** | High-level project dashboard showing current status, progress, milestones, blockers, and overall health. |
| **DEVELOPMENT.md** | Complete development journal including coding sessions, AI prompt history, changelog, deployments, and repository activity. |
| **FEATURES.md** | Tracks completed, active, planned, and future features, bugs, enhancements, technical debt, and release readiness. |
| **ANALYTICS.md** | Development metrics including hours, productivity, AI contribution, Git activity, performance, and project statistics. |
| **DOCUMENTATION.md** | Technical reference for the current architecture, project structure, APIs, database, components, deployment, and configuration. |
| **CLIENT.md** | Non-technical progress report summarizing completed work, current development, deliverables, timeline, and client action items. |
| **KNOWLEDGE_BASE.md** | Long-term project knowledge including design decisions, client preferences, lessons learned, architectural reasoning, and future ideas. |

---

# Which Report Should I Update?

| If you changed... | Update |
|-------------------|--------|
| Project status or milestone | PROJECT.md |
| Code or development sessions | DEVELOPMENT.md |
| Features, bugs, or roadmap | FEATURES.md |
| Hours, commits, AI metrics | ANALYTICS.md |
| Architecture or APIs | DOCUMENTATION.md |
| Client-facing progress | CLIENT.md |
| Design decisions or lessons learned | KNOWLEDGE_BASE.md |

---

# Report Relationships

```text
                PROJECT.md
                     │
      ┌──────────────┼──────────────┐
      │              │              │
 DEVELOPMENT.md   FEATURES.md   ANALYTICS.md
      │              │
      └──────────────┼──────────────┐
                     │              │
          DOCUMENTATION.md    KNOWLEDGE_BASE.md
                     │
                     │
                CLIENT.md
```

---

# Update Philosophy

Each report has a dedicated purpose.

- **PROJECT.md** is the dashboard.
- **DEVELOPMENT.md** records history.
- **FEATURES.md** tracks project scope.
- **ANALYTICS.md** measures progress.
- **DOCUMENTATION.md** describes the current implementation.
- **CLIENT.md** communicates progress to the client.
- **KNOWLEDGE_BASE.md** preserves project knowledge.

Information should exist in **one report only** whenever possible.

---

# Gemini Responsibilities

Gemini should automatically:

- Update reports after meaningful development sessions.
- Keep metrics synchronized across reports.
- Preserve historical information.
- Remove obsolete technical documentation.
- Avoid duplicate information between reports.
- Write client reports using non-technical language.
- Record architectural decisions and lessons learned.
- Maintain consistent formatting throughout the REPORTS directory.

---

# Reporting Workflow

```text
Development Session
        │
        ▼
Analyze Repository Changes
        │
        ▼
Determine Affected Reports
        │
        ▼
Update Relevant Report(s)
        │
        ▼
Synchronize Shared Metrics
        │
        ▼
Complete
```

---

> **Note:** These reports complement the project's root `README.md`. The root README explains **how to use the project**, while the files in this directory document **how the project evolves over time**.
