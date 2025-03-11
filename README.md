# Multiplicación de Matrices y Paralelización

Paralelización Sencilla

* 2.1. Idea Principal
    * Dividir el trabajo entre varios procesadores:
      Cada procesador calcula un grupo de filas del resultado.
      Todos necesitan acceso a toda la matriz B

* 2.2. Pasos Básicos
    1. Repartir filas de A entre los procesadores
    2. Enviar copia de B a todos
    3. Cada uno calcula sus filas de C
   4. Reunir todos los resultados
