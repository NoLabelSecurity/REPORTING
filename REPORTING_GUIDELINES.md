# 🤖 REPORTING_GUIDELINES.md

> Purpose:
>
> This document serves as the operating manual for maintaining every report within the `/REPORTS` directory.
>
> The instructions in each section are copied verbatim from the corresponding report template. If a report's maintenance instructions change, they should also be updated here to keep this document synchronized.

---

# Global Reporting Standards

These instructions apply to every report.

- Never fabricate data.
- Never duplicate information between reports.
- Preserve historical information.
- Update timestamps.
- Use Markdown formatting consistently.
- Preserve HTML `<details>` sections.
- Keep reports synchronized.
- If information cannot be determined, record **Unknown** rather than guessing.

---

# README.md

## Purpose

Describe the REPORTS directory and explain the responsibility of each report.

## Instructions

When updating this report:

- Keep reports synchronized.
- Avoid duplicate information across reports.
- Preserve development history.
- Update metrics automatically.
- Record meaningful decisions.
- Remove outdated technical documentation.
- Maintain consistent formatting.
- Keep client reports non-technical.

---

# PROJECT.md

## Purpose

High-level dashboard and current project status.

## Instructions

When updating this report:

- Update project completion percentage.
- Refresh development statistics.
- Update current milestone and focus.
- Add newly completed work.
- Move completed tasks out of "Currently Working On."
- Record any new blockers or risks.
- Update the Recent Activity table.
- Update the Last Updated timestamp.
- Never delete historical milestones—move them into DEVELOPMENT.md.
- Keep this report concise; detailed information belongs in the other reports.

---

# DEVELOPMENT.md

## Purpose

Development journal, coding sessions, prompt history, changelog, deployments, and repository activity.

## Instructions

When updating this report:

- Append new sessions; never overwrite previous ones.
- Record every meaningful coding session.
- Document commits, pushes, deployments, and branch changes.
- Record significant AI prompts and summarize their outcomes instead of logging trivial prompts.
- Generate a human-readable changelog from code changes.
- Update development metrics automatically.
- Record architectural decisions only when they materially affect the project.
- Preserve historical data.
- Keep entries concise and avoid repeating information already documented elsewhere.

---

# FEATURES.md

## Purpose

Track completed features, active work, roadmap, bugs, technical debt, and enhancements.

## Instructions

When updating this report:

- Update feature progress percentages automatically.
- Move completed features from **Active Development** to **Completed Features**.
- Add newly requested functionality to **Planned Features** unless immediately implemented.
- Record discovered bugs in the Bug Tracker.
- Move resolved bugs to **Recently Fixed**.
- Add shortcuts, workarounds, or deferred improvements to **Technical Debt**.
- Record client requests as **Enhancements** unless they represent entirely new features.
- Keep the Version Roadmap aligned with the project's milestones.
- Never delete completed features or resolved bugs—preserve project history.
- Update feature counts and completion statistics after every meaningful development session.

---

# ANALYTICS.md

## Purpose

Track development hours, AI usage, repository metrics, productivity, and project statistics.

## Instructions

When updating this report:

- Recalculate all metrics automatically after each development session.
- Estimate development hours based on coding activity if exact time tracking is unavailable.
- Categorize AI prompts by purpose and track acceptance rates.
- Calculate estimated AI vs. manual code contribution.
- Record repository activity including commits, pushes, branches, merges, and deployments.
- Track codebase growth (files, components, pages, APIs, and lines of code).
- Update performance metrics whenever benchmarks are available.
- Preserve historical trends instead of overwriting them.
- Highlight noteworthy milestones, productivity achievements, and efficiency improvements.
- Keep all metrics cumulative and easy to compare over time.

---

# DOCUMENTATION.md

## Purpose

Maintain technical documentation describing the project's current implementation.

## Instructions

When updating this report:

- Always reflect the **current** implementation rather than historical changes.
- Automatically update the project structure when folders or major files are added or removed.
- Keep the technology stack synchronized with installed dependencies.
- Document new API routes, database models, and reusable components.
- Update deployment instructions when infrastructure changes.
- Remove obsolete documentation instead of leaving stale information.
- Keep explanations concise, accurate, and developer-focused.
- This document should allow a new developer to understand the project without reading the source code first.

---

# CLIENT.md

## Purpose

Maintain a client-friendly progress report written in non-technical language.

## Instructions

When updating this report:

- Write for a non-technical audience.
- Avoid mentioning commits, AI prompts, repositories, branches, or implementation details.
- Summarize completed work in plain English.
- Highlight new functionality instead of code changes.
- Update overall project progress and milestone completion.
- Clearly identify any items requiring client approval or feedback.
- Keep language positive, concise, and easy to understand.
- Focus on outcomes and deliverables rather than technical implementation.
- If screenshots exist, reference the most recent versions to visually demonstrate progress.

---

# PROJECT_MEMORY.md

## Purpose

Maintain long-term project knowledge including design decisions, client preferences, lessons learned, recurring patterns, and future ideas.

## Instructions

When updating this report:

- Record **why** decisions were made, not just what changed.
- Preserve client preferences and design direction throughout the project.
- Document architectural reasoning and tradeoffs.
- Add lessons learned after major milestones.
- Record recurring development patterns and reusable solutions.
- Update technical constraints and future improvement ideas.
- Capture information that would normally exist only in the developer's memory.
- Keep this report concise, organized, and evergreen.
- Do **not** duplicate information already tracked in DEVELOPMENT.md or DOCUMENTATION.md.
- Think of this report as the project's long-term memory rather than a changelog.

---

# Update Order

Whenever a development session is completed, Gemini should determine which reports are affected and update only those reports.

Recommended order:

1. PROJECT.md
2. DEVELOPMENT.md
3. FEATURES.md
4. ANALYTICS.md
5. DOCUMENTATION.md *(if architecture changed)*
6. CLIENT.md *(if client-visible work occurred)*
7. PROJECT_MEMORY.md *(if new long-term knowledge was gained)*

---

# Completion Checklist

After updating reports, verify:

- [ ] PROJECT.md synchronized
- [ ] DEVELOPMENT.md synchronized
- [ ] FEATURES.md synchronized
- [ ] ANALYTICS.md synchronized
- [ ] DOCUMENTATION.md synchronized (if applicable)
- [ ] CLIENT.md synchronized (if applicable)
- [ ] PROJECT_MEMORY.md synchronized (if applicable)
- [ ] Shared metrics match across reports
- [ ] Completion percentages are consistent
- [ ] Timestamps updated