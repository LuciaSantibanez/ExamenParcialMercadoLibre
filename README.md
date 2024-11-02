# 🧬 PARCIAL DESARROLLO DE SOFTWARE - Detección de ADN Mutante 🧬

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

## ⚙️Funcionamiento 

Se recibe como parámetro un array de String que representan cada fila de una tabla de (NxN) con la secuancia del ADN. Las letras de los Strings solo pueden ser: A, T, C, G, las cuales representan cada base nitrogenada del ADN.
Se sabra si un humano es mutante, si encuentra más de una secuencia de cuatro letras iguales, de forma oblicua, horizontal o vertical.

## Niveles realizados:
- ### 📌 Nivel 1:
  
  Programa en JAVA que cumpla con el método pedido por Magneto.

- ### 📌 Nivel 2:
  
    API REST para detectar mutantes, deployada en Render. Se puede acceder a ella mediante el siguiente enlace:
https://examenparcialmercadolibre.onrender.com/

    **🌐 Enpoints**

    - Método **POST** /mutant: 
Recibe un array de cadenas que representan una secuencia de ADN en formato JSON a verificar.

        https://examenparcialmercadolibre.onrender.com/mutant

        Formato del body:
        ```json
        {
            "dna": [
                "ATGCGA",
                "CAGTGC",
                "TTATGT",
                "AGAAGG",
                "CCCCTA",
                "TCACTG"
            ]
        }
        ```
        
    - Método **GET** /stats: 
    Devuelve la cantidad de ADN humano, la cantidad de ADN mutante y el ratio entre ambos.

        https://examenparcialmercadolibre.onrender.com/stats

        Formato de respuesta:

        ```json
        {
        "ratio": 4.0,
        "count_mutant_dna": 8,
        "count_human_dna": 2
        }
        ```

- ### 📌 Nivel 3:
  
  Anexar una base de datos, la cual guarde los ADN’s verificados con la API.

 **✔️ Base de datos H2:**

<div ; height: auto; display: flex; justify-content: space-around;">
    <img src="https://github.com/user-attachments/assets/992d10ec-dd8b-43cf-ba7b-aeea57431348" alt="Imagen 1" style="width: auto; height: 300px;">
    <img src="https://github.com/user-attachments/assets/0f2118d4-45e7-4bc1-a492-1b64b5d02fb5" alt="Imagen 2" style="width: auto; height: 300px;">
</div>

  **✔️ Test en Jmeter**

<div ; height: auto; display: flex; justify-content: space-around;">

  <img src="https://github.com/user-attachments/assets/9b03d846-950b-40ab-9778-f4730074aa6c" alt="Imagen 1" style="width: 800px; height: auto;"/>
  <img src="https://github.com/user-attachments/assets/af3e40d2-671d-472c-81f5-5c604edaffeb" alt="Imagen 1" style="width: 800px; height: auto;"/>

</div>

**✔️ Pruebas**

Se utiliza Postman para realizar pruebas de la API. En el proyecto, se proporciona el archivo MercadoLibre.postman_collection.json, el cual incluye:

  - Una petición POST que contiene un ejemplo de secuencia de ADN mutante, diseñada para verificar si el sistema detecta correctamente a un mutante.
  - Una petición GET que muestra las estadísticas de las verificaciones de ADN realizadas, ofreciendo un resumen de cuántas secuencias se han identificado como mutantes o no mutantes.

  **✔️ Diagramas de secuencias**

  <img src="https://github.com/user-attachments/assets/068c9cd2-7237-4483-9690-8c8c97065f33" alt="Imagen 1" style="width: 800px; height: auto;"/>
  <img src="https://github.com/user-attachments/assets/e8bb7008-f98d-423a-af40-531ae982305b" alt="Imagen 1" style="width: 800px; height: auto;"/>









