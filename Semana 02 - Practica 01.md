# Problema de la Planificación de un Viaje en Grupo

Un grupo de amigos está planeando un viaje por carretera. Tu tarea es crear un programa que les ayude a gestionar el presupuesto de viaje, considerando los gastos compartidos.

## **Instrucciones:**

1.  El programa debe preguntar el presupuesto inicial total del grupo.
    
2.  Debe usar un **ciclo** para registrar los gastos del viaje. En cada iteración, el programa debe preguntar el tipo de gasto y el monto:
    
    -   **Gasolina:** El monto debe dividirse entre el número de personas en el grupo.
        
    -   **Comida:** El gasto es individual, por lo que el monto no se divide.
        
    -   **Atracción turística:** El gasto puede ser compartido o no. Si se comparte, se divide el monto entre el número de personas que pagaron.
        
3.  El ciclo debe continuar hasta que el usuario indique que todos los gastos han sido registrados.
    
4.  Dentro del ciclo, se deben utilizar **estructuras condicionales** para:
    
    -   Actualizar el presupuesto restante del grupo.
        
    -   Verificar que cada gasto no supere el presupuesto disponible. Si es así, se debe mostrar un mensaje de error y no se debe registrar el gasto.
        
    -   Se debe usar una expresión lógica con **AND** y/o **OR** para validar un gasto. Por ejemplo, un gasto es válido si el tipo de gasto es "gasolina", **O** si es "comida", **O** si es "atracción turística", **Y** si el monto es mayor a cero.
        
5.  El programa debe llevar un **contador** de la cantidad de gastos registrados y un **acumulador** que sume el total gastado en el viaje.
    
6.  Al final del ciclo, el programa debe mostrar un resumen que incluya:
    
    -   El presupuesto restante del grupo.
        
    -   La cantidad de gastos registrados (el contador).
        
    -   El total de dinero gastado (el acumulador).
        
    -   Un mensaje final usando el operador lógico **NOT** para indicar si el presupuesto final **NO** es superior a un monto de reserva (por ejemplo, si el presupuesto final **NO** es mayor o igual a $200).
