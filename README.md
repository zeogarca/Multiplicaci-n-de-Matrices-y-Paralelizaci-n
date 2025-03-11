# Multiplicación de Matrices en Paralelo  

**Objetivo General:**  
Crear un programa paralelizado que multiplique matrices grandes de manera eficiente, distribuyendo el trabajo entre múltiples procesadores usando MPI.  

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
