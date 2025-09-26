# **Enunciado del Ejercicio: Máquina de Contar Monedas**

## **Contexto:**
Imagina que tienes una alcancía digital. Quieres crear un programa que te ayude a saber cuánto dinero has ahorrado.

**Tu tarea es** diseñar un diagrama de flujo y luego codificar en Java un programa que simule el proceso de ir metiendo monedas en la alcancía una por una.

## **Descripción del Programa:**

El programa debe funcionar así:

1.  **Inicio:** La alcancía empieza vacía. El programa muestra el mensaje: "**Alcancía Digital**".

2.  **Bucle Principal (While):** El programa debe correr en un bucle `while` que continúe mientras el usuario quiera seguir agregando monedas.

3.  **Interacción en cada vuelta:** En cada repetición del bucle, el programa debe:
    *   Preguntar al usuario: "¿Ingresar una moneda? (S para Sí, N para No): ".

4.  **Procesamiento (Estructura Condicional):**
    *   **Si el usuario responde 'S' (o 's'):**
        *   El programa suma una cantidad fija (por ejemplo, **$1.000**) a un total.
        *   Muestra un mensaje confirmando: "¡Clink! Has agregado $1.000. Total ahorrado: $[Total]".
        *   El bucle continúa.
    *   **Si el usuario responde 'N' (o 'n'):**
        *   El bucle `while` debe terminar.
    *   **Si el usuario ingresa cualquier otra letra:** El programa muestra un mensaje: "Opción no válida. Por favor, ingresa S para Sí o N para No." y vuelve a preguntar **sin contar una moneda nueva**.

5.  **Fin del Programa:** Cuando el usuario decida no ingresar más monedas (escribiendo 'N'), el bucle termina y el programa muestra un mensaje final: "¡Felicidades! Tu ahorro total es: $[Total]".

## **Elementos Clave a Utilizar:**
*   **`while`:** Para repetir el proceso de preguntar y agregar monedas.
*   **Contador/Acumulador:** Una variable que guarde el **total de dinero ahorrado** (se va sumando +1000 cada vez que el usuario dice 'S').
*   **Estructura Condicional (`if` - `else if`):** Para decidir qué hacer según la letra que ingrese el usuario ('S', 'N' u otra).
*   **Condición de Salida:** La respuesta del usuario ('N') es lo que hará que la condición del `while` sea falsa.

---

Este ejercicio es ideal como primer contacto porque:
*   La lógica es muy clara y lineal.
*   La condición del `while` se basa directamente en la entrada del usuario.
*   Introduce el concepto de acumulador de forma muy visual (el total va creciendo).
*   Practican la validación básica de entradas con las condicionales.

¡Espero que les sea de mucha ayuda para dar sus primeros pasos!
