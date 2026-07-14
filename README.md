# 🚢 Optimización Logística de Exportación Marítima - Andes Pacific Shipping

## 📌 Contexto del Proyecto
Desarrollo de un modelo analítico de optimización lineal para programar el plan semanal de exportación de **1,400 contenedores** desde 4 puertos estratégicos del Perú (Callao, Paita, Matarani y el nuevo puerto de Chancay) hacia los mercados internacionales de Los Ángeles y Shanghái. 

El objetivo principal es **minimizar el costo logístico global semanal total**, garantizando al mismo tiempo el cumplimiento estricto de límites presupuestarios (máx. US$ 2,250,000), capacidades operativas de los terminales, ventanas operativas de tránsito y políticas de gestión de riesgos para evitar la sobreconcentración en Chancay.

---

## 🛠️ Stack Tecnológico Utilizado
* **Lenguaje principal:** Python 3.x (Desarrollado en Google Colab)
* **Librería de Optimización:** `scipy.optimize` (Módulos `linprog`)
* **Procesamiento de Datos:** `pandas` y `numpy`
* **Visualización de Datos:** `matplotlib` y `seaborn`

---

## 📊 Principales Hallazgos y Conclusiones de Negocio

Tras implementar el solucionador de programación lineal con el método `HiGHS`, se lograron extraer las siguientes conclusiones clave de cara a la toma de decisiones gerenciales:

1. **Eficiencia Financiera Significativa:** El modelo determinó una asignación óptima con un costo logístico mínimo total de **US$ 2,164,770.00**, lo que representa un ahorro directo de **US$ 85,230.00** respecto al presupuesto límite de la compañía.
2. **Identificación de Cuellos de Botella Operativos:** Los puertos de **Callao (520 TEUs)**, **Paita (280 TEUs)** y **Chancay (460 TEUs)** terminaron operando al **100% de su capacidad máxima permitida**, actuando como restricciones activas dentro de la red. Cualquier disrupción en estas terminales alteraría críticamente los costos totales de exportación.
3. **Flexibilidad Estratégica en el Sur:** El puerto de **Matarani** registró una utilización de apenas el **58.33%**, dejando una holgura disponible de 100 contenedores. Esto lo posiciona como la única alternativa logística de contingencia ante incrementos inesperados en la demanda comercial hacia Los Ángeles.
