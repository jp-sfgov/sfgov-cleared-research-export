# SFGOV Cleared Research Export

**Everything committed to this repository is publicly disclosed.** Do not commit anything here that Jeremy Pollock has not explicitly cleared for public release.

## What belongs here

Only self-contained research packets that Jeremy has reviewed and cleared for public disclosure. A packet must record:

- Clearance date
- Public sources (with links)
- Source commit (from the originating private repository)
- Intended destination (where or how this will be used or published)
- Exclusions (what was deliberately left out, and why)
- Unresolved caveats (open questions, unverified claims, pending corrections)

See `PACKET_TEMPLATE.md` for the required shape.

## What never belongs here

- Raw City files or verbatim City-authored documents
- Intake material: newsletters, weekly registers, daily-intel briefs, scratchpads, source queues, session transcripts
- Session-state files or agent-instruction files
- Credentials, tokens, or account/access details
- Private identifiers (names, contact information, internal usernames) not already public
- Level 3–5 City data
- Private operating context (personal runtime, device, provider, spend, cron, or local-path details)
- Git history from any source repository — packets are authored fresh, not copied with history

## Provenance

This repository receives content only in the personal → work → public direction, from packets reviewed against the private work repositories `jp-sfgov/sfgov-models-and-harnesses` and `jp-sfgov/sfgov-ccsf-compute`. It does not receive direct pushes carrying those repositories' history, and content flowing the other direction (public → private, or City → personal) is out of scope here entirely.
