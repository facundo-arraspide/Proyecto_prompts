# IA Personal Trainer – Entretejiendo Imaginación y Algoritmos

## Resumen
IA Personal Trainer genera rutinas de entrenamiento personalizadas mediante técnicas de **fast prompting**. El proyecto demuestra un flujo completo **texto→texto** (rutinas generadas por un LLM — Gemini) y **texto→imagen** (prompt para un generador de imágenes), con una POC entregada en Jupyter Notebook.

## Introducción
**Nombre del proyecto:** IA Personal Trainer – Entretejiendo Imaginación y Algoritmos  
**Autor:** Facundo Arraspide  
**Comisión:** 76295

**Problema:** Muchas personas no saben cómo diseñar una rutina personalizada y abandonan por falta de instrucciones o motivación.  
**Solución propuesta:** Usar LLMs para generar rutinas textuales adaptadas a objetivos, restricciones y contexto (ej. invierno en Uruguay) y generar imágenes de apoyo (posters/ejercicios) con herramientas externas (Nightcafe/DALL·E).

## Objetivos
- Diseñar prompts optimizados (fast prompting) para generar rutinas útiles y seguras.  
- Implementar una POC en Jupyter Notebook que muestre la conexión texto→texto con Gemini.  
- Documentar prompts de texto→imagen y aportar la imagen generada como evidencia.

## Metodología
1. Definir casos de usuario (ej.: perder grasa, sin equipamiento, principiantes).  
2. Crear prompt básico y prompt optimizado (role, formato de salida, contexto).  
3. Implementar llamadas a la API (Gemini) para texto→texto; en ausencia de key, el notebook simula respuestas.  
4. Generar imágenes con Nightcafe o DALL·E usando prompts reproducibles; guardar outputs en `/images/`.

## Herramientas y tecnologías
- Google Gemini (Google Gen AI) — texto→texto.  
- Nightcafe o DALL·E — texto→imagen (interfaz web).  
- Jupyter Notebook / Google Colab.  
- Python (requests) para llamadas HTTP al endpoint REST de Generative Language.

## Implementación
- `notebooks/ProyectoFinal_POC_Gemini.ipynb`: Notebook con:
  - plantilla para llamar a Gemini (requiere `GEMINI_API_KEY`),
  - ejemplo de prompt básico y prompt optimizado,
  - lógica de simulación si no hay API key,
  - instrucciones para añadir la imagen generada en `/images/`.
- `images/rutina_generada.png`: Imagen generada externamente (Nightcafe/DALL·E).
- `images/prompt_rutina.txt`: Prompt exacto y ajustes usados para generar la imagen.

### Cómo ejecutar (breve)
1. Abrir el notebook en Colab.  
2. En una celda, dejar seteada la variable `API_KEY` (usa `getpass()` para no exponerla).  
3. Ejecutar celdas: se hará la llamada al endpoint de Gemini y mostrará el texto con la rutina.  
4. Si usaste Nightcafe, guarda la imagen en `/images/` y usa `IPython.display.Image` para verla en el notebook.

## Resultados
- El notebook permite comparar salida de prompt básico vs prompt optimizado y visualizar la mejora con fast prompting.  
- La imagen en `/images/` prueba la parte texto→imagen de la solución.

## Conclusiones
El uso de fast prompting mejora claridad y adaptación de las rutinas. Integrar llamadas reales a Gemini valida la POC; la parte visual puede realizarse con Nightcafe y documentarse en el repo.

## Archivos incluidos
- `README.md`  
- `notebooks/ProyectoFinal_POC_Gemini.ipynb`  
- `images/rutina_generada.png`  
- `images/prompt_rutina.txt`

## Referencias
- Google Gen AI / Gemini docs  
- Nightcafe Creator
