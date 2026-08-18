# GSLHub Repository Map

GSLHub separates code, methodology, benchmarks, datasets, documentation and brand assets so that each has a clear canonical home and licensing model.

| Repository | Status | Canonical responsibility | Default/public license model |
|---|---|---|---|
| [`gslhub/website`](https://github.com/gslhub/website) | Public | Main research platform and website source code | AGPL-3.0-only |
| [`gslhub/research`](https://github.com/gslhub/research) | Public | Scientific methodology, protocols, codebooks and study definitions | CC BY 4.0 for original research documentation |
| [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks) | Public | Benchmark specifications, metric definitions and synthetic validation fixtures | CC BY 4.0 for original benchmark documentation |
| `gslhub/datasets` | Private until first reviewed release | Reviewed public dataset releases and provenance | Per dataset release |
| `gslhub/software` | Private; first standalone package validated for public release | Independently reusable research utilities and libraries | AGPL-3.0-only unless a package states otherwise |
| [`gslhub/docs`](https://github.com/gslhub/docs) | Public | Cross-project public technical/institutional documentation | CC BY 4.0 unless stated otherwise |
| [`gslhub/branding`](https://github.com/gslhub/branding) | Public | Approved visual identity and brand usage guidance | Brand/trademark terms; separate from software/research licenses |
| [`gslhub/.github`](https://github.com/gslhub/.github) | Public | Organization profile, contribution defaults, issue/PR templates and security policy | Organization governance files |

## Canonical-source rule

When a document moves to a specialized repository, avoid maintaining independent copies in multiple repositories. Prefer a stable pointer from the old location to the new canonical source.

This rule is already used for the Project Matrix, first pilot protocol and Observation/Citation Codebook, whose canonical versions live in `gslhub/research` while the `website` repository retains pointers for implementation context.

## Material placement

Use this decision order:

```text
Is it application/platform code?            → website
Is it reusable standalone research code?    → software
Is it scientific methodology/protocol?      → research
Is it a benchmark or metric specification?  → benchmarks
Is it a reviewed data release?              → datasets
Is it cross-project public documentation?   → docs
Is it logo/identity/brand guidance?          → branding
Is it organization-wide GitHub governance?  → .github
```

## Public/private boundary

A repository being part of the organization does not mean all of its internal or future content must be public. Publication follows the review policy appropriate to each material type.
