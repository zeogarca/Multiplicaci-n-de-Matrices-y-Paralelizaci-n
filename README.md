# Multiplicación de Matrices en Paralelo  y MAtrices de Rotación

**Objetivo General:**  
Crear un programa paralelizado que multiplique matrices grandes de manera eficiente, distribuyendo el trabajo entre múltiples procesadores usando MPI.  

**Hacer**
Saber como haxcer las operaciones para no copiar toda la matriz en cada proceso.
Tener el algoritmo listo para una matriz pequeña para el siguiente mes.
Posiblemente traducir una imagen a una matriz numerica, y después pasarla por una matriz de rotacion


## 📖 ¿Qué es la multiplicación de matrices?  
Operación matemática donde:  
- Se toma una matriz **A** (de tamaño N×M)  
- Se multiplica por una matriz **B** (de tamaño M×P)  
- El resultado es una matriz **C** (de tamaño N×P)  
- Cada elemento de **C** se calcula sumando productos de filas de **A** y columnas de **B**  

## 🎯 ¿Qué hace este proyecto?  
1. **Divide el trabajo**: Reparte filas de la matriz **A** entre distintos procesadores.  
2. **Paraleliza el cálculo**: Cada procesador calcula una parte del resultado **C** usando su porción de **A**. 
3. **Combina resultados**: Reúne todas las partes calculadas para formar la matriz final **C**.  
