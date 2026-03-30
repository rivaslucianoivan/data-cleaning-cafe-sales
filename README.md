#  🧹 Data Cleaning - Cafe Sales Dataset



Proyecto de limpieza y análisis de datos de ventas de un café usando Python y Pandas.  


---

 

## 📋 Problema de negocio

 

Dataset de Kaggle con **10.000 registros de ventas** de un café, intencionalmente "ensuciado" para práctica de data cleaning.

 

**Problemas detectados:**

- ❌ \~40% de valores faltantes en `Location`

- ❌ \~32% de valores faltantes en `Payment Method`

- ❌ Valores inválidos: `"ERROR"`, `"UNKNOWN"`, `"N/A"`

- ❌ Tipos de datos incorrectos (todo como texto)

- ❌ Filas sin información crítica de ventas

 

**Objetivo:** Generar un dataset limpio y confiable listo para análisis de ventas.

 

---

 

## 🛠️ Tecnologías utilizadas

 

- **Python 3.9+**

- **Pandas** - Manipulación y limpieza de datos

- **Matplotlib & Seaborn** - Visualizaciones

- **Jupyter Notebook** - Documentación interactiva

 

---

 

## 📊 Metodología aplicada

| Etapa | Técnica | Resultado |
| --- | --- | --- |
| **EDA** | Análisis exploratorio sistemático | Mapa completo de problemas |
| **Unificación** | Estandarización de valores faltantes | ERROR/UNKNOWN → NaN |
| **Conversión** | Casting de tipos de datos | Numéricos a float, fechas a datetime |
| **Imputación** | Lógica de negocio: `Total = Qty × Price` | Recuperación inteligente de datos |
| **Tratamiento** | Categóricas: NaN → "Unknown" | Preservación de registros |
| **Validación** | Verificación de integridad | Dataset sin inconsistencias |



---

 

## 📈 Resultados

 

✅ **Tasa de recuperación:** ~95% del dataset original (9.500+ filas válidas)  

✅ **Sin valores NaN:** Todos los faltantes fueron tratados apropiadamente  

✅ **Integridad matemática:** Relación `Total Spent = Quantity × Price Per Unit` verificada  

✅ **Listo para análisis:** Tipos correctos, datos consistentes



### Visualizaciones generadas

 

*Ejemplo de insights extraídos del dataset limpio:*

- Evolución temporal de ventas por mes

- Top 10 productos por ingresos

- Distribución de ventas por ubicación y método de pago

- Métricas clave de transacciones

 

---

 

## 🚀 Cómo ejecutar el proyecto

 

```bash

# Clonar el repositorio

git clone https://github.com/TU\_USUARIO/data-cleaning-cafe-sales.git

cd data-cleaning-cafe-sales

 

# Instalar dependencias

pip install -r requirements.txt

 

# Ejecutar el notebook

jupyter notebook notebooks/01\_data\_cleaning.ipynb



