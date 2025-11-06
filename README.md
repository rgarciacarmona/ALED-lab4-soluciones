# ALED (Algorithms and Data Structures) Lab Session 4 - Solution

This repository contains the code for two Java applications:

- One that simulates an ER of a hospital using threads.
- One that performs a parallelized linear search to find a DNA sequence inside a reference genome.

This code is the solution for this lab session: https://github.com/rgarciacarmona/ALED-lab4

## Respuestas a las preguntas

### Sección 1.3

- **En el diagrama, ¿qué significa la flecha que va desde `Patient` hasta `Thread`?:** Que la clase `Patient` es hija de `Thread`.
- **¿Qué metodo de la clase `Patient` no aparece dentro de dicha clase en el diagrama (aparte de `getX()`, `setX()`, `equals()` y `toString()`)? ¿Para qué sirve dicho método? ¿A qué clase pertenece?:** El método `run()`, heredado de `Thread`. Este método es invocado por `start()` cuando se arranca `Patient` como hebra.
- **En esta simulación simplificada de un servicio de Urgencias, ¿los objetos de qué clase se ejecutarán de forma concurrente? ¿Por tanto, qué agentes existen en esta simulación?:** Los objetos de `Patient`. Los agentes serán los pacientes.

### Sección 1.4

- **¿En las líneas que empiezan por la palabra “AREA”, qué significan cada uno de los números y el texto que la siguen?:** La coordenada X, la coordenada Y, el tiempo de espera y el nombre de la sección, respectivamente.
- **¿En las líneas que empiezan por la palabra “PATIENT”, qué significan el número y el texto que la siguen?:** El número y el `Area` en las que empieza el paciente, respectivamente.
- **¿En las líneas que empiezan por la palabra “TRANSFER”, qué significan los dos números y el texto que la siguen?:** El número del `Patient`, el nombre del `Area` hacia la que se mueve y el tiempo que tarda en moverse, respectivamente.

### Sección 2.1

- **¿Cuál debe ser el primer argumento del programa si queremos que se ejecute el servicio de Urgencias que se describe en la Sección 1.4?:** La ubicación en la que se encuentra el archivo que contiene los datos del servicio de Urgencias.

### Sección 3.3

- **¿Cuántos procesadores tiene su equipo?:** Cualquier número entero, normalmente entre 4 y 48.
- **¿Cuántas hebras está usando su nueva búsqueda lineal?:** El mismo número que procesadores tiene el equipo.
- **¿Cuánto se ha reducido el tiempo de ejecución de su nueva búsqueda lineal en comparación con la original? ¿Era lo que esperaba?:** Aproximadamente tantas veces como hebras se han utilizado.