# Estructura del repositorio

## Árbol de carpetas
```text
.
├── README.md
├── docs/
│   ├── propuesta.md
│   ├── caso_de_uso.md
│   ├── estructura_repositorio.md
│   ├── plan_de_pruebas.md
│   └── reflexion_ia.md
├── src/
│   └── main.s
├── scripts/
│   └── run.sh
└── tests/
    └── casos_manual.md
```

## Descripción de archivos clave
- `src/main.s`: núcleo del microproyecto en ARM64 Assembly, incluye macro funcional y flujo principal.
- `scripts/run.sh`: automatiza ensamblado, enlazado y ejecución básica en entorno local.
- `tests/casos_manual.md`: bitácora breve para anotar resultados observados por caso.
- `docs/*.md`: evidencia técnica para evaluación por competencias.

## Convenciones de nombres
- Archivos en minúsculas con guion bajo: `caso_de_uso.md`.
- Nombres descriptivos y estables para facilitar rúbrica.
- En Assembly, etiquetas cortas y semánticas: `validar`, `convertir`, `mostrar_resultado`.
- Macro en mayúsculas para distinguirla de rutinas: `PRINT`.

## Versionado simple
- Se recomienda versionado académico por hitos:
  - `v0.1-propuesta` (documentación inicial),
  - `v0.2-ensamblado_base` (entrada/salida con macro),
  - `v1.0-entrega` (funcionalidad + pruebas completas).
- Commits con prefijos sugeridos: `docs:`, `asm:`, `test:`.
