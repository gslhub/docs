# GSLHub Architecture Overview

This document describes the **public architectural model** of GSLHub without exposing secrets or unnecessary deployment-specific details.

## System layers

```text
Public website / research dissemination
                │
                ▼
Research platform and governed operations
                │
        ┌───────┴────────┐
        ▼                ▼
 Structured research   Preserved research
 records / metadata    artifacts / evidence
        │                │
        └───────┬────────┘
                ▼
      Metrics and reproducibility
                │
                ▼
     Reviewed public outputs
```

## Main platform

The primary application lives in [`gslhub/website`](https://github.com/gslhub/website) and currently uses:

- Next.js;
- TypeScript / React;
- Payload CMS;
- MongoDB;
- Tailwind CSS;
- Node.js;
- GitHub Actions.

## Scientific separation

GSLHub deliberately separates:

1. **methodology** — protocols, codebooks and research governance in `gslhub/research`;
2. **execution infrastructure** — governed application logic in `gslhub/website`;
3. **benchmark specification** — metrics/evaluation in `gslhub/benchmarks`;
4. **data releases** — reviewed public datasets in `gslhub/datasets`;
5. **reusable tools** — independent utilities in `gslhub/software`.

This separation makes it possible to version a scientific method independently from the application implementation used to execute it.

## Provenance model

At a high level:

```text
Protocol / Benchmark
→ Experiment
→ Prompt Execution
→ Research Artifact
→ Evidence
→ Observation / Citation
→ Metric Result
→ Public Dataset / Publication
```

The exact governed model is documented in the canonical Project Matrix in [`gslhub/research`](https://github.com/gslhub/research/blob/main/methodology/PROJECT-MATRIX.md).

## Public/private boundary

The public architecture explains system responsibilities and reproducibility controls. It does not require publishing:

- credentials or environment secrets;
- private research records;
- restricted artifacts;
- private backup locations;
- unnecessary server/user identifiers;
- security-sensitive operational details.

## Reproducibility

Research reproducibility depends on the combination of versioned methodology, frozen execution context, preserved evidence, integrity checks, governed coding and versioned metric definitions—not on any one software component alone.
