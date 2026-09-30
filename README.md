# Kooch — CSC301 Group 6

This is the CSC301 course repository for Group 6's partnership project with Kooch. It contains course deliverables and documentation. The application source code remains in Kooch's partner repository and will be linked here once the team receives access.

## Partner Intro

Kooch is a settlement and integration platform for international newcomers. It helps newcomers navigate important tasks related to immigration, housing, banking, healthcare, and community life. The platform currently focuses on the Netherlands and plans to support additional countries.

| Partner information | Details |
| --- | --- |
| Partner organization | **Kooch** |
| Primary partner contact | **Nazanin** — Product Contact |
| Partner email | [nazanin.mirsharifi@gmail.com](mailto:nazanin.mirsharifi@gmail.com) |
| Technical partner contact | **Hossein** — Technical Contact and Repository Support; email not provided |
| Kooch GitHub organization | [https://github.com/letskooch](https://github.com/letskooch) |
| Deployed application | [https://letskooch.com](https://letskooch.com) |

Complete contact information will also be maintained in `deliverables/team/Stakeholders.txt`.

## Team Organization and Partner Communication

- **Qilin — Primary Kooch Liaison and Roadmap UI Developer:** Main contact with Nazanin and Hossein; collects team questions, sends meeting agendas, communicates with the partner and TA, helps maintain meeting minutes, and works on the user-facing roadmap, intake flow, multilingual interface, and right-to-left support.
- **Nikolos — Backup Kooch Liaison and Admin Editor Lead:** Acts as the secondary partner contact and leads development of the rule editor and preview feature.
- **Roni — Team Coordinator and Co-Engine Lead:** Coordinates internal meetings and sprint planning and co-leads development of the rule-pack format, validator, and roadmap generator.
- **Isabelle — Rules Engine Lead:** Leads the rule-pack format, validation logic, and roadmap-generation engine.
- **Bohan — Roadmap UI and QA Developer:** Works on the user-facing roadmap, intake flow, multilingual and right-to-left support, test profiles, and quality assurance.
- **Jia Ying — Rule Content Lead:** Researches official Netherlands settlement sources and prepares rule content for Kooch's review.
- **Ryan — QA and Testing Lead:** Leads test-profile creation, automated engine testing, and the release checklist.

Primary responsibilities identify ownership but do not prevent members from contributing to other parts of the system. Qilin is the main liaison with Kooch, Nikolos is the backup liaison, and Roni supports planning and meeting coordination. Partner communication takes place through WhatsApp, with Google Meet meetings scheduled when clarification, feedback, or approval is required.

## Description About the Project

Settlement information is often scattered across government websites, forums, and informal advice. Kooch provides newcomers with one personalized, step-by-step settlement roadmap.

Our project will extend Kooch's existing Netherlands-focused roadmap into a configurable system. Country-specific tasks, conditions, deadlines, dependencies, translations, and expert-help categories should be managed as rule data rather than rebuilt in code for every country.

## Key Features

The proposed MVP includes:

1. **Personalized intake and roadmap:** Users answer questions about their country, city, visa type, nationality group, arrival date, and purpose. The system displays only relevant tasks.
2. **Task dependencies:** Blocked tasks are visually distinct, explain their prerequisites, and unlock when prerequisite tasks are completed.
3. **Arrival-based deadlines:** Due dates are calculated from the user's arrival or start date, with clear guidance for upcoming or missed deadlines.
4. **Configurable rule editor:** Authorized Kooch staff can edit task content, conditions, dependencies, translations, and deadline offsets without changing application code.
5. **Preview and versioning:** Administrators can compare draft rule results across sample profiles before publishing while preserving previous rule versions.
6. **Expert handoff:** Selected tasks can link users to an appropriate professional-help category without exposing unnecessary personal information.
7. **Multilingual roadmap:** The MVP supports English and Farsi, including right-to-left rendering. Supported languages will be configured in rule data rather than hardcoded.

The final MVP scope is subject to the partner's written approval and may be refined after the team reviews the existing codebase.

## Instructions

The expected end-user flow is:

1. Open the Kooch application and sign in or create an account.
2. Open the settlement roadmap from the user's journey dashboard.
3. Complete the intake questionnaire.
4. Review the generated roadmap and its current journey stage.
5. Open tasks to view instructions, prerequisites, and deadlines.
6. Complete available tasks; dependent tasks unlock automatically.
7. Use **Get Help** when a task offers professional support.
8. Switch between available languages when needed.

The existing application is available at [letskooch.com](https://letskooch.com). Final testing accounts and feature-specific access instructions will be added after the roadmap feature is deployed.

## Development Requirements

The existing Kooch application uses **Next.js, TypeScript, Prisma, Vercel, and Sentry**. The authoritative setup instructions are maintained in Kooch's development repository.

After repository access is provided, developers will generally:

1. Accept the invitation to Kooch's GitHub organization.
2. Clone the development repository.
3. Install the required Node.js dependencies.
4. Configure local environment variables without committing secrets.
5. Follow the documented Prisma database setup or migration process.
6. Start the Next.js development server.
7. Run the repository's tests, linting, and other automated checks.

Exact commands, supported runtime versions, database requirements, and environment-variable names will be added after the team reviews the partner's setup documentation.

## Deployment and GitHub Workflow

Course documentation is stored in this CSC301 repository. Application code is developed in Kooch's repository, following the partner's existing branching and deployment conventions.

For each implementation task, a team member creates a dedicated branch and opens a pull request into the partner repository's designated integration branch. Every pull request requires approval from at least one team member who is not its author. After approval and successful automated checks, the pull-request author may merge it. Vercel is the existing deployment platform; the precise preview and production deployment process will be documented after the codebase walkthrough.

This workflow provides review before integration, reduces conflicts, and keeps course documentation separate from the partner's production code.

## Coding Standards and Guidelines

The team will follow the existing Kooch codebase conventions for TypeScript, Next.js, formatting, linting, naming, tests, and documentation. New conventions will be agreed upon with the partner and enforced through code review and automated checks where possible.

## Licenses

Students and the University will not assert intellectual-property ownership over work developed for Kooch, in accordance with CSC301 course requirements. The project will remain in Kooch's repository and follow Kooch's existing license and usage terms. The team will confirm with the partner whether the code is proprietary or uses a specific software license before the final release.

## Deployed URL / Access Instructions

- **Current Kooch application:** [https://letskooch.com](https://letskooch.com)
- **Kooch GitHub organization:** [https://github.com/letskooch](https://github.com/letskooch)
- **Development repository:** Link to be added after access is granted.
- **Roadmap test access:** Test account and feature instructions to be added when available.

## Course Deliverables

Course deliverables are stored under `deliverables/`. For D1, the required planning document and prototype materials belong in `deliverables/D1`, while the team roster, stakeholder information, and meeting minutes belong in `deliverables/team`.

Each submitted deliverable will be tagged as a GitHub release according to the course instructions. The D1 release will be named `deliverable-1`, and one team member will submit its release URL on Quercus on behalf of the team.

## D3 Improvement Highlight

Not applicable for D1. This section will be updated for D3 with a brief summary of changes made since D2 and instructions for locating them.
