# **Enunciado del Problema: Control de Aforo en una Biblioteca**

## **Contexto:**
Eres parte del equipo de sistemas de una biblioteca universitaria. La biblioteca tiene una sala de estudio con una capacidad máxima de **50 personas** por motivos de seguridad y comodidad. Para gestionar el flujo de usuarios, se necesita un programa simple que controle el ingreso y salida de personas.

**Tu tarea es** diseñar un diagrama de flujo y luego codificar en Java un programa que simule este sistema de control durante un día de operaciones.

## **Descripción del Programa:**

El programa debe funcionar de la siguiente manera:

1.  **Inicialización:** Al comenzar, la sala está vacía. El programa mostrará un mensaje de bienvenida: "Sistema de Control de Aforo Iniciado. Capacidad máxima: 50 personas."

2.  **Bucle Principal (While):** El programa debe correr en un bucle mientras la biblioteca esté abierta. La condición para permanecer abierto es que **no** se haya ingresado una señal especial para cerrar.

3.  **Menú de Opciones:** En cada iteración del bucle, el programa debe mostrar un menú con las siguientes opciones:
    *   **1:** Registrar **ingreso** de una persona.
    *   **2:** Registrar **salida** de una persona.
    *   **3:** Cerrar el sistema (señal especial para terminar el programa).

4.  **Procesamiento de Opciones (Estructuras Condicionales):** Dependiendo de la opción seleccionada, el programa debe:
    *   **Opción 1 (Ingreso):**
        *   Verificar que el aforo actual sea **menor que** la capacidad máxima (50). **(Operador lógico de comparación)**.
        *   **Si hay espacio:** Permitir el ingreso, aumentar el contador de personas dentro de la sala y mostrar un mensaje de "Ingreso registrado. Personas en la sala: [X]".
        *   **Si no hay espacio (aforo lleno):** Mostrar un mensaje de "Aforo completo. No se puede ingresar. Espere su turno.".
    *   **Opción 2 (Salida):**
        *   Verificar que el aforo actual sea **mayor que** cero (no se puede registrar una salida si la sala está vacía). **(Operador lógico de comparación)**.
        *   **Si hay personas:** Registrar la salida, disminuir el contador de personas y mostrar un mensaje de "Salida registrada. Personas en la sala: [X]".
        *   **Si la sala está vacía:** Mostrar un mensaje de "Error: La sala está vacía. No se puede registrar una salida.".
    *   **Opción 3 (Cerrar sistema):**
        *   Terminar el bucle `while` y finalizar el programa, mostrando un mensaje final como "Sistema cerrado. El aforo final es de: [X] personas.".

5.  **Elementos Clave a Utilizar:**
    *   **`while`:** Para mantener el programa en ejecución hasta que se elija la opción de cerrar.
    *   **Contador:** Una variable que lleve la cuenta del número actual de personas en la sala (se incrementa con ingresos y se decrementa con salidas).
    *   **Acumulador (Opcional pero recomendado):** Una variable que lleve la cuenta del **total de personas** que ingresaron a la sala durante todo el día (solo se incrementa con cada ingreso exitoso).
    *   **Estructuras Condicionales (`if` - `else`):** Para decidir las acciones al ingresar, salir o cerrar, y para las validaciones de aforo lleno o sala vacía.
    *   **Operadores Lógicos:** Serán necesarios en las condiciones para comparar el aforo actual con la capacidad máxima y con cero (por ejemplo: `aforoActual < capacidadMaxima`).

## **Requerimientos de Salida:**
Los mensajes en consola deben ser claros e informativos, indicando siempre la acción realizada y el estado actual del aforo.
