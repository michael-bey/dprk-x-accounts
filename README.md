# DPRK X Accounts 🇰🇵

A community-maintained list of verified North Korean (DPRK) accounts on X (formerly Twitter).

## Purpose
This repository serves as the source of truth for the **DPRK Detector** project. It contains a curated list of social media accounts that are confirmed to be affiliated with, sympathetic to, or operated by the Democratic People's Republic of Korea (North Korea).

## Data Format
The data is stored in `accounts.json`. Each entry represents a single account:

```json
{
  "handle": "example_handle",
  "platform": "x",
  "full_url": "https://x.com/example_handle",
  "evidence_source": "kfa_website",
  "verification_status": "community_verified",
  "date_identified": "2023-01-01T00:00:00Z"
}
```

`statistics.total_accounts` counts entries in the `accounts` array only.

Accounts that are no longer on X are moved from `accounts` to `archived_accounts`. Archived entries keep the fields above and add `inactive_reason` (`not_found` or `suspended`) and `inactive_as_of`. They stay in this file so the tracking record is kept, and they are not part of the active list.

## Contributing
We welcome contributions from the OSINT community!

1.  **Fork** this repository.
2.  Add a new account to `accounts.json`.
    *   Ensure the `handle` is correct (no `@` symbol).
    *   Provide a valid `evidence_source` (e.g., link to official website, cross-reference).
3.  Submit a **Pull Request**.

## License
MIT
