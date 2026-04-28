# Propuesta técnica del microproyecto

## Problema
Se requiere una práctica breve que permita evaluar competencias de bajo nivel (instrucciones, registros y llamadas al sistema) sin depender de infraestructura compleja. El reto es que el estudiantado implemente una utilidad de línea de comandos en ARM64 Assembly, verificable con casos de prueba simples.

## Justificación
Este microproyecto conecta teoría de arquitectura con evidencia tangible de aprendizaje. Al trabajar con ARM64 Assembly, el estudiantado comprende de forma directa:
- manejo explícito de registros,
- control de flujo y comparación,
- estructura modular mínima con macros,
- relación entre entrada/salida y sistema operativo.

## Alcance y límites
**Alcance (3 a 5 funcionalidades pequeñas):**
1. Leer una cadena numérica desde entrada estándar.
2. Validar que la entrada contenga solo dígitos y salto de línea.
3. Convertir ASCII a entero (rango pequeño controlado).
4. Determinar si el número es par o impar.
5. Mostrar resultado y código de salida.

**Límites:**
- Núcleo obligatorio en ARM64 Assembly.
- Sin Python.
- Sin frameworks pesados, sin Docker, sin Kubernetes.
- Sin servicios cloud o APIs pagadas.
- Sin base de datos obligatoria.
- Máximo sugerido: ~150 líneas funcionales.

## Arquitectura (alto nivel)
- **Capa 1 (núcleo ARM64 Assembly, obligatoria):**
  - Archivo principal (`src/main.s`) con secciones `.data` y `.text`.
  - Macro funcional `PRINT msg, len` para estandarizar salida por `write`.
  - Rutinas: lectura, validación, conversión y evaluación de paridad.
- **Capa 2 (opcional mínima, Bash):**
  - Script simple de compilación/ejecución (`scripts/run.sh`) para facilitar pruebas locales.

## Riesgos y mitigación
- **Riesgo:** errores de manejo de buffer.
  - **Mitigación:** longitud máxima fija y validación de fin de línea.
- **Riesgo:** confusión con llamadas al sistema en ARM64 Linux.
  - **Mitigación:** plantilla base con comentarios y tabla breve de registros usados.
- **Riesgo:** sobrealcance del proyecto.
  - **Mitigación:** limitar funciones a cinco tareas concretas y medibles.

## Supuestos
- El entorno académico cuenta con Linux ARM64 nativo o emulación configurada por la institución.
- El estudiantado dispone de ensamblador y enlazador estándar (por ejemplo, `as` y `ld`).
- La evaluación prioriza claridad técnica, evidencia de pruebas y cumplimiento de restricciones.
