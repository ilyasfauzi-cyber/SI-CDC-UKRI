# CLAUDE.md
# SI CDC UKRI - Claude Code Instructions

## 1. Project Information

**Project:** Sistem Informasi Career Development Center (SI CDC UKRI)  
**Institution:** Universitas Kebangsaan Republik Indonesia  
**Repository:** https://github.com/ilyasfauzi-cyber/SI-CDC-UKRI

**Technology Stack:**
- Backend: Laravel (PHP)
- Frontend: Blade
- CSS Framework: Tailwind CSS
- Database: MySQL
- Local Development: Laragon

## 2. Mandatory Instructions

Before performing any development task, you MUST read and follow:

1. `AGENTS.md` — AI coding guidelines and project development standards.
2. `RULES.md` — Team collaboration, Git workflow, commit, and Pull Request rules.
3. `README.md` — Project overview, technology stack, and setup instructions.

These files are the primary references for project development.

## 3. Project Documentation

Before implementing features, inspect the available project documentation, especially:

- KAK
- Software Requirements Specification (SRS)
- Project Plan
- Gantt Chart

Use approved project documents as the source of functional requirements.

If requirements conflict or are unclear, explain the issue and ask for clarification before making major changes.

## 4. Development Rules

- Inspect the existing codebase before modifying files.
- Follow the existing Laravel architecture and coding conventions.
- Use Blade and Tailwind CSS for frontend development.
- Use MySQL for database operations.
- Maintain consistent UI and application structure.
- Use migrations for database structure changes.
- Apply authentication, validation, and authorization appropriately.
- Do not introduce unnecessary dependencies.
- Do not remove existing functionality without approval.
- Do not invent features outside approved requirements.

## 5. Team Collaboration

Follow the Git workflow defined in `RULES.md`.

- `main`: Stable application version.
- `develop`: Integration branch.
- `feature/*`: Feature development branches.

Do not directly push to shared branches or perform Git operations that modify shared history without explicit authorization.

## 6. Working Procedure

For every development task:

1. Understand the user's requested task.
2. Read the relevant project instructions and documentation.
3. Inspect existing files and implementation.
4. Explain the plan before significant changes.
5. Implement only the requested scope.
6. Run relevant tests and checks.
7. Report modified files and test results.
8. Clearly explain any remaining issues.

Do not claim that a feature works unless it has been verified.

## 7. Important Restrictions

Never:

- Expose `.env`, passwords, API keys, or tokens.
- Perform destructive database operations without approval.
- Change the approved technology stack without permission.
- Change project requirements without approval.
- Delete existing project files without understanding their purpose.
- Commit or push changes without authorization.

## 8. Main Objective

Help the SI CDC UKRI development team build a secure, reliable, maintainable, and well-documented Career Development Center information system.

Always prioritize project requirements, existing code conventions, and team collaboration rules.
