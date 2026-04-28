# Caso de uso: Evaluar paridad de un número

## Actor principal
Estudiante desarrollador/a en laboratorio de arquitectura de computadoras.

## Flujo principal
1. El actor ejecuta el programa desde terminal.
2. El sistema solicita un número entero positivo en formato decimal.
3. El actor captura el número y presiona Enter.
4. El sistema valida formato numérico.
5. El sistema convierte la entrada a entero.
6. El sistema evalúa paridad (par/impar).
7. El sistema muestra resultado y finaliza con código de salida exitoso.

## Escenarios alternos
### Alterno A: Entrada con caracteres no numéricos
1. El actor introduce texto con letras o símbolos.
2. El sistema detecta formato inválido.
3. El sistema muestra mensaje de error y termina con código distinto de cero.

### Alterno B: Entrada vacía
1. El actor presiona Enter sin capturar dígitos.
2. El sistema identifica ausencia de datos válidos.
3. El sistema informa error de entrada y solicita reintento en nueva ejecución.

## Precondiciones
- Programa compilado para ARM64.
- Entorno de ejecución con permisos de consola.
- Archivos de proyecto y documentación disponibles en el repositorio.

## Postcondiciones
- Se emite salida clara sobre paridad o error de validación.
- Se registra comportamiento esperado según caso de prueba.
- El binario concluye con código de salida coherente con el resultado.

## Criterios de aceptación
- La entrada `8` produce salida “PAR”.
- La entrada `7` produce salida “IMPAR”.
- La entrada `7a` produce mensaje de formato inválido.
- La entrada vacía produce mensaje de error de captura.
- La macro de Assembly definida se usa al menos una vez en la salida del programa.
