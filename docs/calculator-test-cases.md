# Casos de prueba para calculadora / Calculator Test Cases

Diseño de casos para validar operaciones básicas (suma, resta, multiplicación, división).  
Design of test cases to validate basic operations (addition, subtraction, multiplication, division).

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Generar operación de Suma

**Acceptance Criteria:**  
1. Dentro de la calculadora el usuario podrá ingresar dos operados dentro de los campos "Primer número" y "Segundo número". Ambos campos deben aceptar únicamente números enteros y decimales.  
2. El usuario podrá seleccionar desde una lista desplegable llamada "Operación" una de las siguientes 5 operaciones básicas: suma, resta, multiplicación, división, concatenación.  
3. La calculadora tendrá un botón "Calcular" el cual al oprimirlo realice el cálculo de los dos valores ingresados según la operación que fue seleccionada.  
4. La operación deberá ejecutarse y mostrar el resultado de manera inmediata, sin demoras perceptibles con tiempos de respuestas dentro del primer segundo a partir de la ejecución.

**Precondition:**  
La calculadora esta abierta y lista para operar.

| Step  | Step Action                                               | Step Expected                                                                                                                |
|-------|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 1     | Ingresar números enteros en el campo "Primer número"      | El sistema visualiza el campo ¨Primer numero¨ el cual acepta números enteros .                                               |
| 2     | Ingresar números enteros en el campo "Segundo número"     | El sistema visualiza el campo ¨Segundo numero¨ el cual acepta números enteros .                                              |
| 3     | Seleccionar una de la opción Suma de la lista "Operación" | El usuario debe tener acceso a una lista llamada ¨Operación¨ la cual le permitirá seleccionar la opción Suma.                |
| 4     | Hacer click en el botón "Calcular" para recibir resultado | El sistema visualiza el botón ¨Calcular¨ el cual, al darle click, debe mostrar un resultado acorde a los valores ingresados. |
| 5     | Recibir resultado del calculo al instante                 | El resultado del calculo hecho se refleja de manera instantánea.                                                             |

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Generar operación de Resta

**Acceptance Criteria:**  
(igual que arriba)

**Precondition:**  
La calculadora esta abierta y lista para operar.

| Step  | Step Action                                                | Step Expected                                                                                                                |
|-------|------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 1     | Ingresar números enteros en el campo "Primer número"       | El sistema visualiza el campo ¨Primer numero¨ el cual acepta números enteros .                                               |
| 2     | Ingresar números decimales en el campo "Segundo número"    | El sistema visualiza el campo ¨Segundo numero¨ el cual acepta números enteros .                                              |
| 3     | Seleccionar una de la opción Resta de la lista "Operación" | El usuario debe tener acceso a una lista llamada ¨Operación¨ la cual le permitirá seleccionar la opción Resta.               |
| 4     | Hacer click en el botón "Calcular" para recibir resultado  | El sistema visualiza el botón ¨Calcular¨ el cual, al darle click, debe mostrar un resultado acorde a los valores ingresados. |
| 5     | Recibir resultado del calculo al instante                  | El resultado del calculo hecho se refleja de manera instantánea.                                                             |

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Generar operación de Multiplicación

**Acceptance Criteria:**  
1. Dentro de la calculadora el usuario podrá ingresar dos operados dentro de los campos "Primer número" y "Segundo número". Ambos campos deben aceptar únicamente números enteros y decimales.  
2. El usuario podrá seleccionar desde una lista desplegable llamada "Operación" una de las siguientes 5 operaciones básicas: suma, resta, multiplicación, división, concatenación.  
3. La calculadora tendrá un botón "Calcular" el cual al oprimirlo realice el cálculo de los dos valores ingresados según la operación que fue seleccionada.  
4. La operación deberá ejecutarse y mostrar el resultado de manera inmediata, sin demoras perceptibles con tiempos de respuestas dentro del primer segundo a partir de la ejecución.  
6. El usuario dispondrá de un check llamado "Solo enteros" el cual al ser marcado ocultará los decimales correspondientes al resultado de la operación, el sistema debe permitir al usuario poder marcar el check "Solo enteros" antes y/o después de obtener el resultado de la operación.

**Precondition:**  
La calculadora esta abierta y lista para operar.

| Step  | Step Action                                                         | Step Expected                                                                                                                |
|-------|---------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 1     | Ingresar números decimales en el campo "Primer número"              | El sistema visualiza el campo ¨Primer numero¨ el cual acepta números enteros .                                               |
| 2     | Ingresar números decimales en el campo "Segundo número"             | El sistema visualiza el campo ¨Segundo numero¨ el cual acepta números enteros .                                              |
| 3     | Seleccionar una de la opción Multiplicación de la lista "Operación" | El usuario debe tener acceso a una lista llamada ¨Operación¨ la cual le permitirá seleccionar la opción Multiplicación.      |
| 4     | Hacer click en el botón "Calcular" para recibir resultado           | El sistema visualiza el botón ¨Calcular¨ el cual, al darle click, debe mostrar un resultado acorde a los valores ingresados. |
| 5     | Recibir resultado del calculo al instante                           | El resultado del calculo hecho se refleja de manera instantánea.                                                             |
| 6     | Seleccionar la opción "Solo enteros"                                | El usuario podrá optar por una opción llamada ¨Solo enteros¨, después de la operación, la cual oculta los decimales.         |

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Generar operación de División

**Acceptance Criteria:**  
(igual que en suma)

**Precondition:**  
La calculadora esta abierta y lista para operar.

| Step  | Step Action                                                   | Step Expected                                                                                                                |
|-------|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 1     | Ingresar números decimales en el campo "Primer número"        | El sistema visualiza el campo ¨Primer numero¨ el cual acepta números enteros .                                               |
| 2     | Ingresar números enteros en el campo "Segundo número"         | El sistema visualiza el campo ¨Segundo numero¨ el cual acepta números enteros .                                              |
| 3     | Seleccionar una de la opción División de la lista "Operación" | El usuario debe tener acceso a una lista llamada ¨Operación¨ la cual le permitirá seleccionar la opción División.            |
| 4     | Hacer click en el botón "Calcular" para recibir resultado     | El sistema visualiza el botón ¨Calcular¨ el cual, al darle click, debe mostrar un resultado acorde a los valores ingresados. |
| 5     | Recibir resultado del calculo al instante                     | El resultado del calculo hecho se refleja de manera instantánea.                                                             |

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Generar operación de Concatenación

**Acceptance Criteria:**  
1. Dentro de la calculadora el usuario podrá ingresar dos operados dentro de los campos "Primer número" y "Segundo número". Ambos campos deben aceptar únicamente números enteros y decimales.  
2. El usuario podrá seleccionar desde una lista desplegable llamada "Operación" una de las siguientes 5 operaciones básicas: suma, resta, multiplicación, división, concatenación.  
3. La calculadora tendrá un botón "Calcular" el cual al oprimirlo realice el cálculo de los dos valores ingresados según la operación que fue seleccionada.  
4. La operación deberá ejecutarse y mostrar el resultado de manera inmediata, sin demoras perceptibles con tiempos de respuestas dentro del primer segundo a partir de la ejecución.  
6. El usuario dispondrá de un check llamado "Solo enteros" el cual al ser marcado ocultará los decimales correspondientes al resultado de la operación, el sistema debe permitir al usuario poder marcar el check "Solo enteros" antes y/o después de obtener el resultado de la operación.

**Precondition:**  
La calculadora esta abierta y lista para operar.

| Step  | Step Action                                                        | Step Expected                                                                                                                |
|-------|--------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 1     | Ingresar números enteros en el campo "Primer número"               | El sistema visualiza el campo ¨Primer numero¨ el cual acepta números enteros .                                               |
| 2     | Ingresar números decimales en el campo "Segundo número"            | El sistema visualiza el campo ¨Segundo numero¨ el cual acepta números enteros .                                              |
| 3     | Seleccionar la opción "Solo enteros"                               | El usuario podrá optar por una opción llamada ¨Solo enteros¨, antes de la operación, la cual oculta los decimales.           |
| 4     | Seleccionar una de la opción Concatenación de la lista "Operación" | El usuario debe tener acceso a una lista llamada ¨Operación¨ la cual le permitirá seleccionar la opción Concatenación.       |
| 5     | Hacer click en el botón "Calcular" para recibir resultado          | El sistema visualiza el botón ¨Calcular¨ el cual, al darle click, debe mostrar un resultado acorde a los valores ingresados. |
| 6     | Recibir resultado del calculo al instante                          | El resultado del calculo hecho se refleja de manera instantánea.                                                             |

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Validar mensaje de error al dividir entre cero

**Acceptance Criteria:**  
5. Si el usuario intenta dividir entre cero, la calculadora debe mostrar el siguiente mensaje de error "Error".

**Precondition:**  
La calculadora esta abierta y lista para operar.

| Step  | Step Action                                | Step Expected                                                                                |
|-------|--------------------------------------------|----------------------------------------------------------------------------------------------|
| 1     | Ingresar un numero para dividir entre cero | El sistema permite al usuario ingresar un numero decimal y/o entero para dividir entre cero. |
| 2     | Dar click al botón "Calcular"              | Al dividir aparece el mensaje ¨Error al dividir entre cero¨.                                 |

---

## TC - Creación de calculadora básica para matemáticas (para practicar) - Borrar operaciones y resultados existentes

**Acceptance Criteria:**  
7. El usuario debe tener la opción de limpiar los campos correspondientes a los operandos y al resultado para realizar una nueva operación sin necesidad de refrescar o reiniciar la calculadora.

**Precondition:**  
La calculadora debe mostrar una operación y su resultado de esta.

| Step  | Step Action                         | Step Expected                                                                                                                                                                                              |
|-------|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1     | Hacer click en "Limpiar los campos" | El usuario tendrá a su disponibilidad una opción para limpiar toda operación y resultado ejecutado. La calculadora queda lista para realizar nuevas operaciones sin la necesidad de darle refresh/restart. |

---

## 📁 Recursos Relacionados

- [Versión PDF de esta práctica](https://fraimymv.github.io/docs/TestCases_FraimyMV.pdf)

