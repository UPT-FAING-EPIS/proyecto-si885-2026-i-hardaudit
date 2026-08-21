# Propuesta de Proyecto: Sistema Automatizado de Auditoría y Análisis de Compatibilidad de Hardware

## 1. Planteamiento del Problema
En la actualidad, tanto instituciones educativas como corporativas enfrentan un desfase constante entre el hardware de sus equipos y los requerimientos cada vez más exigentes del software moderno (herramientas de diseño, simulación, desarrollo, etc.). 

El problema principal radica en el **desconocimiento del estado real y la capacidad operativa de la infraestructura tecnológica**. Las auditorías de hardware tradicionales suelen realizarse de forma manual, lo que resulta en un proceso lento, propenso a errores y que se desactualiza rápidamente. Como consecuencia, las organizaciones sufren pérdidas de productividad debido a equipos lentos, o realizan inversiones a ciegas, reemplazando computadoras enteras cuando una simple actualización de componentes habría solucionado el problema.

## 2. Impacto y Valor para las Empresas
Aunque el proyecto nace para laboratorios académicos, su aplicación en el sector empresarial resuelve problemas críticos de gestión de TI, generando el siguiente impacto:

*   **Optimización de Presupuesto (Ahorro de Costos):** Al identificar exactamente qué componente es el "cuello de botella" (por ejemplo, falta de RAM o un disco HDD lento), la empresa invierte en actualizaciones estratégicas (upgrades) en lugar de comprar flotas completas de hardware nuevo.
*   **Mejora en la Productividad del Personal:** Garantiza que los empleados trabajen con herramientas que fluyen adecuadamente, eliminando los "tiempos muertos" o frustraciones causadas por el software que se congela.
*   **Toma de Decisiones Basada en Datos:** Permite a los gerentes de TI planificar las compras y renovaciones tecnológicas con reportes visuales exactos en tiempo real, en lugar de basarse en suposiciones.
*   **Reasignación Inteligente de Equipos:** Maximiza el retorno de inversión (ROI) al identificar si una computadora que ya no sirve para un área pesada (ej. Arquitectura) sigue siendo 100% óptima para tareas de otra área (ej. Contabilidad o Administración), alargando su vida útil.

*   
## 3. Descripción General
El proyecto consiste en una plataforma bajo una arquitectura cliente-servidor diseñada para auditar el hardware de las computadoras de un laboratorio académico de forma automatizada. 

El sistema recolecta especificaciones técnicas de cada equipo (CPU, GPU, RAM, almacenamiento) sin intervención manual, y las compara con una base de datos centralizada que contiene los requisitos mínimos y recomendados de diversos programas de software (como Sketchup, AutoCAD, IDEs de desarrollo, máquinas virtuales, etc.). A partir de esta comparación, se genera un diagnóstico de viabilidad y rendimiento, indicando si los equipos son aptos u óptimos para ejecutar dichos programas.

## 4. Objetivos del Proyecto

*   **Objetivo General:** Desarrollar una herramienta automatizada que evalúe la compatibilidad y el rendimiento del hardware de los equipos de laboratorio frente a los requerimientos de software universitario, facilitando la gestión de la infraestructura tecnológica.
*   **Objetivos Específicos:**
    *   Automatizar la extracción de datos de hardware de los equipos en red.
    *   Crear un motor de reglas y una matriz de compatibilidad basada en los requisitos oficiales del software.
    *   Generar reportes visuales y centralizados sobre el estado de la infraestructura para respaldar la toma de decisiones.


## 5. Módulo de Evaluación y "Scoring" (Valor Agregado)

En lugar de una simple validación de "Sí/No", el sistema implementará un algoritmo de puntuación de compatibilidad para cada programa evaluado:

*   **0% - 49% (Incompatible):** El hardware no cumple con los requisitos mínimos de ejecución.
*   **50% - 79% (Apto / Mínimo):** El programa se puede ejecutar, pero el rendimiento puede verse comprometido en tareas complejas (ej. renderizados pesados).
*   **80% - 100% (Óptimo):** El equipo cumple o supera ampliamente los requisitos recomendados.

## 6. Módulo de Recomendación de Actualizaciones (Upgrades)

Como un impacto económico y administrativo positivo, el sistema detectará cuellos de botella y sugerirá compras específicas. Por ejemplo: *"Aumentar la RAM de 8GB a 16GB en las 15 máquinas del Laboratorio 2 logrará un 100% de compatibilidad con la suite de diseño, evitando la compra de equipos completamente nuevos"*.
