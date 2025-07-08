# Ejemplos de Test Automatizados en Postman

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

```javascript
pm.test("La respuesta contiene 'firstName'", function () {
    var jsonData = pm.response.json();
    pm.expect(jsonData.firstName).to.not.be.undefined;
});
```
