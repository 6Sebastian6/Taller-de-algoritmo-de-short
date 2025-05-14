# Proyecto de Simulación de Algoritmo Cuántico de Shor

Este proyecto implementa una simulación clásica del **Algoritmo de Shor**, utilizado para la factorización eficiente de números compuestos. Se centra en el caso específico de la factorización de \( N = 247 \) usando la base \( a = 2 \), siguiendo el procedimiento teórico del algoritmo y sus pasos computacionales.

## Descripción del Proyecto

El objetivo principal es ilustrar cómo el algoritmo de Shor permite obtener los factores de un número compuesto, en este caso \( N = 247 \), mediante el cálculo del período de una función modular exponencial. Esta implementación se hace de forma clásica, simulando lo que en un sistema cuántico real se resolvería mediante técnicas de estimación de fase cuántica.

### Funcionalidades Implementadas

1. **Cálculo de potencias módulo \( N \)**: Se generan las potencias sucesivas de \( a^k \mod N \), para detectar el período de la función.

2. **Búsqueda del período \( r \)**: Se determina el menor valor \( r \) tal que \( a^r \equiv 1 \mod N \). Este valor es esencial para el éxito del algoritmo.

3. **Verificación de condiciones**: Se comprueba si \( r \) es par y \( a^{r/2} \not\equiv -1 \mod N \), lo cual permite continuar con el cálculo de factores.

4. **Cálculo de factores mediante el MCD**: Se utilizan expresiones del tipo \( \gcd(a^{r/2} \pm 1, N) \) para obtener los factores no triviales de \( N \).

5. **Visualización de potencias**: Se grafica la función \( a^k \mod N \) para ilustrar visualmente el comportamiento periódico.

### Ejercicio Simulado

Este proyecto resuelve el siguiente ejercicio:

> **Compute the factors of \( N = 247 \) using \( a = 2 \)**

Como resultado, se encuentra que los factores de 247 son:


