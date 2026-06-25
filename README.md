# Dataset Publishing Pipeline

Reproducible release pipeline for Make AI Visible research datasets.

This repository owns the steps that transform reviewed, anonymized, scored records into privacy-protected public dataset releases and accompanying metadata.

## MVP Scope

- Validate that only approved anonymized records enter a release.
- Aggregate or transform records according to the release policy.
- Apply publication thresholds and privacy checks.
- Generate metadata, changelogs, schema files, and dataset cards.
- Prepare release artifacts for GitHub, Hugging Face, Zenodo, or other approved hosts.

## Privacy Boundary

The publishing pipeline must fail closed when records are missing approval metadata, privacy checks, or schema validation.

## Suggested Stack

- Python CLI.
- JSON Schema or Pydantic validation.
- Reproducible release manifests.
- Synthetic sample datasets for tests.

## First Milestone

Create a local release builder that turns synthetic reviewed records into an aggregate dataset artifact plus a dataset card draft.
