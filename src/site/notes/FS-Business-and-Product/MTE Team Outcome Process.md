---
{"dg-publish":true,"permalink":"/fs-business-and-product/mte-team-outcome-process/","title":"MTE Team Outcome Process","tags":["Work","ProductManagement","Confluence","MTE-SOC","Outcomes"],"dg-note-properties":{"title":"MTE Team Outcome Process","date":"2026-10-02","tags":["Work","ProductManagement","Confluence","MTE-SOC","Outcomes"]}}
---


# MTE Team Outcome Process

How each Member Temple Experience SOC team ties its work to a product outcome, reports progress, and learns from experiments. Set up 2026-10-02. **The Confluence pages are the source of truth**; this note explains the approach and why it is shaped this way.

## The model

The process combines three frameworks:

- **Teresa Torres (Continuous Discovery):** each team owns one *product outcome*, a change in customer behavior it can directly influence. That outcome is a leading indicator expected to predict a SOC business metric. The outcome is negotiated with the SOC and changes only when renegotiated, not every quarter.
- **Roger Martin / OGSM:** the Team Outcome page is the team's OGSM equivalent: outcome, a goal in the form "move X to Y by date," measures with instruments, and five strategies at most.
- **Strategyzer (Testing Business Ideas):** experiments are framed before they run (Test Card) and closed out with an explicit decision (Learning Card).

## How it fits under the SOC

```
SOC vision → 2027 MTE SOC Product Strategy (objectives, business outcomes, main metrics)
   └─ SOC quarterly report (John Alexander's template 02, product-strategy repo)
        └─ Team level (this process)
             Team Outcome page ← Monthly retros ← Test / Learning Cards
                     └─ Quarterly Business Review → feeds SOC quarterly report
```

A team's "control" is the leading indicator shown (or still assumed) to predict the SOC's lagging metric. Initiatives are the levers the team pulls to move that leading indicator. See [[FS-Business-and-Product/Poloski MTE Deck vs 2027 Strategy - Comparison In Progress\|Poloski MTE Deck vs 2027 Strategy - Comparison In Progress]].

## The five artifacts

| Artifact | When | Purpose |
|---|---|---|
| **Team Outcome page** | Created once; changes only on renegotiation. Current and Status are updated monthly. | One page: why this outcome, the goal, key measures (leading, lagging, guardrail) each linked to an instrument, up to five strategies, active experiments, outcome history. |
| **Monthly Business Retrospective** | Monthly, separate from the SDLC sprint retro | Four questions: What measurable progress did we make? What did we do to move the needle? What did we learn? What will we do next month? Ends with a strategy decision: **Persevere / Adjust / Stop**. |
| **Quarterly Business Review** | Quarterly | Mirrors the Official QBR Template deck (`OneDrive/QBR/MTE_SOC/Official QBR Template.pptx`): goals marked COMPLETE / PARTIAL / CANCELLED with planned vs. actual effort; learnings → "therefore what"; key metric charts against the target; up to five proposed goals, with the outcome goal first. Built from the quarter's three monthly retros. Feeds the SOC quarterly report. |
| **Test Card** | Before each experiment | Hypothesis, test, metric, criteria. **All four, including the success criteria, are written before the test starts.** Also covers risk type (desirability / feasibility / viability), cost and reliability. |
| **Learning Card** | When each experiment ends | Hypothesis (copied unchanged), what we observed, what we learned, a decision (new hypothesis / keep testing / update strategy / stop), and a link to what comes next. |

## Operating rhythm

1. **Negotiate the outcome** with the SOC lead → fill in the Team Outcome page and label it.
2. **Run experiments** with a Test Card before and a Learning Card after. Link them from the Team Outcome page's Active experiments line.
3. **Each month**, hold the business retro, which links its Test and Learning Cards. Afterward, update Current and Status on the Team Outcome page so the SOC roll-up stays current.
4. **Each quarter**, build the QBR from the three monthly retros. Proposed goals for the next quarter go back to the SOC for agreement.
5. **If the outcome is renegotiated**, add a row to Outcome history on the Team Outcome page and change the goal. Don't create a new page.

## Where it lives in Confluence

Product space → MTE SOC (2557181997) → **[MTE SOC Team Outcomes](https://icseng.atlassian.net/wiki/spaces/Product/pages/2681831599)** (2681831599)

| Page | ID |
|---|---|
| Template 1 — Team Outcome Page | 2681995415 |
| Template 2 — Monthly Business Retrospective | 2682454110 |
| Template 3 — Quarterly Business Review | 2682585154 |
| Template 4 — Test Card | 2682388553 |
| Template 5 — Learning Card | 2681831626 |

**How teams use them:** open a template → ••• → Copy → put it in the team's own area → rename it and replace the bracketed placeholders → delete the italic guidance lines.

## The roll-up

- The hub page has a **Page Properties Report** that pulls from every page labeled `mte-team-outcome` and shows CFT, PM, Goal, Current, Target and Status.
- Each Team Outcome page has a **Page Properties** block at the top (Team, CFT, PM, Trio, Goal, Current, Target, Status, Outcome negotiated, Next review). The report reads that block.
- **Only team copies get the label.** The template itself must not carry it, or it shows up in the report as if it were a team.
- If a report column comes up blank, the heading in the team's Page Properties block probably doesn't match exactly (for example, someone renamed "Current"). The report matches headings by name.

## Design choices and why

- **Copyable pages, not Confluence space templates.** The Atlassian connector can't create real space templates. A space admin could promote these later without changing the content.
- **Short pages.** Each page answers one question, and the pages link to each other instead of restating content. This follows Gregg's preference for compact Confluence pages.
- **At most five strategies and five proposed goals,** in line with Ryan Parker's limit of five items per strategy group.
- **Every measure links to an instrument.** If none exists yet, the page names who is building it and by when, so no measure goes untracked without anyone noticing.
- **Success criteria are set before the test runs,** so no one can move the goalposts after seeing the data.
- **The monthly retro is not the sprint retro.** It's about outcome movement, not delivery process.
- **The July OGSM + roadmap scope was dropped.** No roadmap template; strategies and experiments do that job. History: [[FS-Business-and-Product/OGSM and Roadmap Templates - Project Context\|OGSM and Roadmap Templates - Project Context]].

## Changing the templates

- Edit the Confluence template pages directly. Changes don't reach copies teams have already made, so tell the PMs when a template changes.
- If you change a Page Properties heading on Template 1, also update the `headings` list in the hub's report and ask teams to rename the heading on their own copies.
- The drafts in [[FS-Business-and-Product/Team Outcome Templates - Drafts/01-team-outcome-page\|Team Outcome Templates - Drafts]] are historical and no longer kept in sync.

## Next steps

- [ ] Roll the process out to the PMs. Staff meeting is the first audience.
- [ ] Watch the first teams' Team Outcome pages show up in the hub report.
- [ ] After teams have used the templates for a cycle, open a `[Proposal]` issue to John Alexander to add them as team-level templates in `product-strategy/templates/` (05–09).
- [ ] Optional: ask a Product space admin to promote the five pages to real space templates.

## Sources

- Strategyzer Test and Learning Card PDFs: `PM-Learning/Strategyzer/_resources/Testing_Tools_and_Other_Resources.resources/`
- Product Talk / Continuous Discovery: `PM-Learning/Product-Talk/`
- [[FS-Business-and-Product/Member Temple Experience SOC and Strategy\|Member Temple Experience SOC and Strategy]] · [[FS-Business-and-Product/Presenting to Strategic Objective Council (SOC)\|Presenting to Strategic Objective Council (SOC)]]
