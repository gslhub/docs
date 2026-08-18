<div align="center">

# GSLHub Documentation

### Public technical and institutional documentation

**Architecture, repository map, public operating concepts and documentation standards for GSLHub**

**English** · [Español](./README.es.md)

[Website](https://gslhub.com) · [Platform](https://github.com/gslhub/website) · [Research](https://github.com/gslhub/research) · [Organization](https://github.com/gslhub)

</div>

---

## Purpose

`gslhub/docs` is the public documentation layer of **GSLHub — Generative Search Lab Hub**.

It is designed for documentation that helps researchers, developers, collaborators and reviewers understand the system **without exposing credentials, private research records or unnecessary infrastructure details**.

## Documentation boundaries

GSLHub separates documentation by purpose:

- [`gslhub/research`](https://github.com/gslhub/research) — canonical scientific methodology, protocols and codebooks;
- [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks) — benchmark and metric specifications;
- `gslhub/datasets` — controlled dataset-release channel; kept private until a reviewed dataset is ready;
- `gslhub/software` — reusable research-software channel; kept private until the first standalone tool is released;
- [`gslhub/website`](https://github.com/gslhub/website) — source code and implementation-specific documentation;
- **`gslhub/docs`** — cross-project public technical and institutional documentation.

## Planned structure

```text
docs/
├── architecture/     # Public architecture and system boundaries
├── guides/           # Public contributor/user guides
├── governance/       # Documentation and release governance
├── reference/        # Stable cross-repository references
├── REPOSITORY-MAP.md
├── PUBLICATION-POLICY.md
└── README.md
```

## Initial public references

- [`REPOSITORY-MAP.md`](REPOSITORY-MAP.md) — where each type of GSLHub material belongs.
- [`architecture/OVERVIEW.md`](architecture/OVERVIEW.md) — high-level system architecture.
- [`PUBLICATION-POLICY.md`](PUBLICATION-POLICY.md) — rules for deciding whether operational documentation is safe to publish.

## Public documentation principles

Documentation should be:

- accurate for the version/context it describes;
- linked to canonical sources rather than duplicated unnecessarily;
- explicit about public/private boundaries;
- free from credentials and secrets;
- conservative about host paths, internal identifiers and operational details that add no research value;
- versioned when changes affect reproducibility or public API behavior.

## Licensing

Original public documentation in this repository is licensed under **CC BY 4.0**, unless a file states otherwise. Code snippets copied from software repositories may remain under the software license of their source.

---

© 2026 GSLHub / Eduardo Yauri
