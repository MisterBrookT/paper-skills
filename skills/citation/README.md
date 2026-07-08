# Citation

Curated citation search, reference verification, DOI checks, and
reference-manager export skills.

Default strategy: integrate or reference strong public citation workflows before
rebuilding local versions.

## Scope

- check whether cited claims are supported by nearby references;
- detect missing, stale, or over-broad citations;
- verify DOI, title, venue, year, and author metadata;
- prepare export notes for BibTeX, CSL JSON, or reference managers.

## Demo Prompt

```text
Audit citations in this related-work section. For each citation, classify the
role, check whether the sentence overclaims, flag missing canonical work, and
return a table with risk level and suggested action.
```

## Integration Bias

Prefer existing search and reference-checking tools. Paper Skills should add
field-specific citation norms and paper-section context.
