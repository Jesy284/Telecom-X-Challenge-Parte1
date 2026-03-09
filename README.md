[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-1.5+-red.svg)](https://pandas.pydata.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

EXTRACCIÓN: Datos descargados desde API JSON oficial
TRANSFORMACIÓN:
Limpieza de valores nulos y conversión de tipos
Renombrado de columnas para legibilidad
ANÁLISIS:
Estadísticas descriptivas univariadas y bivariadas
Visualizaciones con matplotlib y seaborn
CONCLUSIONES: Insights basados en evidencia de datos

**Herramientas utilizadas**: Python, Pandas, Matplotlib, Seaborn, Google Colab


## 📁 Archivos del Proyecto
Telecom-X-Challenge/
├── 📄 Telecom-X-Analisis.ipynb ← Este notebook
├── 📄 datos_limpios.csv ← Dataset procesado (opcional)
├── 📄 README.md ← Documentación del proyecto
└── 📁 images/ ← Gráficas exportadas (opcional)

## 🔍 Conclusiones Principales

### 1️⃣ El tipo de contrato es el predictor más fuerte de churn
- Los clientes con contrato **"Mes a mes"** presentan una tasa de cancelación del **~42%**, significativamente mayor que aquellos con contratos anuales (~11%) o bianuales (~3%).
- Esto sugiere que la flexibilidad contractual, aunque atractiva para el cliente, incrementa sustancialmente el riesgo de fuga.

### 2️⃣ La antigüedad del cliente es un factor crítico de retención
- Los clientes con **menos de 12 meses** de antigüedad tienen una probabilidad de cancelación **2.1 veces mayor** que aquellos con más de 36 meses.
- El primer año de relación con el cliente representa la ventana de mayor vulnerabilidad para la empresa.

### 3️⃣ Los cargos mensuales elevados correlacionan con mayor churn
- Los clientes que cancelaron tienen un cargo mensual promedio de **$74.44**, frente a **$61.27** en clientes activos.
- Esto indica que los clientes perciben un desajuste entre el valor recibido y el precio pagado en planes de mayor costo.

### 4️⃣ El método de pago influye en la permanencia del cliente
- Los clientes que utilizan **cheque electrónico** presentan una tasa de cancelación del ~35%, mientras que aquellos con pagos automáticos (tarjeta o transferencia) muestran tasas inferiores al ~18%.
- La fricción en el proceso de pago manual parece contribuir al abandono del servicio.

| Métrica | Valor | Interpretación |
|---------|-------|---------------|
| Tasa global de churn | 26.6% | 1 de cada 4 clientes cancela |
| Churn en contratos mensuales | ~42% | Riesgo 4x mayor vs. contrato anual |
| Antigüedad promedio (churn) | 17.98 meses | Clientes nuevos son más vulnerables |
| Cargo mensual promedio (churn) | $74.44 | Precio percibido como barrera |

[Distribución de Churn por Tipo de Contrato]
 Los clientes con contrato "Mes a mes" representan la mayor proporción de cancelaciones*


## 🔍 Conclusiones del Análisis

### Hallazgos Principales

1. **Tasa de Churn del 26.6%**
   - Más de 1 de cada 4 clientes cancela el servicio
   - Esto representa un problema significativo para la empresa

2. **Tipo de Contrato - Factor MÁS CRÍTICO**
   - Contratos "Month-to-month": 42.7% de cancelación
   - Contratos "One year": 11.3% de cancelación  
   - Contratos "Two year": 2.8% de cancelación
   - **Los clientes mensuales tienen 15x más probabilidad de cancelar**

3. **Antigüedad del Cliente**
   - Los clientes que cancelaron tienen menor antigüedad (mediana ~10 meses)
   - Los clientes leales (>38 meses) tienden a permanecer
   - **El primer año es crítico para la retención**

4. **Cargo Mensual**
   - Los clientes que cancelaron tienen diferentes patrones de cargo
   - Se requiere análisis más profundo para identificar el punto óptimo de precio

5.  El 26.6% de los clientes cancelaron el servicio*


## 💡 Recomendaciones Estratégicas

### Prioridad 1: Convertir contratos mensuales a anuales
- Ofrecer descuento del 15% por contrato anual
- Beneficio: Mes gratis en contrato de 2 años
- Impacto potencial: Reducir churn de 42.7% a ~11%

### Prioridad 2: Programa de retención para clientes nuevos
- Contacto proactivo en meses 1, 3, 6 y 9
- Encuestas de satisfacción
- Ofertas de fidelización temprana

### Prioridad 3: Revisar estructura de precios
- Analizar si los cargos mensuales altos justifican el valor percibido
- Considerar planes intermedios

## 📊 Métricas Clave

| Métrica | Valor |
|---------|-------|
| Tasa global de churn | 26.6% |
| Churn en contratos mensuales | 42.7% |
| Churn en contratos anuales | 11.3% |
| Churn en contratos 2 años | 2.8% |

## 💡 Recomendaciones de Negocio

### 🎯 Priorizar retención en clientes nuevos (<12 meses)
- Implementar un **programa de onboarding** con contacto proactivo en los meses 1, 3, 6 y 9.
- Ofrecer beneficios de fidelización temprana: descuentos progresivos, servicios adicionales gratuitos o upgrades temporales.
- Establecer alertas automáticas para identificar clientes nuevos con señales de riesgo (quejas, reducción de uso, etc.).

### 🔄 Incentivar la migración a contratos de largo plazo
- Diseñar campañas dirigidas a clientes "Mes a mes" con ofertas de conversión: 
  - 10-15% de descuento por firmar contrato anual
  - 1 mes gratis por contrato bianual
  - Beneficios exclusivos (soporte prioritario, datos adicionales, etc.)
- Comunicar claramente el ahorro acumulado y la estabilidad de precio como ventajas competitivas.

### 💳 Simplificar y automatizar los métodos de pago
- Promover activamente la configuración de pagos automáticos mediante:
  - Descuento del 5% en la primera factura con débito automático
  - Recordatorios amigables y multicanal antes del vencimiento
  - Asistencia personalizada para configurar el método de pago preferido
- Reducir la dependencia del cheque electrónico mediante incentivos y educación al cliente.

  

> **Autor**: Jesica Sosa G 
> **Programa**: Alura ONE - Data Science LATAM  
> **Fecha**: 08/03/2026  
> **Repositorio**: https://github.com/Jesy284/Telecom-X-Challenge-Parte1

*Análisis realizado con fines educativos como parte del Challenge Telecom X*

## 🚀 Cómo Ejecutar el Proyecto

### Opción 1: Google Colab (Recomendado)
1. Abre [Google Colab](https://colab.research.google.com)
2. Ve a **Archivo → Abrir notebook → GitHub**
3. Busca: `Jesy284/Telecom-X-Challenge-Parte1`
4. Selecciona `Telecom_X_Challenge_Parte1.ipynb`
5. Ejecuta celda por celda con `Shift + Enter`

### Opción 2: Jupyter Notebook Local
```bash
# Clonar el repositorio
git clone https://github.com/Jesy284/Telecom-X-Challenge-Parte1.git
cd Telecom-X-Challenge-Parte1

# Instalar dependencias
pip install pandas matplotlib seaborn requests

# Abrir notebook
jupyter notebook Telecom_X_Challenge_Parte1.ipynb
