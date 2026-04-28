# Plan de pruebas

## Estrategia de pruebas
Se aplicarán pruebas funcionales de caja negra sobre la interfaz de consola. Cada caso valida una condición específica de entrada, proceso y salida. La prioridad es comprobar comportamiento observable y código de retorno del programa.

## Casos de prueba
| ID | Entrada | Resultado esperado | Criterio de éxito |
|---|---|---|---|
| CP-01 | `8` + Enter | Mensaje de resultado “PAR” | La salida contiene “PAR” y retorna código 0 |
| CP-02 | `7` + Enter | Mensaje de resultado “IMPAR” | La salida contiene “IMPAR” y retorna código 0 |
| CP-03 | `0` + Enter | Mensaje de resultado “PAR” | Se procesa cero como valor válido y retorna 0 |
| CP-04 | `7a` + Enter | Error por formato inválido | Se muestra error y retorna código distinto de 0 |
| CP-05 | Enter sin datos | Error por entrada vacía | Se muestra error y retorna código distinto de 0 |
| CP-06 | `12345` + Enter | Resultado de paridad correcto | Coincide salida con cálculo esperado |

## Cobertura mínima
- Validación de formato: cubierta por CP-04 y CP-05.
- Conversión de ASCII a entero: cubierta por CP-01, CP-02, CP-03 y CP-06.
- Lógica de paridad: cubierta por CP-01, CP-02, CP-03 y CP-06.
- Manejo de salida y códigos de retorno: cubierta por todos los casos.

## Criterios de aprobación
- Ejecutar al menos 6/6 casos definidos.
- Aprobar mínimo 5/6 casos para acreditación básica.
- Aprobar 6/6 casos para desempeño sobresaliente.
- Documentar evidencia de ejecución (captura de terminal o bitácora textual) con fecha y versión del commit.
