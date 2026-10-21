# 0002 — Where logins and secrets are kept

**Date:** {{SETUP_DATE}}
**Decided by:** pending ({{OUR_APPROVER}})
**Status:** proposed (standing default from the client template)

## Context

We will hold client logins (hosting, domain, Google, site builders and similar). The team wants everything in one place. Plain-text passwords in Git are a risk: they stay in history forever, sit in every clone, and are read by every AI session that opens the repo.

## Options

1. **Shared password manager vault** (for example Bitwarden or 1Password, one "{{CLIENT_SHORT}}" vault). The repo records which logins exist and "kept in: {{CLIENT_SHORT}} vault". Recommended: simplest, revocable per person, nothing secret in Git.
2. **Encrypted file in the repo** (SOPS with age, or git-crypt). Secrets live next to the docs but are unreadable without a key held by the team.
3. **Plain text in the private repo.** Not recommended.

## Decision

Pending. Until decided, no plain-text secrets in the repo (see [AGENTS.md](../AGENTS.md#credentials)).
