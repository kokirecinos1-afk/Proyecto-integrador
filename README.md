# Proyecto-integrador
Proyecto integrador curso python kodigo
proyecto-integrador-m4/
├── README.md               # Carta de presentación del proyecto (se actualizará en las siguientes semanas)
├── LICENSE                 # Archivo de licencia (ej. MIT)
├── .gitignore              # Archivo para ignorar datos pesados y caché
├── .dockerignore           # Archivo para ignorar archivos innecesarios en Docker
├── requirements.txt        # Dependencias fijadas del proyecto[cite: 3, 5]
├── Dockerfile              # Configuración para contenedorizar la API[cite: 5]
├── data/
│   ├── raw/                # Datos crudos (no se suben a GitHub)[cite: 8]
│   ├── processed/          # Datos transformados[cite: 8]
│   └── muestra/            # Muestra pequeña incluida para pruebas rápidas[cite: 8]
├── notebooks/              # Cuadernos de exploración (EDA)[cite: 8]
├── src/                    # Código fuente modular
│   ├── ingesta/            # Scripts de Dask / PySpark[cite: 8]
│   ├── almacenamiento/     # Conexión a MongoDB y S3 simulado[cite: 8]
│   ├── modelos/            # Clases POO y entrenamiento de modelos[cite: 8]
│   └── api/                # Endpoints con FastAPI (main.py)[cite: 5, 8]
├── tests/                  # Pruebas unitarias con pytest[cite: 5, 8]
├── docs/                   # Documentación y registro de decisiones (decisiones.md)[cite: 8]
└── reports/
    └── figures/            # Gráficos y capturas para el README[cite: 8]
