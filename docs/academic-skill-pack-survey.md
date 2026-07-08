# Academic Skill Pack Survey

Date: 2026-07-08

## Summary

Academic skill packs are already crowded. The strongest public projects cover
research-to-publication workflows, journal-specific packs, and domain-specific
science tooling. Paper Skills should not compete by rebuilding every writing or
citation skill from scratch.

Best wedge:

```text
curated academic skill hub + original discipline-aware plot skill
```

## Key Projects

| Project | Stars | What It Covers | Lesson for Paper Skills |
| --- | ---: | --- | --- |
| Yuan1z0825/nature-skills | 26,941 | Nature-style research workflows, writing, figures, reader, response, citation, search | Strong name and strong pain point. Front-load narrative, demos, and install paths. |
| imbad0202/academic-research-skills | 36,796 | research -> write -> review -> revise -> finalize | Full academic pipeline already exists. Avoid generic pipeline clone. |
| Orchestra-Research/AI-Research-SKILLs | 10,492 | AI research and engineering skill categories | Broad skill libraries need catalog discipline. |
| Galaxy-Dawn/claude-scholar | 4,533 | semi-automated research assistant skills | Scholar naming space is crowded. |
| google-deepmind/science-skills | 2,280 | grounded scientific workflows and database/tool integration | Science name taken; strong institutional signal. Compete by field-expression layer, not brand scale. |
| brycewang-stanford/Awesome-Journal-Skills | 708 | journal-specific packs across many venues | Venue packs are real demand. Paper Skills can curate or interoperate. |
| Boom5426/Nature-Paper-Skills | 346 | Nature-style manuscript lifecycle | More proof that Nature naming pulls attention. |
| jaechang-hits/SciAgent-Skills | 227 | bioinformatics and life-science skills | Deep domain packs work when the user group is explicit. |
| lishix520/academic-paper-skills | n/a | planning and writing academic papers | Paper Skills name has neighbors; differentiate with plot and curation. |
| diggerdu/paper-skills | 1 | LaTeX paper workflow checks | Name collision exists but weak. Use stronger subtitle and owner identity. |

## Strategic Read

1. `Paper Skills` is viable if the subtitle carries the aspiration:
   `Journal-ready AI skills for every research discipline`.
2. `plot` should be first-party and prominent. It gives Paper Skills a real
   technical claim.
3. Writing, citation, review, and venue packs should start as curated wrappers.
4. Per-discipline expression is the product insight: each field has its own
   writing, figure, evidence, and review language.
5. Non-CS users need a later platform surface, likely `Paper Studio`, but the
   repo should stay skill-first.

## Recommended Initial Structure

```text
paper-skills
  skills/plot
  skills/writing
  skills/citation
  skills/review
  skills/venue-packs
  integrations/catalog.md
  registry.yaml
```

## Near-Term Next Steps

1. Keep the integration catalog current with license status and attribution
   notes.
2. Fill `skills/plot` with the circuit seed-bench workflow.
3. Create integration notes for 5-8 upstream projects with license status.
4. Add one demo prompt per skill entry.
5. Decide whether public-facing site is `Paper Skills` or `Paper Studio`.
