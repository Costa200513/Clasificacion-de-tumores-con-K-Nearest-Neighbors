# Clasificación de Tumores con k-Nearest Neighbors (k-NN)

## Introducción

Este proyecto utiliza un modelo de clasificación **k-Nearest Neighbors (k-NN)** para predecir si un tumor es **Benigno** o **Maligno** a partir de características clínicas obtenidas de imágenes de tejido mamario.

El modelo se entrena con tres variables principales del dataset: `radius_mean`, `perimeter_mean` y `area_mean`.  
El objetivo es permitir que, ingresando manualmente valores de estas características, el sistema realice una predicción del tipo de tumor.

## Justificación de la elección de variables

- **radius_mean:** refleja el tamaño promedio de las células.  
- **perimeter_mean:** asociado al contorno de las células.  
- **area_mean:** mide la extensión de las células.  

## Casos de prueba

### 1️⃣ Tumor Benigno

- **radius_mean:** 12.5  
- **perimeter_mean:** 80  
- **area_mean:** 500  

**Diagnóstico estimado:** Benigno  

![Tumor Benigno](https://github.com/user-attachments/assets/db2045eb-4c3e-4a65-b72a-fbf970b653b0)  

> Valores relativamente bajos sugieren que las células son pequeñas y regulares.

### 2️⃣ Tumor Maligno

- **radius_mean:** 20.5  
- **perimeter_mean:** 130  
- **area_mean:** 1200  

**Diagnóstico estimado:** Maligno  

![Tumor Maligno](https://github.com/user-attachments/assets/edd722bf-d7c8-4fad-9403-3d287c356d89)  

> Valores altos en todas las variables, típicos de tumores malignos.

## Conclusión

El modelo k-NN muestra que las variables `radius_mean`, `perimeter_mean` y `area_mean` son determinantes en la clasificación de tumores:

- Tumores con valores bajos en estas variables suelen ser **Benignos**.  
- Tumores con valores altos en estas variables suelen ser **Malignos**.

