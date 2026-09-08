# PREP — Exam Prep Dashboards

Personal, interactive study dashboards for competitive exams. One folder per exam, each with its own single-page dashboard (syllabus checklist, previous-year papers, progress tracking). Deployed to GitHub Pages via GitHub Actions.

**Live site:** https://pimpalemahesh.github.io/PREP/

## Structure

```
.
├── index.html              # landing page (lists all exams)
├── ISRO/
│   └── index.html          # ISRO Scientist/Engineer 'SC' — Computer Science
└── .github/workflows/
    └── deploy.yml          # builds & deploys the whole site to GitHub Pages
```

## Adding a new exam

1. Create a new folder (e.g. `GATE/`) with an `index.html`.
2. Add a card linking to it in the root `index.html`.
3. Push to `master` — the workflow redeploys automatically.

## Exams

### ISRO Scientist/Engineer 'SC' — Computer Science  →  `/ISRO/`
Interactive dashboard for the ISRO ICRB written exam (Post Code BE003):
- Live readiness meter — weighted across syllabus learning (50%), previous-year papers (30%) and revision/mocks (20%). Progress saves in the browser's local storage; use the in-page Export button to back it up.
- Full syllabus as a tick-able checklist, ordered by weightage, with notes links.
- 92-day study calendar.
- Previous-year paper tracker — links to each paper's public source (Google Drive / GATE Overflow) plus online quizzes.
- Part B (General Aptitude & Reasoning) and revision/mock trackers.

**Notes:** ISRO publishes no official CS syllabus; content treats it as GATE-CSE-equivalent plus applied topics. Subject weightage and calendar are an unofficial community estimate. Previous-year papers are linked to their existing public sources, not re-hosted here. Always confirm exam pattern, marking and dates against the official notification on [isro.gov.in](https://www.isro.gov.in/).

---

*Personal study aid. Not affiliated with ISRO or any exam body.*
