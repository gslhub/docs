<div align="center">

# GSLHub Documentation

### Documentación técnica e institucional pública

**Arquitectura, mapa de repositorios, conceptos operativos públicos y estándares de documentación de GSLHub**

[English](./README.md) · **Español**

[Web](https://gslhub.com) · [Plataforma](https://github.com/gslhub/website) · [Investigación](https://github.com/gslhub/research) · [Organización](https://github.com/gslhub)

</div>

---

## Propósito

`gslhub/docs` es la capa pública de documentación de **GSLHub — Generative Search Lab Hub**.

Está diseñada para documentación que ayude a investigadores, desarrolladores, colaboradores y revisores a comprender el sistema **sin exponer credenciales, registros privados de investigación ni detalles innecesarios de infraestructura**.

## Fronteras documentales

GSLHub separa la documentación según su finalidad:

- [`gslhub/research`](https://github.com/gslhub/research) — metodología científica canónica, protocolos y codebooks;
- [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks) — especificaciones de benchmarks y métricas;
- `gslhub/datasets` — canal controlado de releases de datasets; permanece privado hasta que exista un dataset revisado listo;
- [`gslhub/software`](https://github.com/gslhub/software) — canal de software de investigación reutilizable;
- [`gslhub/website`](https://github.com/gslhub/website) — código fuente y documentación específica de la implementación;
- **`gslhub/docs`** — documentación técnica e institucional pública y transversal.

## Estructura prevista

```text
docs/
├── architecture/     # Arquitectura pública y límites del sistema
├── guides/           # Guías públicas para contribuidores/usuarios
├── governance/       # Gobernanza de documentación y releases
├── reference/        # Referencias estables entre repositorios
├── REPOSITORY-MAP.md
├── PUBLICATION-POLICY.md
└── README.md
```

## Referencias públicas iniciales

- [`REPOSITORY-MAP.md`](REPOSITORY-MAP.md) — dónde debe vivir cada tipo de material de GSLHub.
- [`architecture/OVERVIEW.md`](architecture/OVERVIEW.md) — arquitectura de alto nivel del sistema.
- [`PUBLICATION-POLICY.md`](PUBLICATION-POLICY.md) — reglas para decidir si una documentación operativa es segura para publicar.

## Principios de documentación pública

La documentación debe ser:

- exacta para la versión y contexto que describe;
- enlazada a fuentes canónicas en lugar de duplicada sin necesidad;
- explícita respecto a fronteras públicas/privadas;
- libre de credenciales y secretos;
- conservadora con rutas de host, identificadores internos y detalles operativos que no aportan valor científico;
- versionada cuando los cambios afectan a reproducibilidad o comportamiento de APIs públicas.

## Licencias

La documentación pública original de este repositorio se distribuye bajo **CC BY 4.0**, salvo que un archivo indique lo contrario. Los snippets de código copiados desde repositorios de software pueden mantener la licencia del repositorio de origen.

---

© 2026 GSLHub / Eduardo Yauri
