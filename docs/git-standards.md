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
