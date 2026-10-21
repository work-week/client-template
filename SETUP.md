# Setting up a new client from this template

This repository is a template. Each client gets its own copy. Follow these steps once, then **delete this file** in the same commit.

## 1. Make the client's repository

On GitHub, open `work-week/client-template` → **Use this template** → **Create a new repository**. Name it after the client (for example `work-week/ACME`) and keep it **private**.

## 2. Ask who you are working with

The team shares accounts. Before writing anything, the agent asks who it is talking to and uses that name as author and approver. See [AGENTS.md](AGENTS.md#who-you-are-working-with).

## 3. Fill in the placeholders

Every placeholder is in double curly braces. Replace all of them:

| Placeholder | Meaning | Example |
| --- | --- | --- |
| `{{CLIENT_NAME}}` | Client's full name | Acme Logistics, LLC |
| `{{CLIENT_SHORT}}` | Short name used across the files | Acme |
| `{{REPO}}` | This repository | work-week/ACME |
| `{{OUR_APPROVER}}` | Who approves changes on our side | a name |
| `{{CLIENT_APPROVER}}` | Who signs off for the client, and their role | a name and title |
| `{{SETUP_DATE}}` | The day you set this repository up | YYYY-MM-DD |

Find any left over:

```bash
grep -rn "{{" --exclude-dir=.git . | grep -v SETUP.md
```

## 4. Tailor it to the client

Every client has its own needs. The template stays neutral; you make it specific.

- **Client-facing changes** in [AGENTS.md](AGENTS.md#client-facing-changes): list the client's real properties (website, socials, listings, a product, whatever applies).
- **[map/accounts.md](map/accounts.md):** replace the example rows with the client's actual accounts.
- **[project/scope.md](project/scope.md)** and **[project/roadmap.md](project/roadmap.md):** what this engagement actually is.
- **Default decisions:** 0001 to 0003 apply to every client. Re-read them, then keep, adjust or supersede each. Number the client's own decisions from 0004.
- Add or remove folders only when the client needs it, and record why in a decision.

## 5. First session

Run the `session-log` skill to write the first log ("Knowledge base set up"), then commit and push. Delete this file in that commit.
