<!-- 
1. Purpose

2. Branching Strategy

3. Branch Naming Convention

4. Commit Standards

5. Pull Request Standards

6. Release Strategy

7. Hotfix Strategy

8. Definition of Done

9. AI Requirements -->

# Purpose

Git is the single source of truth for all software changes.

The objective of this standard is to ensure:

* Traceability
* Consistency
* Collaboration
* Auditability
* Safe deployments

Every change must be represented through a clear Git workflow.


# Branching Strategy

The organization follows Git Flow.

Branches:

main

* Production environment

develop

* QA environment

feature/*

* New functionality

bugfix/*

* Non-production bug fixes

hotfix/*

* Production fixes

release/*

* Release preparation


# Branch Naming Convention

Format:

type/short-description

Examples:

feature/device-command-retry

feature/version-management

feature/device-bulk-actions

bugfix/device-status-sync

hotfix/mqtt-reconnection

release/v1.8.0


# Commit Standards

Use Conventional Commits.

Format:

<emoji> <type>(scope): description

Examples:

✨ feat(handler): add MQTT retry mechanism

🐛 fix(dispatcher): prevent duplicate command execution

♻️ refactor(backend): simplify device synchronization

📝 docs(playbook): update git standards

✅ test(handler): add MQTT integration tests

Preferred Emojis:

✨ feat     -> New feature
🐛 fix      -> Bug fix
♻️ refactor -> Code refactor
📝 docs     -> Documentation
✅ test     -> Tests
🚀 perf     -> Performance improvements
🔒 security -> Security improvements
🔥 remove   -> Remove code or features
⚙️ ci       -> CI/CD changes
⬆️ deps     -> Dependency upgrades


# Pull Request Standards

Every Pull Request must:

- Have a clear title
- Reference the related feature or issue
- Explain the purpose of the change
- Describe implementation details
- Describe testing performed

Pull Requests should remain focused on a single concern.

Avoid large Pull Requests whenever possible.

# Definition of Done

A task is considered complete when:

- Code is implemented
- Tests are passing
- Code review completed
- Documentation updated when necessary
- No critical issues remain
- Branch merged successfully

Done does not mean code exists.

Done means the change is production-ready.


# Hotfix Strategy

Hotfixes are reserved for production issues.

Flow:

hotfix/*
↓
main
↓
develop

Every hotfix must:

- Identify root cause
- Include validation steps
- Be merged back into develop

Avoid using hotfixes for unfinished work.


# Release Strategy

Releases are managed through Semantic Versioning and Git Tags.

Format:

vMAJOR.MINOR.PATCH

Examples:

v1.0.0
v1.2.0
v1.2.5

Pre-release environments may use suffixes:

v1.0.0-qa
v1.2.0-qa

Guidelines:

- MAJOR for breaking changes
- MINOR for new features
- PATCH for bug fixes

Environment deployments should be triggered from Git Tags.

Examples:

v1.2.0-qa -> QA Deployment

v1.2.0 -> Production Deployment

Tags represent the official release history and deployment traceability.


# AI Requirements

When proposing changes, always provide:

* Feature Name
* Branch Name
* Commit Message
* Pull Request Title

Examples:

Feature:
device-command-retry

Branch:
feature/device-command-retry

Commit:
✨ feat(handler): add MQTT retry mechanism

Pull Request:
feat: implement MQTT retry workflow
