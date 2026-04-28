# Actividad: Propuesta de Práctica Temática (Enfoque en Documentación)

## 1) Título de la práctica

**Diseño de Mini Práctica Temática para Sistemas (Documentación Primero)**

> Ejemplos de tema (elige uno o propón otro similar):
> - “Mini Toolkit en ARM64”
> - “Asistente de Estudio en Terminal”
> - “Reporteador de Información del Sistema”
> - “Organizador de Archivos”
> - “Juego de Aprendizaje en Línea de Comandos”

---

## 2) Descripción general

En esta actividad **no vas a construir un proyecto grande**, sino a diseñar una **propuesta sólida y bien documentada** para una práctica temática pequeña que pueda desarrollarse de forma realista en este curso.

Tu propuesta debe centrarse en:
- definir claramente el problema o necesidad,
- justificar por qué vale la pena resolverlo,
- planear la estructura del repositorio,
- y describir cómo validarías su funcionamiento.

Debes elegir **un solo lenguaje principal** para tu práctica:
- ARM64 Assembly
- C
- Python
- Bash

> **Nota importante sobre ARM64 Assembly:** úsalo únicamente para programas **muy pequeños** (por ejemplo, utilidades de consola sencillas, operaciones básicas o flujos cortos). No se recomienda para propuestas grandes en esta actividad.

### Enfoque de la tarea
Primero documentación y planeación, después código mínimo (si aplica). La calidad de tu propuesta pesa más que la cantidad de código.

---

## 3) Entregables del estudiante

Tu repositorio debe incluir, como mínimo, los siguientes archivos:

- `README.md`
- `docs/propuesta.md`
- `docs/caso_de_uso.md`
- `docs/estructura_repositorio.md`
- `docs/plan_de_pruebas.md`

Opcionales:
- `src/`
- `scripts/`
- `tests/`

---

## 4) Estructura recomendada del repositorio

Usa esta base mínima:

```text
nombre-del-proyecto/
├── README.md
├── docs/
│   ├── propuesta.md
│   ├── caso_de_uso.md
│   ├── estructura_repositorio.md
│   └── plan_de_pruebas.md
├── src/
│   └── main.<ext>
├── scripts/
│   └── run.sh
└── tests/
    └── test_plan.md
```

---

## 5) Instrucciones de contenido por archivo

### `README.md`
Debe incluir:
1. Nombre del proyecto.
2. Lenguaje principal elegido.
3. Resumen breve (5–8 líneas).
4. Objetivo general.
5. Cómo se organiza el repositorio.
6. Estado del proyecto: “Propuesta inicial” o “Prototipo mínimo”.

---

### `docs/propuesta.md`
Debe responder de forma concreta:
1. **Tema y contexto**: ¿qué problema pequeño atiende?
2. **Objetivo técnico**: ¿qué hará el programa exactamente?
3. **Alcance acotado** (qué sí incluye y qué no incluye).
4. **Lenguaje elegido y justificación**.
5. **Viabilidad**: por qué puede hacerse en pequeño tiempo y con herramientas gratuitas.
6. **Entregable funcional mínimo (MVP)**: describe la versión más pequeña útil.

Incluye al final una sección: **“Riesgos y mitigaciones”** (mínimo 3 riesgos).

---

### `docs/caso_de_uso.md`
Incluye:
1. Nombre del caso de uso.
2. Actor principal (usuario).
3. Precondiciones.
4. Flujo principal paso a paso.
5. Flujos alternos (errores o entradas inválidas).
6. Resultado esperado.

Agrega una tabla de **3 escenarios de ejemplo** con columnas:
- Entrada
- Acción
- Salida esperada

---

### `docs/estructura_repositorio.md`
Describe:
1. Árbol del repositorio (actualizado).
2. Propósito de cada carpeta/archivo.
3. Convenciones de nombres (archivos, scripts, funciones).
4. Estrategia para mantener simplicidad y legibilidad.

---

### `docs/plan_de_pruebas.md`
Define un plan de pruebas básico pero claro:
1. Objetivo de pruebas.
2. Alcance de pruebas.
3. Casos de prueba mínimos (al menos 5).
4. Criterios de éxito/fallo.
5. Evidencia esperada (capturas de terminal, logs o salidas guardadas).

Incluye una tabla con:
- ID de prueba
- Descripción
- Entrada
- Salida esperada
- Resultado (Pendiente/OK/Falla)

---

## 6) Restricciones técnicas (obligatorias)

Para mantener el proyecto pequeño y viable:

- No usar frameworks pesados.
- No usar APIs pagadas.
- No usar bases de datos externas.
- No usar servicios en la nube.
- No usar contenedores (Docker/Podman).
- No añadir dependencias complejas de instalación.

El proyecto debe poder ejecutarse con herramientas comunes del sistema (terminal + compilador/intérprete estándar).

---

## 7) Criterios de evaluación sugeridos (100%)

1. **Claridad de la propuesta** (25%)
   - Problema definido con precisión.
   - Objetivo técnico entendible y acotado.

2. **Calidad de documentación** (35%)
   - Archivos completos, coherentes y bien redactados.
   - Términos técnicos usados correctamente.

3. **Diseño del repositorio** (20%)
   - Estructura limpia y lógica.
   - Nombres consistentes y orden adecuado.

4. **Plan de pruebas** (20%)
   - Casos de prueba relevantes y medibles.
   - Criterios de éxito bien definidos.

---

## 8) Recomendaciones pedagógicas para el estudiante

- Empieza con un objetivo mínimo funcional.
- Evita “idea gigante”; prioriza una herramienta pequeña pero útil.
- Si eliges ARM64, reduce alcance al máximo.
- Antes de codificar, valida que tu caso de uso y pruebas estén bien definidos.
- Si usas IA (Codex u otra), úsala para mejorar redacción, estructura y pruebas, no para inflar complejidad.

---

## 9) Checklist de entrega

Marca cada punto antes de enviar:

- [ ] Elegí **un** lenguaje principal (ARM64, C, Python o Bash).
- [ ] Incluí `README.md` con resumen y objetivo.
- [ ] Completé `docs/propuesta.md` con alcance y MVP.
- [ ] Completé `docs/caso_de_uso.md` con flujo principal y alternos.
- [ ] Completé `docs/estructura_repositorio.md`.
- [ ] Completé `docs/plan_de_pruebas.md` con al menos 5 pruebas.
- [ ] Mi propuesta evita dependencias complejas y servicios externos.
- [ ] El proyecto es pequeño y viable en tiempo de curso.

---

## 10) Formato de entrega en GitHub Classroom

1. Crea/acepta tu repositorio en GitHub Classroom.
2. Sube los archivos solicitados con commits claros.
3. Usa mensajes de commit descriptivos, por ejemplo:
   - `docs: agregar propuesta inicial`
   - `docs: definir caso de uso y flujos alternos`
   - `docs: añadir plan de pruebas base`
4. Entrega el enlace del repositorio según indicación del docente.

---

## 11) Plantilla breve de autoevaluación (opcional)

Incluye al final de tu `README.md`:

- ¿Qué tan claro está el problema que resolverás? (1–5)
- ¿Qué tan realista es tu alcance para 1–2 semanas? (1–5)
- ¿Qué parte de la documentación necesitas mejorar antes de programar?
- ¿Cuál es tu MVP exacto en una oración?

---

### Mensaje final al estudiante

La meta de esta actividad es que aprendas a **pensar como ingeniero/a de sistemas**: definir bien el problema, acotar, justificar decisiones técnicas y planear pruebas antes de escribir demasiado código.
