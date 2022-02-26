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
| https://jsonplaceholder.typicode.com/posts/:id | GET | Obtener un Post por el ID |
| https://jsonplaceholder.typicode.com/posts/:id/comments | GET | Obtener todos los comentarios de un Post por el ID |

## Test cases 1
| Ruta | Verbo http | Descripcion |
| --- | --- | --- |
| https://jsonplaceholder.typicode.com/posts | GET | Obtener 100 Posts |

| # | Scenario |
| --- | --- |
| 1 | API responde con 200 |
| 2 | Retorna 100 resultados (100 posts) |
| 3 | Formato del JSON es valido |

## Test cases 2
| Ruta | Verbo http | Descripcion |
| --- | --- | --- |
| https://jsonplaceholder.typicode.com/posts | POST | Creacion de un resource |

| # | Scenario |
| --- | --- |
| 1 | API responde con 200 |
| 2 | Retorna un JSON |
| 3 | Formato del JSON es valido |
