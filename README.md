# 📊 Diagnóstico de Retención y Ventas: Retail Solutions X
**Consultores:** Prado, Leila y Morales, Gustavo  
**Estado:** Finalizado

---

## 📝 Descripción del Proyecto
Este proyecto aborda la problemática de la caída de facturación de **Retail Solutions X**. A través de un Análisis Exploratorio de Datos (EDA) sobre una base de 50,000 registros transaccionales (2024-2025), hemos identificado patrones de abandono de clientes (**Churn**) y evaluado el impacto económico de la pérdida de lealtad.

## 📂 Estructura del Proyecto
Basado en estándares de la industria de Ciencia de Datos:

* 📂 `data/`: Contiene los datasets originales y el archivo final `ventas_con_churn_2024_2025.csv`.
* 📂 `docs/`: Documentación del proyecto (Alcance, Diccionario de Datos corregido e Informe Ejecutivo).
* 📂 `notebooks/`: Jupyter Notebook `01_EDA_Retail_Solutions_X.ipynb` con el pipeline de limpieza y análisis.
* 📂 `output/`: Gráficos de impacto financiero y segmentación por categorías.

## ⚙️ Configuración del Entorno (Environment)
Para replicar este entorno de manera idéntica, puedes optar por Conda (recomendado para Ciencia de Datos) o Pip.

Opción A: Importación con Conda (Recomendado)
Si tienes Anaconda o Miniconda instalado, utiliza el archivo environment.yml incluido en la raíz:
1. Crear e importar el entorno:
    <pre>
        conda env create -f environment.yml
    </pre>    

2. Activar el entorno:
    <pre>
        conda activate env_retail
    </pre>


Opción B: Entorno Virtual con Pip
Si prefieres no usar Conda, puedes crear un entorno estándar de Python:
1. Crear el entorno: 
    <pre>
        python -m venv env_retail
    </pre>
2. Activar el entorno: 
    - Windows:
    <pre>
        env_retail\Scripts\activate
    </pre> 

    - Mac/Linux:
    <pre>
        source env_retail/bin/activate
    </pre>

3. Instalar dependencias:
    <pre>
        pip install pandas matplotlib seaborn numpy jupyter
    </pre>

## 🔍 Hallazgos Clave
1.  **Ticket Promedio de Abandono:** Los clientes en estado de *Churn* tienen un ticket promedio de **$428.95**, solo un 1.02% menor que los clientes activos. Esto indica que estamos perdiendo clientes de valor estándar de forma masiva.
2.  **Distribución del Churn:** El abandono es homogéneo entre categorías (~6.3%), descartando problemas de stock en departamentos específicos.
3.  **Calidad de Datos:** Se realizó una imputación estadística por mediana en el 12% de los datos de edad faltantes para asegurar la integridad del análisis demográfico.