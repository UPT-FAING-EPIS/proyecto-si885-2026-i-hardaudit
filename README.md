# Propuesta de Proyecto: Sistema Automatizado de Auditoría y Análisis de Compatibilidad de Hardware

## 1. Descripción General
El proyecto consiste en una plataforma bajo una arquitectura cliente-servidor diseñada para auditar el hardware de las computadoras de un laboratorio académico de forma automatizada. 

El sistema recolecta especificaciones técnicas de cada equipo (CPU, GPU, RAM, almacenamiento) sin intervención manual, y las compara con una base de datos centralizada que contiene los requisitos mínimos y recomendados de diversos programas de software (como Sketchup, AutoCAD, IDEs de desarrollo, máquinas virtuales, etc.). A partir de esta comparación, se genera un diagnóstico de viabilidad y rendimiento, indicando si los equipos son aptos u óptimos para ejecutar dichos programas.

## 2. Objetivos del Proyecto

*   **Objetivo General:** Desarrollar una herramienta automatizada que evalúe la compatibilidad y el rendimiento del hardware de los equipos de laboratorio frente a los requerimientos de software universitario, facilitando la gestión de la infraestructura tecnológica.
*   **Objetivos Específicos:**
    *   Automatizar la extracción de datos de hardware de los equipos en red.
    *   Crear un motor de reglas y una matriz de compatibilidad basada en los requisitos oficiales del software.
    *   Generar reportes visuales y centralizados sobre el estado de la infraestructura para respaldar la toma de decisiones.


## 3. Módulo de Evaluación y "Scoring" (Valor Agregado)

En lugar de una simple validación de "Sí/No", el sistema implementará un algoritmo de puntuación de compatibilidad para cada programa evaluado:

*   **0% - 49% (Incompatible):** El hardware no cumple con los requisitos mínimos de ejecución.
*   **50% - 79% (Apto / Mínimo):** El programa se puede ejecutar, pero el rendimiento puede verse comprometido en tareas complejas (ej. renderizados pesados).
*   **80% - 100% (Óptimo):** El equipo cumple o supera ampliamente los requisitos recomendados.

## 4. Módulo de Recomendación de Actualizaciones (Upgrades)

Como un impacto económico y administrativo positivo, el sistema detectará cuellos de botella y sugerirá compras específicas. Por ejemplo: *"Aumentar la RAM de 8GB a 16GB en las 15 máquinas del Laboratorio 2 logrará un 100% de compatibilidad con la suite de diseño, evitando la compra de equipos completamente nuevos"*.
