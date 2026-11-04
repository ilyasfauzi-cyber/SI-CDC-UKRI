# AGENTS.md
# AI CODING AGENT GUIDELINES - SI CDC UKRI

## 1. Project Overview

You are assisting with the development of:

**Project Name:** Sistem Informasi Career Development Center (SI CDC UKRI)

**Institution:** Universitas Kebangsaan Republik Indonesia

**Repository:** https://github.com/ilyasfauzi-cyber/SI-CDC-UKRI

SI CDC UKRI is a Career Development Center information system designed to support student and alumni career development, job vacancy management, industry partnerships, and alumni tracer studies.

Your responsibility is to assist the development team while preserving the project's existing architecture, requirements, and coding standards.

## 2. Technology Stack

The project uses the following technologies:

- Backend: Laravel (PHP).
- Frontend: Blade.
- CSS Framework: Tailwind CSS.
- Database: MySQL.
- Local Development Environment: Laragon.
- Version Control: Git and GitHub.

Do not introduce a different framework or technology without explicit approval from the Project Leader.

Do not assume a specific Laravel, PHP, or Node.js version. Inspect the existing project configuration first.

## 3. Main System Modules

The application consists of three main modules:

### A. Talent Profile & Portfolio
- Student and alumni profiles.
- Educational background.
- Skills and competencies.
- Work experience.
- Portfolio management.

### B. Job Vacancies & DUDI Partnerships
- Job vacancy management.
- Company and DUDI information.
- Industry partnership management.
- Job information for students and alumni.

### C. Analytics & Tracer Study
- Alumni tracer study.
- Career development information.
- Data management and reporting.
- Analytics and dashboard information.

Follow the existing project documentation for detailed requirements. Do not invent functionality that has not been approved.

## 4. User Roles

The system is designed for five user categories:

1. Super Admin.
2. Admin CDC.
3. DUDI Representative.
4. Student / Alumni.
5. University Leadership.

Respect role-based permissions. Never allow users to access data or functionality outside their authorized roles.

## 5. Documentation Priority

Before implementing a feature, inspect the available project documentation.

Prioritize the following sources:

1. Kerangka Acuan Kerja (KAK).
2. Software Requirements Specification (SRS).
3. Project Plan.
4. Gantt Chart.
5. `README.md`.
6. `RULES.md`.

If documentation is inconsistent or a requirement is unclear, report the discrepancy to the user or Project Leader before making a significant implementation decision.

Do not silently change approved project requirements.

## 6. Development Principles

Follow these principles:

- Inspect the existing code before making changes.
- Preserve the existing Laravel architecture.
- Use Laravel conventions and best practices.
- Write clean, readable, and maintainable code.
- Avoid unnecessary dependencies.
- Reuse existing components and functions where appropriate.
- Keep changes focused on the requested task.
- Do not delete existing functionality without approval.
- Do not overwrite existing files without understanding their purpose.

## 7. Backend Guidelines

When developing backend functionality:

- Use Laravel MVC architecture.
- Use Controllers to handle application requests.
- Use Models for database interactions.
- Use Migrations for database structure changes.
- Use Seeders for development and testing data.
- Use Form Requests or appropriate validation mechanisms.
- Apply authentication and authorization where required.
- Use Eloquent ORM where appropriate.
- Handle errors and exceptions properly.
- Avoid exposing sensitive information in responses.

Do not modify production data or perform destructive database operations without explicit approval.

## 8. Frontend Guidelines

When developing frontend functionality:

- Use Blade templates.
- Use Tailwind CSS for styling.
- Create reusable components where appropriate.
- Maintain a consistent interface across pages.
- Make interfaces responsive for desktop, tablet, and mobile.
- Use clear labels, forms, buttons, and navigation.
- Provide validation feedback and useful error messages.
- Follow the existing design system if one has already been established.

Do not introduce another frontend framework without approval.

## 9. Database Guidelines

- Use MySQL as the primary database.
- Follow Laravel migration conventions.
- Use appropriate primary and foreign keys.
- Maintain referential integrity.
- Use appropriate indexes where necessary.
- Avoid duplicate and inconsistent data.
- Never hardcode database credentials.
- Keep database configuration in `.env`.

Before changing database structure, inspect the existing migrations and related models.

## 10. Security Guidelines

Security must be considered in every implementation.

- Validate all user input.
- Apply authorization checks.
- Protect sensitive information.
- Use secure password hashing.
- Avoid SQL injection vulnerabilities.
- Prevent unauthorized access.
- Do not expose API keys, passwords, or tokens.
- Never commit `.env` files or real credentials.
- Follow Laravel security conventions.

## 11. Git and Collaboration Guidelines

Follow the repository's `RULES.md`.

The team uses:

- `main` for stable releases.
- `develop` for integration.
- `feature/*` for individual feature development.

Never push directly to `main` or `develop` unless explicitly authorized.

Do not create commits, push branches, merge Pull Requests, or rewrite Git history without user authorization.

Use clear and consistent commit messages following Conventional Commits.

## 12. Testing and Quality Assurance

After implementing a feature:

1. Review the modified code.
2. Check for syntax errors.
3. Run relevant tests if available.
4. Verify database migrations when applicable.
5. Check authorization and validation.
6. Verify that existing functionality is not broken.
7. Report any tests that could not be executed.

Use the project's existing testing setup. Do not claim a feature works if it has not been tested.

## 13. AI Working Procedure

Before starting a task:

1. Read this `AGENTS.md`.
2. Read `RULES.md` and relevant documentation.
3. Inspect the existing project structure.
4. Understand the requested feature.
5. Identify the files that need to be changed.
6. Explain the implementation plan for significant changes.

During development:

- Work only within the requested scope.
- Explain important implementation decisions.
- Preserve existing code and project conventions.
- Ask for clarification when requirements are ambiguous.
- Do not fabricate test results.

After development:

- Summarize the files changed.
- Explain what was implemented.
- List commands or tests executed.
- Report errors and remaining tasks.
- Identify any changes that require team review.

## 14. Important Restrictions

The AI coding agent must not:

- Change the approved technology stack without permission.
- Invent project requirements.
- Remove existing features without permission.
- Delete database tables or records without approval.
- Modify GitHub branch protection settings.
- Expose credentials or private information.
- Commit unfinished or untested code as completed work.
- Claim that an implementation is finished without verification.

## 15. Main Objective

The main objective is to help the SI CDC UKRI team develop a reliable, secure, maintainable, and well-documented Career Development Center information system.

All implementation decisions must remain consistent with the approved project requirements and the team's development workflow.
