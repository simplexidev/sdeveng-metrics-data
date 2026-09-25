# Metrics data development

This repository owns reviewed, sanitized, versioned aggregate data for
`simplexidev/sdeveng`. Commit publishable data only under `public/`, list every JSON
artifact in `public/publication-manifest.json`, and preserve historical aggregates.

Raw runs, prompts, responses, transcripts, private source, logs, local paths, secrets,
and identifying data must never be committed. `private/` is policy-only local staging.
Validation and publication code belongs in `simplexidev/sdeveng-metrics-tooling`; static
presentation belongs in `simplexidev/sdeveng-metrics-dashboard`.

Before merging, run the tooling publisher against this repository and the dashboard so
schema, approval, allowlist, and publication-safety checks all pass.
