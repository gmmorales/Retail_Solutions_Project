# 📊 Diagnóstico de Retención y Ventas: Retail Solutions X
**Consultores:** Prado, Leila y Morales, Gustavo  
**Estado:** Fase 2 Finalizada - Listo para Informe Ejecutivo

---

## 📝 Descripción del Proyecto
Este proyecto aborda la problemática de la caída de facturación de **Retail Solutions X**. A través de un Análisis Exploratorio de Datos (EDA) sobre una base de 50,000 registros transaccionales (2024-2025), hemos identificado patrones de abandono de clientes (**Churn**) y evaluado el impacto económico de la pérdida de lealtad.

## 📂 Estructura del Proyecto
Basado en estándares de la industria de Ciencia de Datos:

* 📂 `data/`: Contiene los datasets originales y el archivo final `ventas_con_churn_2024_2025.csv`.
* 📂 `docs/`: Documentación del proyecto (Alcance, Diccionario de Datos corregido e Informe Ejecutivo).
* 📂 `notebooks/`: Jupyter Notebook `01_EDA_Retail_Solutions_X.ipynb` con el pipeline de limpieza y análisis.
* 📂 `output/`: Gráficos de impacto financiero y segmentación por categorías.

## 🔍 Hallazgos Clave
1.  **Ticket Promedio de Abandono:** Los clientes en estado de *Churn* tienen un ticket promedio de **$428.95**, solo un 1.02% menor que los clientes activos. Esto indica que estamos perdiendo clientes de valor estándar de forma masiva.
2.  **Distribución del Churn:** El abandono es homogéneo entre categorías (~6.3%), descartando problemas de stock en departamentos específicos.
3.  **Calidad de Datos:** Se realizó una imputación estadística por mediana en el 12% de los datos de edad faltantes para asegurar la integridad del análisis demográfico.



## 🛠️ Requisitos Técnicos
Para replicar este análisis, asegúrate de tener instalado:
* Python 3.8+
* Pandas
* Matplotlib
* Seaborn

```bash
pip install pandas matplotlib seaborn