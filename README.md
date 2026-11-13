# IT Work

Runbooks, scripts and queries from my day-to-day work as a systems administrator in a Microsoft 365, Entra ID and Intune environment.

Everything here is sanitized: no tenant IDs, domains, internal IP addresses, usernames, device names or ticket text.

## Layout

| Folder | Contents |
| --- | --- |
| `runbooks/` | One page per problem: symptom, cause, fix, how to verify |
| `scripts/` | PowerShell for Intune remediations and Microsoft 365 administration (added as written) |
| `kql/` | Defender Advanced Hunting queries, each with the question it answers (added as written) |

## Runbooks

See [`runbooks/`](runbooks/). New ones start from [`runbooks/TEMPLATE.md`](runbooks/TEMPLATE.md).

## Before committing

- [ ] No organization, tenant or domain names
- [ ] No internal IP addresses or hostnames
- [ ] No usernames, email addresses or device names
- [ ] No secrets, keys or connection strings
- [ ] Screenshots cropped or left out
