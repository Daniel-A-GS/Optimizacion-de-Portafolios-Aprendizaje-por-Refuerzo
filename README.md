# Optimización de Portafolios con Aprendizaje por Refuerzo | Proximal Policy Optimization

**Autor:** Daniel García Sánchez - [LinkedIn](https://www.linkedin.com/in/daniel-garcia-data-analyst/)

## Descripción del Proyecto

Implementación del algoritmo Proximal Policy Optimization (PPO) para la optimización de un portafolio financieros, maximizando ganancias mientras se mantiene un perfil de riesgo controlado. El algoritmo aprende a distribuir capital entre 10 acciones del Nasdaq100 de manera óptima.

## Resultados Destacados

### Métricas de Performance

| Métrica | Valor |
|---------|-------|
| **Accumulative Portfolio Value** | **144.6%** |
| **Sharpe Ratio** | **1.50** |
| **Max Drawdown** | **-8.68%** |
| **Calmar Ratio** | **2.10** |
| **Omega Ratio** | **1.27** |
| **Sortino Ratio** | **0.01** |
| **Daily VaR (5%)** | **-0.01**|

#### vs Benchmark

- **S&P500 típico**: ~10% anual
- **Outperformance**: +134.6% sobre benchmark tradicional

### Evolución del Portafolio

<img width="1200" height="600" alt="Image" src="https://github.com/user-attachments/assets/561ae7ce-eccb-4edc-8042-6861e5ac7b9b" />

Se entrenó al agente con datos del 1 de enero del 2000 al 31 de diciembre de 2022, posteriormente se hizo la simulación del 1 de enero del 2023 al 1 de enero del 2025 

## Tecnologías Utilizadas

- **Reinforcement Learning**: Stable Baselines3 (PPO)
- **Finanzas Cuantitativas**: FinRL Environment
- **Visualización**: Matplotlib, Seaborn, Plotly
- **Datos Financieros**: yfinance API

## Acciones Analizadas

La selección de acciones se realizó considerando noticias recientes y buscando diversificación entre sectores. Para más detalles metodológicos, consultar el [Research Paper](Research_Paper.pdf).

| Ticker | Empresa                 |
|--------|-------------------------|
| BRK-B  | Berkshire Hathaway      |
| BLK    | BlackRock               |
| JPM    | JPMorgan Chase          |
| LIN    | Linde plc               |
| LLY    | Eli & Lilly             |
| AMGN   | Amgen                   |
| BMY    | Bristol Myers Squibb    |
| NVDA   | NVIDIA                  |
| AMZN   | Amazon                  |
| MSFT   | Microsoft               |

Las acciones se seleccionaron del Nasdaq100 mediante un análisis combinado: se evaluaron las correlaciones entre precios históricos y se aplicó análisis fundamental para identificar oportunidades, considerando factores como proyectos en desarrollo, niveles de deuda y solidez financiera.

### Composición del Portafolio

<img width="1200" height="600" alt="Image" src="https://github.com/user-attachments/assets/34c2cd1d-f416-42f6-b28e-0e6604168924" />

*Disclaimer: Este es un proyecto educativo. No constituye advice financiero. El trading con algoritmos conlleva riesgos significativos.*
