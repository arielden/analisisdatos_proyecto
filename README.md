# Análisis de Muertes Viales en Argentina (2017-2023)

## Análisis exploratorio (Google colab)
- https://colab.research.google.com/drive/1J2E-ObTL3KheFMkoQ8b5CEx_uIXGJglg?usp=sharing

## Descripción del Proyecto
Este proyecto realiza un análisis exploratorio del dataset "SAT-MV-BU_2017-2023" con registros de hechos viales en Argentina, incluyendo víctimas, imputados, y características geográficas/temporales. El objetivo es identificar patrones de siniestralidad, valores faltantes y distribuciones clave para futuras etapas de visualización y modelado.

## Origen de los Datos
- **Fuente**: [datos.gob.ar](https://datos.gob.ar)  
- **Procesamiento**: Los datos han sido previamente limpiados y estructurados por la entidad pública, con formatos unificados y baja presencia de valores nulos.  
- **Período**: 2017-2023.  

## Datos Clave
- **Fuente**: [SAT-MV-BU (Ministerio de Justicia)](https://datos.gob.ar)
- **Período**: 2017-2023
- **Registros**: +50,000
- **Variables principales**:
  - **Geográficas**: Provincia, localidad, coordenadas (latitud/longitud)
  - **Temporales**: Fecha, hora, mes/año
  - **Eventos**: Tipo de siniestro (colisiones, vuelcos), estado de semáforos
  - **Víctimas/Imputados**: Sexo, edad, tipo de vehículo, rol (peatón/conductor)

## Estructura del Repositorio
├── documentos/ # Informes presentados para las evidencias
└── README.md # Documentación del proyecto

## Requisitos
- Python 3.8+
- Bibliotecas principales: `pandas`, `matplotlib`, `seaborn`, `geopandas`.
- Para replicar el análisis, ejecutar los notebooks en el orden numerado.

## Hallazgos Preliminares
1. **Calidad de Datos**:
   - Columnas numéricas (`latitud`, `longitud`) convertidas y analizadas (media, mediana, nulos).
   - Procesamiento de valores ausentes/errores en columnas categóricas (ej: `"Sin datos"` normalizados).
2. **Distribuciones**:
   - Resumen estadístico de variables numéricas (desviación estándar, porcentaje de nulos).
   - Análisis de IDs geográficos (ej: `provincia_id` con 95% de valores válidos).
3. **Inconsistencias Detectadas**:
   - Columnas como `tipo_persona_id` requieren limpieza adicional (ej: textos mal formateados).

## Contribuciones
¡Las contribuciones son bienvenidas! Por favor, abra un *issue* para discutir mejoras o envíe un *pull request*.

## Licencia
Los datos son públicos bajo [licencia de datos abiertos](https://datos.gob.ar/).

---

**Equipo**:

- Mario Ezequiel Arce
- Valentino Lorenzati
- Alejo Nicolas Terreno
- Ariel Denaro
- Gaston Di Campli
- Simon Azul Sanchez Vottero

Docentes: Nahuel Pratta, Marcos Ugarte
