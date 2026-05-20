# Análisis Exploratorio de Datos (EDA) - Campaña de Marketing Bancario 📊🏦

## 📝 Descripción del Proyecto
Este proyecto consiste en un Análisis Exploratorio de Datos (EDA) completo sobre los resultados de una campaña de marketing telefónico (*telemarketing*) realizada por una institución bancaria. El objetivo principal es identificar qué perfiles demográficos y socioeconómicos tienen una mayor probabilidad de contratar un depósito a plazo fijo, optimizando así futuras estrategias comerciales.

## 🎯 Objetivos
* Unificar y consolidar múltiples bases de datos de clientes y resultados de campañas.
* Limpiar y transformar los datos manejando valores nulos, formatos numéricos europeos y variables categóricas.
* Realizar *Feature Engineering* para crear nuevas variables analíticas.
* Extraer *insights* de negocio mediante visualización avanzada de datos.

## 🛠️ Tecnologías y Librerías Utilizadas
* **Python 3.x**
* **Pandas:** Manipulación, limpieza, agrupaciones (`crosstab`) y cruce de datos (`merge`).
* **NumPy:** Computación vectorizada y creación de variables condicionales (`np.select`).
* **Matplotlib & Seaborn:** Visualización de datos estadísticos y distribuciones continuas.

## 📦 Requisitos e Instalación
Para poder ejecutar este cuaderno de Jupyter en tu entorno local, es necesario tener instalado Python 3.x y las siguientes librerías. 

Puedes instalarlas todas de golpe ejecutando el siguiente comando en tu terminal:

```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

## 📁 Estructura del Repositorio
```text
├── notebooks/
│   └── proyecto_eda.ipynb          # Cuaderno de Jupyter con el código, análisis y gráficas.
├── datos/
│   ├── bank-additional.csv         # Dataset principal con los resultados de la campaña telefónica.
│   └── customer-details.xlsx       # Dataset histórico con los datos personales de los clientes (pestañas 2012, 2013, 2014).
└── README.md                       # Documentación explicativa del proyecto.
```

## 📂 Estructura del Análisis
1. **Integración de Datos:** Concatenación de archivos históricos (2012-2014) y unión con el dataset de la campaña.
2. **Transformación y Limpieza:**
   * Conversión de variables con formato de coma decimal europeo.
   * Estrategia de imputación de nulos específica por tipo de dato (mediana para numéricas continuas, moda para binarias, 'unknown' para categóricas).
3. **Ingeniería de Variables:** Creación de cohortes generacionales (`rango_edad`) a partir de la variable continua.
4. **Análisis y Visualización:** * Análisis del volumen absoluto vs. tasa de conversión relativa.
   * Descubrimiento de nichos de alta rentabilidad (jóvenes, seniors, estudiantes y jubilados) frente a la baja conversión del mercado mayoritario (adultos del sector administrativo).

## 💡 Conclusión Principal
El análisis revela un dataset fuertemente desbalanceado (88.75% rechazo vs. 11.25% aceptación). Se concluye que la estrategia de llamadas masivas al sector mayoritario (adultos 30-50 años) es ineficiente. El banco debe pivotar hacia una segmentación enfocada en clientes fuera del mercado laboral activo tradicional (extremos generacionales), donde la probabilidad de conversión es significativamente superior.


## 👤 Autor
*   **José Manuel López** - [xhemanue](https://github.com/xhemanue)
