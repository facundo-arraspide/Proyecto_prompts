# IA Personal Trainer – Rutinas y Motivación con Prompts

## Introducción
El proyecto **IA Personal Trainer** busca resolver la dificultad que enfrentan muchas personas al iniciar una rutina de entrenamiento físico: 
- No saben cómo armar un plan acorde a sus objetivos (perder peso, ganar fuerza, mejorar resistencia, etc.).
- Carecen de motivación o acompañamiento personalizado.
- Los tutoriales y rutinas disponibles en internet suelen ser demasiado generales.

Este proyecto propone una solución basada en **prompts inteligentes**, generando rutinas personalizadas de entrenamiento a través de un modelo de IA (texto → texto).  

De esta forma, los usuarios pueden recibir rutinas claras, adaptadas a sus necesidades, junto con explicaciones sencillas de cada ejercicio.

## Propuesta de solución
La solución consiste en utilizar **fast prompting** para diseñar un sistema de rutinas personalizadas con:
- **Instrucciones claras y adaptadas** al nivel del usuario.
- **Variedad de rutinas** (fuerza, cardio, movilidad, estiramientos).
- **Consejos de motivación** y constancia.  

Ejemplo de prompt:
```
Genera una rutina de 20 minutos para alguien que quiere perder grasa, sin saltos ni equipamiento, adaptada al invierno en Uruguay.
```

## Justificación de la viabilidad
- **Recursos**: uso de ChatGPT (texto → texto).  
- **Tiempo**: es factible dentro del curso, ya que solo se necesitan prompts y un entorno simple (Notebook).  
- **Limitaciones**: el modelo no sustituye a un entrenador humano, pero sí ayuda a principiantes.  
- **Viabilidad técnica**: no requiere hardware especial, solo conexión a internet y acceso a un modelo de lenguaje.  

## Objetivos
- Desarrollar un sistema de prompts para crear rutinas de entrenamiento personalizadas.  
- Demostrar cómo el **fast prompting** optimiza la generación de respuestas.  
- Probar la viabilidad de la solución con una **POC en Jupyter Notebook**.  

## Metodología
1. Definir casos de usuario (ej: perder peso, mejorar resistencia, entrenamiento sin equipamiento).  
2. Diseñar prompts básicos.  
3. Optimizar con técnicas de **fast prompting** (role prompting, chain-of-thought simplificado, instrucciones claras y concisas).  
4. Implementar pruebas en Notebook.  

## Herramientas y tecnologías
- **ChatGPT / OpenAI API** para prompts texto → texto.  
- **Jupyter Notebook** para la POC.  
- **Fast Prompting**: redacción precisa, estructuración de instrucciones y roles.  

## Implementación
En el notebook se incluyen:
- Ejemplos de prompts básicos.  
- Optimización con fast prompting.  
- Comparación entre resultados.
- Ejemplos de prompts básicos.  
- Optimización con fast prompting.  
- Comparación entre resultados.
