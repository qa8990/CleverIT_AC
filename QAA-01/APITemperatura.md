## Ejercicio 1 (QAA-01) API Temperatura

#Descripción:

Crear los casos de prueba posibles para testear el siguiente microservicio GET, que recibe:
En el request la fecha del día actual en formato DD-MM-AAAA.
Dos headers, el primero es "Country", cuyo dominio de valores puede ser "Chile" o "Argentina" y el segundo es "City", cuyo dominio de
valores es "Santiago","Arica", "Chiloe" (cuando se trata de Country Chile) y "BuenosAires", "SanJuan" (cuando country es Argentina)
Cuando el resultado es positivo entrega status ok y código http 200 y en caso de error el status es "client error" y en caso de error de
conexion el status es "server error" y en el caso de codigo para cada uno de estos status se entrega los codigos http de error estándar.
Considera que cuando es un País distinto a los señalados o una ciudad distinta el response "País y Ciudad incorrectos", y que todos los
campos a ingresar son Sensitive Case.
El response del microservicio devuelve la temperaturaActual y temperaturaDiaSiguiente en formato json.
