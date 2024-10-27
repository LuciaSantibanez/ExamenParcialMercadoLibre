# PARCIAL DESARROLLO DE SOFTWARE

El presente repositorio contiene el ejercicio técnico de Mercado Libre sobre la detección de mutantes.

## Introducción 

Magneto quiere reclutar la mayor cantidad de mutantes para poder luchar 
contra los X-Mens. 
Te ha contratado a ti para que desarrolles un proyecto que detecte si un 
humano es mutante basándose en su secuencia de ADN. 
Para eso te ha pedido crear un programa con un método o función con la siguiente firma: 

```java
boolean isMutant(String[] dna)
```

## Funcionamiento 

Se recibe como parámetro un array de String que representan cada fila de una tabla de (NxN) con la secuancia del ADN. Las letras de los Strings solo pueden ser: A, T, C, G, las cuales representan cada base nitrogenada del ADN.
Se sabra si un humano es mutante, si encuentra más de una secuencia de cuatro letras iguales, de forma oblicua, horizontal o vertical.

## Niveles a realizar:
- **Nivel 1:** Programa (en cualquier lenguaje de programación) que cumpla con el método pedido por Magneto.

- **Nivel 2:** Crear una API REST, hostear esa API en un cloud computing libre (Google App Engine, 
Amazon AWS, etc), crear el servicio “/mutant/” en donde se pueda detectar si un humano es 
mutante enviando la secuencia de ADN mediante un HTTP POST con un Json.

- **Nivel 3:** Anexar una base de datos, la cual guarde los ADN’s verificados con la API.

## Base de datos H2:

## Deploy en Render

La API se encuentra en Render. Se puede acceder a ella mediante el siguiente enlace:

https://examenparcialmercadolibre.onrender.com/

### Enpoints

- Método **POST**: 
Recibe un arreglo de cadenas que representan una secuencia de ADN en formato JSON y devuelve si la secuencia corresponde a un ADN mutante o humano.

- Método **GET**:
Devuelve la cantidad de ADN humano, la cantidad de ADN mutante y el ratio entre ambos.



