## Ejercicio 1 (QAA-01) API Temperatura

## Descripción:

#Crear los casos de prueba posibles para testear el siguiente microservicio GET, que recibe:

- En el request la fecha del día actual en formato DD-MM-AAAA.
- Dos headers, el primero es "Country", cuyo dominio de valores puede ser "Chile" o "Argentina" y el segundo es "City", cuyo dominio de valores es "Santiago","Arica", "Chiloe" (cuando se trata de Country Chile) y "BuenosAires", "SanJuan" (cuando country es Argentina)
- Cuando el resultado es positivo entrega status ok y código http 200 y en caso de error el status es "client error" y en caso de error de conexion el status es "server error" y en el caso de codigo para cada uno de estos status se entrega los codigos http de error estándar.
- Considera que cuando es un País distinto a los señalados o una ciudad distinta el response "País y Ciudad incorrectos", y que todos los campos a ingresar son Sensitive Case.
- El response del microservicio devuelve la temperaturaActual y temperaturaDiaSiguiente en formato json.

## Scenarios

| # | Scenario |
| --- | --- |
| 1 | Buscar valores de temperatura para Fecha, Country y City No validos |
| 2 | Buscar valores de temperatura para Fecha, Country No validos y City validos |
| 3 | Buscar valores de temperatura para Fecha y City No Validos, Country validos |
| 4 | Buscar valores de temperatura para Fecha No valida, Country y City validos |
| 5 | Buscar valores de temperatura para Fecha Valida y Country y City No validos |
| 6 | Buscar valores de temperatura para Fecha y City Validos, Country No validos |
| 7 | Buscar valores de temperatura para Fecha y Country Validos, City No validos |
| 8 | Buscar valores de temperatura para Fecha, City y Country validos |

## Tabla de escenarios
| Fecha | Country | City | Status Ok | Status Ok |
| --- | --- | --- | --- |
| FALSE | FALSE | FALSE | :x: |
| FALSE | FALSE | TRUE | :x: |
| FALSE | TRUE | FALSE | :x: |
| FALSE | TRUE | TRUE | :x: |
| TRUE | FALSE | FALSE | :x: |
| TRUE | FALSE | TRUE | :x: |
| TRUE | TRUE | FALSE | :x: |
| TRUE | TRUE | TRUE | :heavy_check_mark: |



