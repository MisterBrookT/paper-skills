# Integration Catalog

Paper Skills should curate before rebuilding. Candidate integration types:

- reference only: link to an external repo and document when to use it;
- vendored skill: copy compatible files with license and attribution;
- adapter: add a local wrapper that points an agent to an external skill;
- fork: maintain local changes when upstream does not match Paper Skills.

## Rules

- Check license before copying content.
- Preserve attribution.
- Prefer wrappers over copy-paste when upstream is active.
- Keep `plot` original and first-party.

## Initial Acknowledgement List

License data checked with GitHub on 2026-07-08. This table is for integration
planning only; re-check upstream licenses before copying or modifying files.

| Project | License | First Integration Mode | Notes |
| --- | --- | --- | --- |
| [`Yuan1z0825/nature-skills`](https://github.com/Yuan1z0825/nature-skills) | Apache-2.0 | adapter / reference | Strong Nature-style narrative and paper workflow signal. |
| [`Imbad0202/academic-research-skills`](https://github.com/Imbad0202/academic-research-skills) | Other | reference only until manual review | Full research-to-publication pipeline; license needs manual check. |
| [`Orchestra-Research/AI-Research-SKILLs`](https://github.com/Orchestra-Research/AI-Research-SKILLs) | MIT | adapter / reference | Broad AI research and engineering skill catalog. |
| [`Galaxy-Dawn/claude-scholar`](https://github.com/Galaxy-Dawn/claude-scholar) | MIT | adapter / reference | Research assistant workflow across coding, experiments, writing, publication. |
| [`google-deepmind/science-skills`](https://github.com/google-deepmind/science-skills) | Apache-2.0 | adapter / reference | Grounded science tooling and database integration patterns. |
| [`brycewang-stanford/Awesome-Journal-Skills`](https://github.com/brycewang-stanford/Awesome-Journal-Skills) | MIT | adapter / reference | Venue-pack demand signal across journals and disciplines. |
| [`Boom5426/Nature-Paper-Skills`](https://github.com/Boom5426/Nature-Paper-Skills) | MIT | adapter / reference | Nature-style manuscript lifecycle. |
| [`jaechang-hits/SciAgent-Skills`](https://github.com/jaechang-hits/SciAgent-Skills) | Other | reference only until manual review | Deep bioinformatics and life-science skill library. |
