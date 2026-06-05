# Resumen de Repositorios - python_CODE

Este documento proporciona un resumen de los propósitos y funcionalidades de cada repositorio consolidado en `python_CODE`.

---

## 📊 Estructura del Proyecto

```
python_CODE/
├── ensamblefinance/    - Predicción de volatilidad financiera
├── MsEntropy/          - Agrupaciones por Entropía
├── MTC/                - Tratamiento de Missing Values (Target Continuo)
├── MsNAIVE/            - Tratamiento de Missing Values (Target Discreto)
└── RESUMEN_REPOSITORIOS.md
```

---

## 📌 Descripción de Cada Repositorio

### 1. **ensamblefinance** 
**Objetivo:** Predicción de volatilidad de activos financieros

- **Descripción:** Combina dos técnicas avanzadas para la predicción de volatilidad:
  - **EWMA** (Exponentially Weighted Moving Average)
  - **Procesos Estocásticos**
  
- **Caso de uso:** Análisis y pronóstico de volatilidad en mercados financieros
- **Archivos principales:**
  - `Ensamble de Modelos - Finanzas.ipynb` - Notebook con ejemplos prácticos

---

### 2. **MsEntropy**
**Objetivo:** Agrupaciones basadas en Entropía

- **Descripción:** Código que realiza agrupaciones aplicando el concepto de Entropía, minimizando el caos entre agrupaciones
- **Características:**
  - Soporta targets dicotómicos (binarios)
  - Soporta targets categóricos (múltiples clases)
  
- **Estado:** En desarrollo 🔄
- **Archivos principales:**
  - `README.md` - Documentación

---

### 3. **MTC (Missing Treatment Continuous)**
**Objetivo:** Imputación de valores faltantes con target continuo

- **Descripción:** Herramienta para tratamiento de missing values usando regresión simple
- **Metodología:**
  - Realiza regresión simple entre variable target (y) y variable a imputar (x)
  - Específicamente diseñada para targets **continuos**
  
- **Configuración:**
  - `umbral_unique` - Umbral para diferenciar variables categóricas de continuas
  - `umbral_nan` - Umbral de missing values para considerar en imputación
  - `variable_y` - Variable target (continua)
  - `variable_x` - Variable(s) a imputar
  - `muestra` - División TRAIN/TEST
  
- **Versión:** 1.0 (09/2022)
- **Archivos principales:**
  - `código_MTC.py` - Código principal
  - `Cód Ej. MTC.ipynb` - Ejemplos prácticos
  - `BD MTC.xlsx` - Base de datos de ejemplo

---

### 4. **MsNAIVE (Missing Naive)**
**Objetivo:** Imputación naive de valores faltantes con target discreto

- **Descripción:** Herramienta para tratamiento de missing values usando método naive
- **Metodología:**
  - Calcula la mediana de la variable x en función de la clase target (y)
  - Imputa los NaN de las variables x usando estas medianas
  - Específicamente diseñada para targets **discretos o categóricos**
  
- **Configuración:**
  - `umbral_unique` - Umbral para diferenciar variables categóricas de continuas
  - `umbral_nan` - Umbral de missing values para considerar en imputación
  - `variable_y` - Variable target (discreto/categórico) ⚠️ **IMPORTANTE**
  - `variable_x` - Variable(s) a imputar
  - `muestra` - División TRAIN/TEST
  - `ventana` - Ventana de cálculo (TRAIN o TEST)
  
- **Versión:** 1.0 (09/2022)
- **Archivos principales:**
  - `código_MsNAIVE.py` - Código principal
  - `MsNAIVE.ipynb` - Ejemplos prácticos
  - `BD MsNAIVE.xlsx` - Base de datos de ejemplo

---

## 🎯 Casos de Uso

| Repositorio | Caso de Uso | Target | Estado |
|---|---|---|---|
| **ensamblefinance** | Predicción de volatilidad financiera | N/A | ✅ Listo |
| **MsEntropy** | Agrupaciones inteligentes | Dicotómico/Categórico | 🔄 En desarrollo |
| **MTC** | Imputación de missing values | Continuo | ✅ Listo |
| **MsNAIVE** | Imputación naive de missing values | Discreto/Categórico | ✅ Listo |

---

## 📚 Recursos Externos

- **Franco A. Mansilla Ibañez** - Autor de todos los módulos
- Website: https://www.francomansilla.com
- Blog Medium: [Regresión: Método para tratamiento de Missing Value](https://medium.com/@fmansillaib/)
- Google Drive con ejemplos y bases de datos: Disponible en los READMEs de cada repositorio

---

## 🚀 Próximos Pasos

1. Completar el desarrollo de **MsEntropy**
2. Crear documentación unificada
3. Considerar crear un módulo unificado que exporte todas las funciones
4. Agregar tests unitarios

---

*Última actualización: Junio 5, 2026*
