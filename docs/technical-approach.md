# Technical Approach for Cognia Accreditation Website

This document outlines the technical requirements and approach for building the Cognia accreditation website, based on the agreed structure and best practices for static sites hosted on GitHub Pages.

---

## 1. Project Setup and Hosting
- **Platform:** GitHub Pages (static site hosting)
- **Version Control:** Git and GitHub repository
- **Branching:** Use `gh-pages` or `/docs` folder in `main` branch for deployment

## 2. Website Structure & Content Management
- **Type:** Static informational website
- **Content:** Written in Markdown (`.md`) for easy editing
- **Static Site Generator (SSG):**
  - **Recommended:** Jekyll (native to GitHub Pages)
  - **Alternatives:** Hugo or Eleventy (require GitHub Actions for deployment)
- **File Structure:**
  - `_layouts/` (Jekyll) – Common page templates
  - `_includes/` (Jekyll) – Reusable components (header, footer, nav)
  - `pages/` – Individual content pages (e.g., `comprehensive-plan.md`, `timeline.md`)
  - `assets/` – CSS, JS, images
  - `index.html` – Homepage

## 3. Design and User Interface (UI)
- **Styling:** Use a modern, responsive CSS framework (e.g., Bootstrap or Tailwind CSS)
- **Theming:** Clean, professional, and easy to navigate
- **Navigation:**
  - **Main Navigation Items:**
    - Home (introduction and website purpose)
    - Self-Assessment Overview (process, timeline, improvement cycle)
    - Standards & Criteria
      - Sub-navigation: Culture of Learning, Leadership for Learning, Engagement of Learning, Growth in Learning
    - Data Collection & Analysis
      - Sub-navigation: Student Performance, Stakeholder Feedback, Learning Environment
    - Evidence Directory (organization and guidance)
    - Timeline (detailed phases and milestones)
    - Committees & Teams
      - Sub-navigation: ASC, Data Lead, RATs, KCWGs, Executive Summary Team, QARC
    - Quality Assurance (QA plan and review process)
    - Supporting Documents (policies, handbooks, plans, etc.)
    - Glossary & Resources (key terms, templates, links)
  - **Optional Features:**
    - Search bar for quick access to standards, evidence, or team members
    - Quick links to templates or submission forms
    - FAQ section for common questions
- **Navigation Design:**
  - Use a top-level menu for main sections, with dropdowns or sidebar navigation for sub-sections where appropriate
  - Ensure mobile-friendliness and accessibility
  - Prioritize clarity, readability, and intuitive user flow

## 4. Content Sections
- **Each main navigation item should correspond to a dedicated page or group of related pages.**
- **Use Markdown for content, with clear templates for each section to ensure consistency and ease of editing.**

### Recommended Content Sections and Subsections

- **Home**
  - Welcome message, accreditation overview, and quick links.

- **Self-Assessment Overview**
  - Purpose, process summary, and timeline snapshot.

- **Standards & Criteria**
  - Overview of Cognia standards and key characteristics.
  - Subpages for each Key Characteristic:
    - Culture of Learning
    - Leadership for Learning
    - Engagement of Learning
    - Growth in Learning
  - For each: list of relevant standards, rubrics, rating criteria, evidence requirements, and links.

- **Data Collection & Analysis**
  - Overview of required analyses.
  - Subpages for:
    - Student Performance
    - Stakeholder Feedback
    - Learning Environment
  - For each: data types, templates, analysis process, and sample reports.

- **Evidence Directory**
  - Explanation of directory structure.
  - Guidelines for submitting and linking evidence.
  - Example: How to reference evidence in narratives.

- **Timeline**
  - Visual timeline (vertical or horizontal) of phases, tasks, and milestones.
  - Downloadable or printable version.

- **Committees & Teams**
  - Overview of team structure.
  - Subpages for each committee/team:
    - Mandate, members, roles, and responsibilities
    - Contact info (if appropriate)
    - Meeting schedules or minutes (optional)

- **Quality Assurance**
  - QA plan, review process, and feedback workflow.

- **Supporting Documents**
  - List and links to policies, handbooks, improvement plans, and other key documents.

- **Glossary & Resources**
  - Definitions of key terms.
  - Downloadable templates and helpful links.

### Additional Guidance
- **Encourage cross-linking** between sections (e.g., from a standard to its evidence, or from a committee to its responsibilities in the timeline).
- **Use headings, tables, and lists** for clarity and accessibility.
- **Include callouts or info boxes** for important notes or tips.

## 5. Deployment & Automation
- **Jekyll:** Standard GitHub Pages deployment
- **Other SSGs:** Use GitHub Actions workflow for build and deploy
- **Configuration:**
  - `_config.yml` (Jekyll)
  - `.github/workflows/deploy.yml` (if needed)

## 6. AI Interaction & Iterative Development
- Be explicit and incremental in requests to AI tools
- Example prompts:
  - "Generate the basic Jekyll project structure."
  - "Create a Markdown file for the 'Comprehensive Plan'."
  - "Design a responsive layout for the 'Timeline' section."
  - "Provide HTML/CSS for a 'Committees' section."

---

**This document serves as the technical foundation for the Cognia accreditation website project.** 