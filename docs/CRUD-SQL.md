# Práctica CRUD con SQL

Este documento contiene una serie de ejemplos prácticos para ejecutar operaciones CRUD (Create, Read, Update, Delete) usando sentencias SQL básicas. Es una simulación de base de datos con tablas como `productos`, `clientes`, `ventas` y `proveedores`.

---

## Sección 1: CREATE - Insertar Datos

### Agregar un nuevo producto
**Nombre:** Galletas Choco  
**Categoría:** Dulces  
**Precio:** 120 pesos  
**Stock:** 50 unidades

```sql
INSERT INTO Productos (Nombre, Categoria, Precio, Stock)
VALUES ('Galletas Choco', 'Dulces', '120', '50')
```

### Registrar un nuevo cliente
**Nombre:** Luis Gómez  
**Correo:** luis.gomez@email.com  
**Teléfono:** 829-123-4567

```sql
INSERT INTO Clientes(Nombre, Apellido, Correo, Telefono)
VALUES('Luis', 'Gómez', 'luis.gomez@email.com', '829-123-4567')
```

### Insertar una venta
**Cliente ID:** 3  
**Total:** 850 pesos

```sql
INSERT INTO Ventas(ID_Clientes, Total)
VALUES('3', '850')
```

### Agregar proveedor
**Nombre:** Distribuidora Tropical  
**Teléfono:** 809-765-4321  
**Correo:** contacto@tropical.com

```sql
INSERT INTO Proveedores(Nombre, Telefono, Email)
VALUES('Distribuidora Tropical', '809-765-4321', 'contacto@tropical.com')
```

### Registrar 3 productos (categoría: Bebidas)

```sql
INSERT INTO Productos (Nombre, Categoria, Precio, Stock, ID_Proveedor) 
VALUES('Jugo de Uva', 'Bebidas', '150', '40', '6'), ('Bebida Hidratante', 'Bebidas', '105', '25', '6'), ('Jugo de Manzana', 'Bebidas', '175', '120', '6')
```

---

## Sección 2: READ - Consultar Datos

### Listar nombre y precio de productos

```sql
SELECT Nombre, Precio 
FROM Productos
```

### Clientes registrados después del 01/01/2024

```sql
SELECT Nombre, Apellido
FROM Clientes
WHERE FechaRegistro>2024-01-01
```

### Ventas realizadas en el último mes

```sql
SELECT * FROM Ventas
WHERE month(FechaVenta)='3'
```

### Productos con precio entre 100 y 500

```sql
SELECT * FROM Productos
WHERE Precio BETWEEN '100' AND '500'
```

### Contar productos en categoría Lácteos

```sql
SELECT COUNT(Categoria) 
FROM Productos
WHERE Categoria LIKE 'Lácteos'
```

---

## Sección 3: UPDATE - Modificar Datos

### Actualizar precio del producto “Leche”

```sql
UPDATE Productos
SET Precio='95'
WHERE ID_Producto='Leche'
```

### Sumar 30 al stock del producto “Pan”

```sql
UPDATE Productos
SET Stock=Stock+'30'
WHERE Nombre='Pan'
```

### Actualizar correo del cliente con ID 5

```sql
UPDATE Clientes
SET Correo='nuevo.email@email.com'
WHERE ID_Cliente='5'
```

### Cambiar nombre del proveedor ID 2

```sql
UPDATE Proveedores
SET Nombre='Alimentos del Caribe Express'
WHERE ID_Proveedor='2'
```

### Incrementar 10% precio de productos categoría "Carnes"

```sql
UPDATE Productos
SET Precio=Precio*'1.10'
WHERE Categoria='Carnes'
```

---

## Sección 4: DELETE - Eliminar Datos

### Eliminar producto con ID 10

```sql
DELETE FROM Productos
WHERE ID_Productos='10'
```

### Borrar cliente por correo

```sql
DELETE FROM Clientes
WHERE Correo='cliente.prueba@email.com'
```

### Eliminar ventas antes del 01/01/2023

```sql
DELETE FROM Ventas
WHERE FechaVenta<'2023-01-01'
```

### Eliminar productos con stock = 0

```sql
DELETE FROM Productos
WHERE Stock ='0'
```

### Eliminar proveedor ID 4 y sus productos

```sql
DELETE FROM Proveedores
WHERE ID_Proveedor='4'

DELETE FROM Productos
WHERE ID_Proveedor='4'
```

---

## 📎 Notas

- Este CRUD simula un entorno de base de datos con relaciones básicas.
- La estructura de las tablas no está incluida, pero puedes asumir campos comunes como `id`, `nombre`, `categoria`, etc.
---

## 📁 Recursos Relacionados

- [Versión PDF de esta práctica](https://fraimymv.github.io/docs/CRUD_SQL_FraimyMV.pdf)
- Repositorio con imágenes de las consultas realizadas