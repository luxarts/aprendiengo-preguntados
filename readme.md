# Preguntados

## Objetivo
Hacer un programa que haga preguntas y el usuario deba seleccionar la opción correcta.
Al final del programa se mostrarán los resultados obtenidos. Por ejemplo:

```
Respondiste 6 preguntas correctas de 10.
```

## Características
- Las preguntas y respuestas se ingresaran al programa mediante un archivo `csv` especificado con el flag `-f` con el siguiente formato:
    ```
    pregunta,opción a,opción b,opción c,opción d,opción correcta
    ```
    Ejemplo:
    ```
    ¿Cuál de estos números es par?,1,3,5,2,d
    ¿Cuál es el nombre del papá de Bart Simpson?,Apu,Krusty,Homero,Moe,c
    ```
- El usuario tendrá un tiempo de 30 segundos para responder cada pregunta o podrá ser especificado en segundos con el flag `-t`. En caso de que el tiempo se acabe el programa debe terminar y mostrar los resultados.
    Ejemplo:
    ```
    ¿Cuál es el nombre del papá de Bart Simpson?
    A) Apu
    B) Krusty
    C) Homero
    D) Moe
    Tiempo restante 0 segundos
    --------------------------
    Respondiste 6 preguntas correctas de 10.
    ```
- Al iniciar el programa una cuenta regresiva se mostrará para darle tiempo al usuario a prepararse.
    Ejemplo:
    ```
    3
    2
    1
    ¡YA!
    ```

## Ejemplo de uso
```
preguntados -f preguntas.csv -t 10
```