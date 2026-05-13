
# Modelo de Crédito — Cirugías Plásticas 🏥

Proyecto Final · Modelos de Crédito · Ingeniería Financiera · ITESO

## Descripción

Modelo matemático-financiero implementado en Python para el 
financiamiento de cirugías plásticas electivas en la Zona 
Metropolitana de Guadalajara, México. Estima riesgo crediticio 
bajo el marco de Basilea II e integra un seguro de vida vinculado 
a cada operación.

## Componentes del modelo

| Componente | Modelos utilizados |
|---|---|
| PD — Probabilidad de Default | Regresión Logística + Random Forest |
| LGD — Pérdida Dado el Incumplimiento | Ridge Regression + Random Forest Regressor |
| EL — Pérdida Esperada | EL = PD × LGD × EAD |

## Dataset

LendingClub (2007–2015) · 95,269 préstamos con resultado conocido  
Fuente: [Kaggle — Lending Club Loan Data](https://www.kaggle.com/datasets/utkarshx27/lending-club-loan-dataset)

## Resultados principales

- AUC: 0.8587 · Gini: 0.7175 · KS: 0.5590
- Simulación masiva: 10,000 solicitudes
- Profit neto: $3,530,740 USD · ROE: 14.58%
- Tasa de mora efectiva: 3.6% vs benchmark nacional 4.5%

## Estructura del repositorio
modelo-credito-cirugias-plasticas/
├── modelo_credito_cirugias_v2.ipynb
├── reporte/
│   └── Modelo_de_Credito_Proyecto_Final_Reporte.pdf
├── presentacion/
│   └── Modelos_de_Credito_Presentacion.pdf
└── README.md

## Autores

Mónica Valeria Jáuregui · Mariana Ripoll · Sofia Vazquez Guerrero  
Ricardo Ibarra · Alberto Marin · Luis Fernando Ramirez  
ITESO — Mayo 2026
