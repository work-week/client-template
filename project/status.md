# Status

Last updated: {{SETUP_DATE}}.

Newest items at the top of each list. Tick items off (`[x]`) and add the date; never delete them.

## Timeline

Estimates. Adjust as the client answers come in. Replace the example tasks with this engagement's real phases.

```mermaid
gantt
    title {{CLIENT_SHORT}} phase 1 (estimate)
    dateFormat YYYY-MM-DD
    axisFormat %b %d
    section Discovery
    Knowledge base set up             :active,  d1, {{SETUP_DATE}}, 1d
    Discovery with the client         :         d2, after d1, 7d
    section Plan
    Scope and plan                    :         p1, after d2, 7d
    section Deliver
    First deliverable                 :         b1, after p1, 14d
```

## Checklist

### To do

- [ ] Fill in [project/scope.md](scope.md) with what this engagement is
- [ ] Discovery: who the client is, who buys from them, what hurts ([open questions](open-questions.md))
- [ ] List the client's accounts and properties in [map/accounts.md](../map/accounts.md)
- [ ] Decide where logins are kept ([decision 0002](../decisions/0002-credentials.md))

### Done

- [x] {{SETUP_DATE}} Knowledge base set up from the client template
