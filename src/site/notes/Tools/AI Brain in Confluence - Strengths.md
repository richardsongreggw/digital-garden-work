---
{"dg-publish":true,"permalink":"/tools/ai-brain-in-confluence-strengths/","title":"AI Brain in Confluence - Strengths","tags":["Work","Ai","Confluence"],"dg-note-properties":{"title":"AI Brain in Confluence - Strengths","date":"2026-07-16","tags":["Work","Ai","Confluence"]}}
---


Reasons Confluence is a strong location for an AI brain (recaptured after the original note, written 2026-07-15, was lost before it synced).

- We already have an instance.
- It has an MCP, works great with Claude, and has Rovo built in.
- It's also good for low-tech humans and business stakeholders, especially those who are laggards in adopting agents.
- Naturally integrates with Jira; we're getting better at integrating with Pilot.
- Built-in browsing.
- Built-in searching.
- Built-in permissions.
- Offers a way to watch for and get notified of content changes and updates.
- Has version history and the ability to revert. However, we'll need to add some diligence through process (as outlined below)
- Commenting capabilities.
- Easy to share a link with others.
- When you move a page using the Move function, all internal links pointing to that page are updated automatically.
- Live co-editing, enhancing collaboration.  However, this presents some risks (as outlined below).
- Page-level analytics.

## Confluence vs. GitHub for the AI brain (compare/contrast)

A peer is proposing GitHub instead. Assessment of both, added 2026-07-16.

**Case for Confluence** (in addition to the strengths above):

- It's where the non-product engineering org already lives — SOC leads, marketing, operations, Support, etc. A GitHub repo is a real adoption barrier for exactly the "low-tech humans and business stakeholders" this brain needs to serve; almost nobody outside engineering opens PRs comfortably.
- Permissions, spaces, and page hierarchy already map cleanly onto the Product / Teams / Disciplines (/ Governance) axes being proposed — no access-control model needs to be rebuilt.
- Comments and watch/notify are standing, page-level, and persistent — not transient like PR comment threads.
- It's the single canonical surface the org is actively trying to consolidate onto (see IA proposals below). Standing up GitHub as an "AI brain" would recreate the exact multi-surface problem (Confluence + legacy fhconfluence + SharePoint) those proposals are trying to eliminate — just with a fourth surface instead of fewer.

**Case for GitHub**:

- Native version control: real diffs, PR review before changes go live, branching for drafts. Confluence's live co-editing means bad edits go live immediately unless draft/status discipline is manually enforced.
- Plain markdown files on a filesystem are what Claude Code (and the Teresa Torres pattern this is modeled on) works with most naturally — no MCP/API layer required, agents can just read/write/grep files directly.
- An automatic checker can inspect every proposed change before it's allowed to go live — e.g. "did you fill in the required fields," "does this match the expected format" — and bounce it back if not, with no human having to catch the mistake by hand. Confluence's flexibility is part of why the current `Product` space rotted into "kitchen sinks" and "stale corpses" in the first place.
- Fully portable, and searchable with simple, everyday tools — no special app or website login required, since the files are just plain text rather than locked inside a vendor's database.

**My take:** GitHub wins on engineering-native workflow (easy-to-read change history, a review step before changes go live, automatic rule-checking) and is the closer match to Torres's original setup. Confluence wins on organizational reach — it's usable by everyone the brain needs to serve, not just engineers, and it avoids adding a fourth knowledge surface to an org that's actively trying to reduce to one. Given the audience for this brain is the whole product org and not just engineering, Confluence's reach probably outweighs GitHub's workflow advantages — but the Confluence gaps below are real and worth a mitigation plan rather than hand-waving away.

### Closing the Confluence gaps

| Gap                        | Plain-English problem                                                                                                                                                     | Confluence fix                                                                                                                                         |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Hard to see what changed   | No easy side-by-side view of exactly what got added or removed                                                                                                            | Page History → Compare Versions, plus requiring a short "what changed" note on every save                                                              |
| No automatic rule-checking | Nothing automatically checks a page has the required fields/format before it's saved — GitHub can auto-inspect every change and bounce back anything that doesn't qualify | Page templates lock in required fields (owner, curator, status, last-reviewed); Claude/Rovo runs periodic sweeps and flags gaps                        |
| Live-edit risk             | Changes go live instantly, no sign-off                                                                                                                                    | Restrict direct editing to owners/curators; everyone else comments/suggests; curator gets a watch notification and can revert fast via version history |

## Related: Confluence IA proposals (John Alexander)

John has been developing how this would actually be structured in Confluence:

- [Two-Space Hybrid IA — Proposal v0.1 (Draft)](https://icseng.atlassian.net/wiki/spaces/Product/pages/2258043036/Two-Space+Hybrid+IA+Proposal+v0.1+Draft) — original draft: `Product` space (by product) + `Teams` space (by SOC → team).
- [Confluence IA Proposal — Three-Space Hybrid Model](https://icseng.atlassian.net/wiki/spaces/KS/pages/2401992775/Confluence+IA+Proposal+Three-Space+Hybrid+Model) — current draft (v0.2), adds a `Disciplines` space (by practice: PM, Program Management, Engineering, SDET, UX, etc.), owned by chapter leads.

My own read: a fourth peer space, **Governance and Controls**, for shared processes/practices (risk, security & access, change & release, SDLC, AI governance, vendor management, etc.) — see the existing [Governance space](https://icseng.atlassian.net/wiki/spaces/Governance/overview), which already covers this ground but isn't yet integrated into John's model as a peer axis alongside Product / Teams / Disciplines.
