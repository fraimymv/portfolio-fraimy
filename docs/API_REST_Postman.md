
# Práctica API REST con Postman - CRUD Estudiantes

Este proyecto documenta una serie de pruebas realizadas con Postman para validar el comportamiento de una API REST simulada, enfocada en la gestión de estudiantes.

La API utilizada responde en el entorno local:  
`http://localhost:3000/students`

---

## 1. Consultar lista de estudiantes

```http
GET localhost:3000/students
```

**Resultado esperado:**  
- Código: 200 OK  
- Respuesta: Lista completa de estudiantes en JSON.

---

## 2. Crear un estudiante con tu nombre

```http
POST localhost:3000/students
```

**Body:**
```json
{
  "id": "4"
  "name": "Fraimy",
  "location": "Dominican Republic",
  "phone": "18295916116"
  "courses": [
      "Python",
      "Java"
  ]
}
```

**Resultado esperado:**  
- Código: 201 Created  
- Estudiante agregado correctamente.

---

## 3. Verificar la creación

```http
GET localhost:3000/students
```

Consulta al estudiante recién creado

---

## 4. Consultar un estudiante por ID

```http
GET localhost:3000/students/2
```

Devuelve la información completa del estudiante con ID 2

---

## 5. Actualizar estudiante por ID

```http
PUT localhost:3000/students/2
```

**Body:**
```json
{
  "id": "2"
  "name": "Kate",
  "location": "US",
  "phone": "98876543213"
  "courses": [
      "Python",
      "Appium",
      "Java"
  ]
}
```

Actualiza todos los campos del estudiante con ID 2.

---

## 6. Eliminar estudiante por ID

```http
DELETE localhost:3000/students/2
```

Elimina al estudiante con ID 1 del sistema.

---

## 7. Verificar eliminación

```http
GET localhost:3000/students/2
```

**Resultado esperado:**  
- Código: 404 Not Found

---

## 8. Prueba negativa: crear sin nombre

```http
POST localhost:3000/students
```

**Body:**
```json
{
    "id": "2",
    "name": "",
    "location": "Latvia",
    "phone": "32156745621",
    "courses": [
        "Appium",
        "Python"
    ]
}
```

**Resultado esperado:**  
- Código: 400 Bad Request o error de validación.

**Resultado actual:**  
- Código: 201 Created.

**Nota:**
- El sistema no valida si el campo “name” está vacío, por lo que esta prueba negativa no fue rechazada como debería. 

---

## 9. Actualizar número de teléfono

```http
PATCH localhost:3000/students/4
```

**Body:**
```json
{
  "phone": "18093328122"
}
```

---

## 10. Crear múltiples estudiantes

```http
POST localhost:3000/students
```

**Body:**
```json
[
  {
    "id": "5"
    "name": "Nate",
    "location": "Russia",
    "phone": "98654123",
    "courses": [
        "Python",
        "Selenium"
    ]
},
{
    "id": "6",
    "name": "Audrey",
    "location": "Australia",
    "phone": "20355789045",
    "courses": [
        "Appium",
        "C#"
    ]
},
{
    "id": "7",
    "name": "Thiago",
    "location": "Argentina",
    "phone": "3025879015",
    "courses": [
        "Java",
        "RestAPI"
    ]
}
]
```

---

## 11. Consultar estudiante con ID 1

```http
GET localhost:3000/students/1
```

---

## 12. Prueba con número de teléfono inválido

```http
POST localhost:3000/students
```

**Body:**
```json
{
    "id": "",
    "name": "Amanda",
    "location": "Mexico",
    "phone": "hgfrtyuplz",
    "courses": [
        "Java"
    ]
}
```

---

## 13. Actualizar con ID inexistente

```http
PUT localhost:3000/students
```
**Body:**
```json
{
    "id": "",
    "name": "Amanda",
    "location": "Mexico",
    "phone": "hgfrtyuplz",
    "courses": [
        "Java",
        "C#"
    ]
}
```

**Resultado esperado:**  
- Código: 404 Not Found

---

## 14. Crear estudiante con 3 cursos

```http
POST localhost:3000/students
```

**Body:**
```json
{
    "id": "8",
    "name": "Sophie",
    "location": "UK",
    "phone": "1025849267",
    "courses": [
        "Java",
        "C#",
        "Cypress"
    ]
}
```

---

## 15. Crear estudiante sin cursos

```http
POST localhost:3000/students
```

**Body:**
```json
{
    "id": "9",
    "name": "Andy",
    "location": "UK",
    "phone": "086849267",
    "courses": []
}
```

---

## 16. Actualizar únicamente ubicación

```http
PATCH localhost:3000/students/5
```

**Body:**
```json
{
    "location": "UK"
}
```

---

## 📎 Evidencias

El archivo PDF contiene capturas de pantalla y evidencia de cada prueba ejecutada:

👉 [`API_REST_Postman_FraimyMV.pdf`](https://fraimymv.github.io/docs/API_REST_Postman_FraimyMV.pdf)

---

## 🛠 Herramientas utilizadas

- Postman
- JSON Server
- Node.js

---

## ✅ Conclusión

Estas pruebas cubren casos positivos y negativos del ciclo CRUD en una API REST. Permiten validar estructura, respuesta y manejo de errores del sistema de estudiantes.
