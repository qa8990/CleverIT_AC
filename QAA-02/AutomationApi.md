# Ejercicio 2 (QAA-02) - Automatización de API

## Descripción:

Tenemos la siguiente API https://jsonplaceholder.typicode.com/
Y esta API tiene los siguientes EndPoints de consulta:
- [ ] posts 100 posts
- [ ] comments 500 comments
- [ ] albums 100 albums
- [ ] photos 5000 photos
- [ ] todos 200 todos
- [ ] users 10 users

Considerando esta API y sus recursos, selecciona 3 de estos recursos y diseñar los casos de prueba funcionales que veas adecuados y luego
automatiza al menos 6 casos de prueba distintos (debe ser en Postman)

## Test Escenarios
| Ruta | Verbo http | Descripcion |
| --- | --- | --- |
| https://jsonplaceholder.typicode.com/posts | GET | Obtener 100 Posts |
| https://jsonplaceholder.typicode.com/posts/1 | GET | Obtener un numero determinado de Posts |
