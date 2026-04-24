# Token-Ignition Ledger

Public append-only ledger for `token-ignition`.

What lives here:

- `submissions/<submission_id>.json` — the canonical public record for each submission
- `submissions/index.json` — optional fast-path index for frontend polling

Design intent:

- no database
- every verdict is visible in git history
- frontend can poll this repo directly
- backend can append verdicts through the GitHub Contents API

This repository is meant to stay simple and machine-readable.
