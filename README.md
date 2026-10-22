# Onboarding Snapshot

Day-one account snapshot for the GitHub account `HeziLiu`. Everything here is
meant to be read on day one by a new platform engineer, with no other context
required.

## What's in data/

- `data/profile.md` — profile facts for the account (login, numeric user ID,
  display name and counts), exactly as returned by the live lookup.
- `data/starred.md` — the repositories the account has starred, as `owner/name`.
- `data/teams.md` — the organization teams the account belongs to.
- `data/first-issues.md` — for each starred repository that was checked, a
  suggested open "good first issue", or an explicit note that none was found.

## Integrity

`MANIFEST.txt` lists each file above with its SHA-256 checksum, computed over
the exact bytes committed to this branch. Verify locally with:

    sha256sum -c MANIFEST.txt

All account data in `data/` was pulled live from the GitHub API when this
snapshot was created; nothing was guessed or hand-copied.
