---
{"dg-publish":true,"permalink":"/fs-business-and-product/ogsm-and-roadmap-templates-project-context/","title":"OGSM and Roadmap Templates - Project Context","tags":["Work","ProductManagement","Confluence","OGSM","Roadmap"],"dg-note-properties":{"title":"OGSM and Roadmap Templates - Project Context","date":"2026-07-14","tags":["Work","ProductManagement","Confluence","OGSM","Roadmap"]}}
---


## Purpose

Working notes for the Cowork project "Confluence: Team OGSM and Roadmap." Keeping this here so the context survives a machine switch (the Cowork project itself is local to one machine).

## Project Goal

Build/edit a series of Confluence pages — likely to become templates — so PMs in my group have a uniform approach to:

1. Capturing and communicating **Outcomes, Goals, Strategies, Measures (OGSM)**
2. Sharing a **short-term roadmap** with stakeholders

## Background

- No prior draft of an OGSM/roadmap strategy doc was found in this vault (checked 2026-07-14).
- Related reference material already in the vault:
	- `PM-Learning/PlayingToWin/OGSM-Sample.md` — pointer to an OGSM sample PDF (Playing to Win)
	- `PM-Learning/PdM Process Notebook/Why Most Outcome Based Roadmaps Fail (and How to Prevent it).md`
	- `PM-Learning/PdM Process Notebook/Strategic Roadmaps.md`
	- `PM-Learning/Product-Talk/Teressa Torres - Product Roadmaps How the Best Product Teams Plan for Uncertainty.md`
	- `FS-Business-and-Product/Group Product Manager - Current Focus.md` — lists "Roadmaps / Plans" as a needed report type

## Frameworks & Where to Find Them

Don't load this material into context by default — pull specific files only when actively working on the relevant template.

**OGSM** — from *Playing to Win* by A.G. Lafley and Roger Martin.
- Vault: `PM-Learning/PlayingToWin/OGSM-Sample.md` (and `_resources/OGSM-Sample.pdf`)
- `~/Dev/pm-learning`: no dedicated notes yet — *Playing to Win* is only on the to-read list (`reading-notes/pm-reading-list.md`, tagged "Strategic choice cascade"). Nothing to pull from here until it's actually read/summarized.

**Roadmaps** — from Teressa Torres, "Product Roadmaps: How the Best Product Teams Plan for Uncertainty."
- Vault: `PM-Learning/Product-Talk/Teressa Torres - Product Roadmaps How the Best Product Teams Plan for Uncertainty.md` — read in full 2026-07-14; summary below for quick reference, but reread the article itself when actually designing the roadmap template.
- Also relevant: `PM-Learning/PdM Process Notebook/Why Most Outcome Based Roadmaps Fail (and How to Prevent it).md`, `PM-Learning/PdM Process Notebook/Strategic Roadmaps.md`
- `~/Dev/pm-learning`: no notes on the specific roadmap article, but deep Torres material exists on her adjacent *Continuous Discovery Habits* framework (outcomes, opportunity solution trees) — useful for the "Outcomes" thinking behind OGSM/roadmap work:
	- `knowledge-base/frameworks/continuous-discovery-habits.md` — primary reference, updated 2026-04-08
	- `knowledge-base/frameworks/Fundamentals/` — supplementary worked examples from her Product Discovery Fundamentals course (see `Fundamentals/README.md` for index)

**Summary — Torres roadmap article:** She walks through four roadmap formats in order of maturity: feature roadmaps (features + dates — calls these "fiction," avoid), theme roadmaps (strategic focus areas, but sales/marketing lose visibility), outcome-based roadmaps (add a measurable metric per theme, same visibility problem), and Now/Next/Later. Her recommended format is a Now/Next/Later grid tied to an opportunity solution tree, where content type changes per column: **Now** = solutions currently in flight (fully spec'd, can carry a date), **Next** = opportunities being explored (no committed solution yet), **Later** = outcomes the team is driving toward (directional only, no commitment). Certainty decreases left to right by design. Transition advice for orgs still on feature roadmaps: don't fight it outright, start attaching the opportunity/outcome behind each feature, then evolve the Now column first. Her Now/Next/Later + opportunity/outcome structure maps naturally onto OGSM (outcomes/opportunities ≈ Outcomes/Goals) and is a strong candidate basis for our roadmap template.

## Deliverables (evolving)

- [ ] Confluence template: OGSM page (Outcomes, Goals, Strategies, Measures)
- [ ] Confluence template: short-term roadmap page for stakeholders
- [ ] Guidance/instructions for PMs on how to fill these out consistently

## Decisions Log

> Only entries Gregg explicitly marks as a decision go here — proposals, drafts, and discussion points don't count until flagged as such.

- 2026-07-14: Started this context doc after confirming no existing draft existed in the vault.

## Open Questions

- What time horizon counts as "short-term" for the roadmap template?
- Should OGSM and roadmap live as one page or two linked pages?
- Which Confluence space/parent page should these templates live under?

## Next Steps

- Define the OGSM template structure and fields.
- Define the roadmap template structure and fields.
- Draft both in Confluence, then convert to Confluence templates once approved.

## Update 2026-10-01 — scope reset to five team templates

Gregg's revised model (after counsel with the SOC): SOC vision/strategy/annual product strategy + SOC quarterly report (John Alexander's template 02 in `~/Dev/product-strategy/templates/`) sit above five **team-level** Confluence templates. The roadmap template from the July scope is dropped.

1. **Team Outcome page** (OGSM equivalent) — product outcome, goal "move X to Y by date", key measures with links to instruments, ≤5 strategies; changes only when the outcome is renegotiated (Torres).
2. **Monthly Business Retrospective** — Gregg's four questions (progress, what we did, what we learned, what's next).
3. **Quarterly Business Review** — mirrors `OneDrive/QBR/MTE_SOC/Official QBR Template.pptx` (goals w/ COMPLETE/PARTIAL/CANCELLED + planned/actual effort; learnings → "therefore what"; key metrics; up to 5 proposed goals).
4. **Test Card** and 5. **Learning Card** — Strategyzer (source PDFs: `PM-Learning/Strategyzer/_resources/Testing_Tools_and_Other_Resources.resources/`).

Drafts: [[FS-Business-and-Product/Team Outcome Templates - Drafts/01-team-outcome-page\|folder: Team Outcome Templates - Drafts]].

**Open decisions (awaiting Gregg):**
- Where in Confluence (proposed: copyable template pages under the MTE SOC area of the Product space; the connector can't create real space templates, so a space admin would paste them in).
- Page Properties on the Team Outcome page + a hub Page Properties Report rolling up all teams?
- Also add as team-level templates 05–09 in `product-strategy/templates/` (README asks for a `[Proposal]` issue to John first)?
- Keep or cut the "Persevere / Adjust / Stop" line added to the monthly retro.

## Update 2026-10-02 — decisions made, pages live in Confluence

Gregg's decisions: (1) copyable template pages under MTE SOC in the Product space; (2) yes to Page Properties + a hub roll-up report; (3) repo copy in `product-strategy/templates/` **later**, after teams have used them, then a `[Proposal]` issue to John Alexander; (4) keep the Persevere / Adjust / Stop line.

Created 2026-10-02 (Product space, under MTE SOC 2557181997):
- Hub: **MTE SOC Team Outcomes** — 2681831599. Page Properties Report (CQL `label = "mte-team-outcome"`; columns CFT, PM, Goal, Current, Target, Status), "how the pieces fit" table, how-to, children list.
- Template 1 — Team Outcome Page — 2681995415 (Page Properties block: Team, CFT, PM, Trio, Goal, Current, Target, Status, Outcome negotiated, Next review)
- Template 2 — Monthly Business Retrospective — 2682454110
- Template 3 — Quarterly Business Review — 2682585154
- Template 4 — Test Card — 2682388553
- Template 5 — Learning Card — 2681831626

Teams copy a template; only the Team Outcome copy gets the `mte-team-outcome` label (the template itself must NOT, or it shows in the report). The connector can't set labels. Confluence pages are now the source; the drafts folder is historical.

The process itself (how the templates fit and how teams run it) is documented in [[FS-Business-and-Product/MTE Team Outcome Process\|MTE Team Outcome Process]].
