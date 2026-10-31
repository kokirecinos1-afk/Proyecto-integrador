# Proyecto-integrador
**Proyecto integrador curso python kodigo**
*Título: Proyecto Integrador - Análisis de Sentimiento de Clientes*
*Autor: Josue Recinos
*Descripción: Aplicación modular desarrollada en Python que procesa un dataset masivo de reseñas mediante procesamiento paralelo (Dask), simula almacenamiento de datos NoSQL (MongoDB / mongomock), implementa un modelo de clasificación de texto con Scikit-Learn bajo principios de Programación Orientada a Objetos (POO), y expone los resultados a través de una API web con FastAPI.
*Tecnologías utilizadas: Python, Dask, Pandas, Scikit-Learn, FastAPI, Mongomock


---

## Bitácora de Desarrollo
* **Exploración de datos:** Carga inicial de 10,000 registros de feedback y validación de columnas clave (`comentario`, `calificacion`).
* **Optimización con Dask:** Uso de procesamiento en bloques (`blocksize="1MB"`) para evitar saturación de memoria en operaciones distribuidas.
* **Decisiones de Arquitectura:** 
  * Se implementó persistencia NoSQL simulada (`mongomock` / MongoDB) para manejar estructuras JSON y consultas complejas (`$gt`).
  * Se estructuró el modelo de Machine Learning (TF-IDF + Regresión Logística) dentro de un `Pipeline` de Scikit-Learn para evitar fugas de datos (*data leakage*), aplicando Programación Orientada a Objetos (POO).

---

## Evaluación de Usuario (Design Thinking - Marco HPI)
1. **Empatizar:** Identificar la necesidad de automatizar la lectura masiva de reseñas para entender rápidamente la satisfacción del cliente.
2. **Definir:** La dificultad de procesar manualmente miles de comentarios en tiempo real para la toma de decisiones comerciales.
3. **Idear:** Desarrollar un pipeline técnico modular que combine procesamiento paralelo, clasificación por IA y una API web.
4. **Prototipar:** Construcción del flujo completo (Dask Modelo POO API con FastAPI).
5. **Evaluar:** Pruebas automatizadas y validación de respuestas de la API en milisegundos con alta precisión operativa.

---

## Evaluación Tecnológica, Financiera y ROI
* **Viabilidad Técnica:** Uso de tecnologías de código abierto (*open-source*) altamente modulares y de fácil mantenimiento en Python.
* **Costes de Infraestructura:** 
  * *Fase de desarrollo:* $0 (Entorno local / Google Colab).
  * *Fase productiva (Nube estimada):* Servidor ligero en la nube (ej. AWS EC2 o Render) entre $10 - $25 USD al mes (~$120 - $300 USD anuales).
* **Retorno de Inversión (ROI):** La automatización reduce en un 90% el tiempo de análisis manual de reseñas (valorado en ~$7,200 USD anuales en horas hombre), amortizando la inversión en infraestructura en menos de dos semanas y generando un flujo de caja altamente positivo.
