<p align="center">
  <a href="https://www.kaggle.com/code/hassanjameelahmed/saudi-telecom-stc-stock-analysis-2010-2025" target="_blank">
    <img src="2020.png" alt="ADBE" width="500">
  </a>
</p>

# 📡 STC (Saudi Telecom Company) Stock Market Analysis — Historical Price & Volume Data (2010–2025)

---

## 📋 Table of Contents

1. [Project Overview](#-project-overview)
2. [Dataset Schema — Column Details](#-dataset-schema--column-details)
3. [Kaggle Tags](#-kaggle-tags)
4. [SEO-Optimized Project Name & Description](#-seo-optimized-project-name--description)
5. [Dataset Coverage](#-dataset-coverage)
6. [Temporal & Geospatial Scope](#-temporal--geospatial-scope)
7. [Provenance](#-provenance)
8. [Data Collection Methodology](#-data-collection-methodology)
9. [Problems & Challenges](#-problems--challenges)
10. [Dataset Source](#-dataset-source)
11. [Problem Development — Step by Step](#-problem-development--step-by-step)

---

## 📌 Project Overview

This project provides a comprehensive historical dataset of **Saudi Telecom Company (STC)** stock prices and trading volumes on the **Saudi Stock Exchange (Tadawul)**, spanning **over 15 years** from March 2010 to December 2025. STC (ticker: 7010) is the largest telecommunications company in the Middle East and North Africa (MENA) region and a cornerstone of Saudi Arabia's **Vision 2030** digital transformation agenda.

The dataset enables researchers, analysts, data scientists, and investors to explore price movements, volatility patterns, trading volume dynamics, and long-term market trends for one of the most significant blue-chip stocks on the Tadawul exchange.

---

## 📊 Dataset Schema — Column Details

The dataset contains **3,891 records** (rows) and **6 columns**. Below is a detailed breakdown of each column:

| #   | Column Name | Data Type             | Description                                                                                                                                                      | Example Value |
| --- | ----------- | --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| 1   | **Date**    | `String` (MM/DD/YYYY) | The trading date for the stock record. Includes weekdays and some non-trading days (weekends/holidays typically show zero volume).                               | `3/4/2010`    |
| 2   | **Close**   | `Float64`             | The **closing price** of the STC stock for the given trading day (in Saudi Riyal, SAR). This represents the last traded price at the end of the trading session. | `42.97999954` |
| 3   | **High**    | `Float64`             | The **highest price** reached by STC stock during the trading session (in SAR). Represents the intraday peak.                                                    | `43.0`        |
| 4   | **Low**     | `Float64`             | The **lowest price** reached by STC stock during the trading session (in SAR). Represents the intraday trough.                                                   | `42.5`        |
| 5   | **Open**    | `Float64`             | The **opening price** of STC stock at the beginning of the trading session (in SAR). This is the first traded price of the day.                                  | `42.5`        |
| 6   | **Volume**  | `Integer`             | The **total number of shares traded** during the session. A volume of `0` indicates a non-trading day (weekend, public holiday, or market closure).              | `2520528`     |

### Key Observations About the Data

- **Price Format**: Early records (2010–2014) show adjusted/split-adjusted prices with many decimal places (e.g., `7.997365952`), while later records (2020–2025) show standard two-decimal pricing (e.g., `42.50`).
- **Non-Trading Days**: Rows with `Volume = 0` represent market closures (Saudi weekends: Fri–Sat, Islamic holidays like Eid al-Fitr, Eid al-Adha, National Day, etc.). Open, High, Low, and Close values remain unchanged from the prior trading day.
- **Stock Split / Adjustment**: The price shift from ~8 SAR range to ~20 SAR and then to ~40+ SAR range reflects potential stock splits, capital adjustments, or price restatements over the years.
- **Currency**: All price data is denominated in **Saudi Riyal (SAR)**.

---

## 🏷️ Kaggle Tags

The following **top 5 tags** are recommended for maximum discoverability on the Kaggle platform:

| #   | Tag                      | Rationale                                                                           |
| --- | ------------------------ | ----------------------------------------------------------------------------------- |
| 1   | **`stock-market`**       | Primary domain — financial stock market data                                        |
| 2   | **`time-series`**        | The dataset is a chronological time series ideal for forecasting and trend analysis |
| 3   | **`finance`**            | Core category covering financial analysis, investment, and portfolio management     |
| 4   | **`saudi-arabia`**       | Geographic specificity — focuses on the Saudi Arabian market                        |
| 5   | **`telecommunications`** | Industry-specific tag — STC operates in the telecom sector                          |

---

## 🔍 SEO-Optimized Project Name & Description

### Project Name

> **STC (Saudi Telecom Company) Stock Market Analysis — Historical Price & Volume Data (2010–2025)**

### SEO Description

> Explore 15+ years of historical stock market data for Saudi Telecom Company (STC, Tadawul: 7010), the largest telecom operator in the Middle East. This dataset contains 3,891 daily records of Open, High, Low, Close prices and trading Volume from March 2010 to December 2025. Ideal for time-series forecasting, technical analysis, volatility modeling, algorithmic trading backtesting, and financial EDA. Perfect for studying the impact of Saudi Arabia's Vision 2030, oil price dynamics, and MENA region market behavior on a blue-chip telecom stock.

### SEO Keywords

`STC stock data`, `Saudi Telecom Company`, `Tadawul stock exchange`, `Saudi Arabia stock market`, `STC historical prices`, `7010 stock`, `MENA telecom stocks`, `time series forecasting`, `stock price prediction`, `Vision 2030 investment`, `Saudi Arabia financial data`, `OHLCV dataset`

---

## 🌐 Dataset Coverage

### What This Dataset Covers

| Dimension                | Details                                                                           |
| ------------------------ | --------------------------------------------------------------------------------- |
| **Company**              | Saudi Telecom Company (STC) — Tadawul Ticker: **7010**                            |
| **Market**               | Saudi Stock Exchange (**Tadawul**) — the largest stock exchange in the Arab world |
| **Data Granularity**     | Daily (one record per trading day)                                                |
| **Total Records**        | 3,891 rows                                                                        |
| **Total Features**       | 6 columns (Date, Open, High, Low, Close, Volume)                                  |
| **Price Currency**       | Saudi Riyal (SAR)                                                                 |
| **Time Span**            | ~15.8 years (March 2010 – December 2025)                                          |
| **Trading Days Covered** | ~3,300+ actual trading sessions (remaining are non-trading/holiday entries)       |

### Asset Profile

STC is a **mega-cap** company and one of the **top 5 most valuable** companies on the Tadawul exchange. It holds:

- The largest **market capitalization** among MENA telecom companies
- Operations across **12+ countries** including Saudi Arabia, Kuwait, Bahrain, Turkey, and Malaysia
- A critical role in Saudi Arabia's **Vision 2030** digital infrastructure development
- Significant government ownership through the **Public Investment Fund (PIF)**

---

## 📅 Temporal & Geospatial Scope

### Temporal Scope

| Parameter            | Value                                                            |
| -------------------- | ---------------------------------------------------------------- |
| **Start Date**       | **03/04/2010**                                                   |
| **End Date**         | **12/31/2025**                                                   |
| **Duration**         | ~15 years and 10 months                                          |
| **Frequency**        | Daily (includes non-trading days with zero volume)               |
| **Trading Calendar** | Saudi Stock Exchange (Tadawul) — Sunday to Thursday trading week |

### Geospatial Scope

| Parameter            | Value                                                            |
| -------------------- | ---------------------------------------------------------------- |
| **Country**          | 🇸🇦 **Saudi Arabia** (Kingdom of Saudi Arabia)                    |
| **City**             | **Riyadh** (STC headquarters & Tadawul exchange location)        |
| **Region**           | Middle East and North Africa (MENA)                              |
| **Exchange**         | Saudi Stock Exchange (Tadawul) — located in Riyadh, Saudi Arabia |
| **Market Regulator** | Capital Market Authority (CMA) of Saudi Arabia                   |

### Key Historical Periods in the Dataset

| Period    | Event                                      | Impact on STC Stock                               |
| --------- | ------------------------------------------ | ------------------------------------------------- |
| 2010–2012 | Post-global financial crisis recovery      | Gradual price stabilization                       |
| 2014–2016 | Oil price crash                            | Significant downward pressure on Saudi equities   |
| 2016–2018 | Vision 2030 announcement & reforms         | Market liberalization boosted investor confidence |
| 2019      | Tadawul joins MSCI Emerging Markets Index  | Increased foreign institutional investment        |
| 2020      | COVID-19 pandemic                          | Market volatility with accelerated digital demand |
| 2020–2021 | STC rebranding & expansion                 | Strategic transformation and price appreciation   |
| 2022–2025 | 5G rollout & digital infrastructure growth | Sustained growth in valuation                     |

---

## 📜 Provenance

### Data Source Origin

The data is sourced from **publicly available financial market records** of the **Saudi Stock Exchange (Tadawul)**. Stock price and volume data for STC (Ticker: 7010) is transmitted and aggregated by authorized financial data providers.

### Primary Data Providers

| Provider                           | Role                                                                           |
| ---------------------------------- | ------------------------------------------------------------------------------ |
| **Tadawul (Saudi Stock Exchange)** | Primary source — official exchange where STC shares are listed and traded      |
| **Yahoo Finance**                  | Secondary aggregator — provides historical OHLCV data for international access |
| **Investing.com / Google Finance** | Alternative sources — cross-reference and validation                           |

### Data Transformations

1. **Price Adjustment**: Historical prices appear to be **split-adjusted** and **dividend-adjusted** to ensure consistency across the full time range. This explains the decimal-heavy prices in early years (e.g., `7.997365952` in 2010).
2. **Non-Trading Day Inclusion**: Days with zero volume (weekends, holidays) are included in the dataset with prices carried forward from the last trading day.
3. **Format Standardization**: Dates are formatted in `MM/DD/YYYY` format. All prices are in Saudi Riyal (SAR).
4. **No Imputation**: Missing values do not appear to be imputed — non-trading days are explicitly marked by `Volume = 0`.

### Data Integrity Notes

- A few anomalous values exist (e.g., `Close = 20.99` on 01/06/2011 and `Close = 20.52` on 06/27/2013), which may indicate data entry errors or extraordinary corporate actions (such as rights issues, splits, or ex-dividend adjustments).
- Users should validate these outliers before using the dataset for quantitative modeling.

---

## 🔬 Data Collection Methodology

### How the Data Was Collected

| Step                            | Description                                                                                                                                                                |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Source Identification**    | STC stock (Tadawul: 7010) was identified as the target instrument for data collection.                                                                                     |
| **2. API/Platform Query**       | Historical price data was retrieved from a financial data provider (e.g., Yahoo Finance API, Tadawul official records, or a financial terminal such as Bloomberg/Reuters). |
| **3. OHLCV Extraction**         | Daily Open, High, Low, Close, and Volume values were extracted for each trading session within the specified date range.                                                   |
| **4. Date Range Selection**     | The data collection window was set from **March 4, 2010** to **December 31, 2025**, capturing over 15 years of market history.                                             |
| **5. Price Adjustment**         | Prices were adjusted for stock splits and dividends to provide a consistent price series for time-series analysis.                                                         |
| **6. Non-Trading Day Handling** | Non-trading days (Saudi weekends: Friday–Saturday; Islamic holidays) were retained in the dataset with Volume set to 0 and prices carried forward.                         |
| **7. Export & Formatting**      | Data was exported to CSV format with columns: Date, Close, High, Low, Open, Volume.                                                                                        |

### Collection Tools & Technologies

- **Financial APIs**: Yahoo Finance (`yfinance` Python library), Alpha Vantage, or direct Tadawul data feeds
- **Data Processing**: Python (`pandas`, `numpy`) for data cleaning and formatting
- **Storage Format**: Comma-Separated Values (CSV) file — `STC.csv`

---

## ⚠️ Problems & Challenges

### 1. Data Quality Issues

| Challenge                   | Description                                                                                                                                                                                                                                           |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Anomalous Price Spikes**  | At least two records show unrealistic price jumps (e.g., Close ≈ 20.99 on 01/06/2011 and Close ≈ 20.52 on 06/27/2013) that deviate dramatically from surrounding data. These likely represent data errors or unresolved corporate action adjustments. |
| **Adjusted vs. Raw Prices** | The mix of heavily adjusted prices (early years) and raw prices (later years) may confuse models if not properly handled.                                                                                                                             |
| **Non-Trading Day Noise**   | Including zero-volume days inflates the dataset size without adding information, potentially skewing volume-based indicators (e.g., VWAP, OBV).                                                                                                       |

### 2. Market-Specific Challenges

| Challenge                     | Description                                                                                                                                                                                              |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Islamic Calendar Holidays** | Saudi Arabia observes a calendar with variable holidays (Eid al-Fitr, Eid al-Adha, Hajj season), making standardized time-series analysis and cross-market comparison more complex than Western markets. |
| **Trading Week Differences**  | Tadawul operates Sunday–Thursday, which misaligns with global markets (Monday–Friday). This complicates multi-market correlation studies.                                                                |
| **Government Influence**      | STC's largest shareholder is the Public Investment Fund (PIF), a sovereign wealth fund. Government policy decisions can disproportionately affect STC stock compared to fully private companies.         |
| **Oil Price Dependency**      | Despite being a telecom company, STC's stock is heavily influenced by oil prices due to Saudi Arabia's petro-economy. This external dependency creates confounding factors for pure telecom analysis.    |

### 3. Analytical Challenges

| Challenge                  | Description                                                                                                                                                |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Limited Feature Set**    | Only OHLCV data is provided — no fundamental data (revenue, earnings, P/E ratio), no sentiment data, and no macroeconomic indicators are included.         |
| **Currency Fluctuations**  | While SAR is pegged to the USD (1 USD ≈ 3.75 SAR), international investors must account for currency risk and exchange rate considerations.                |
| **Regime Changes in Data** | The data spans multiple market regimes (e.g., pre-Vision 2030 vs. post-Vision 2030, pre-COVID vs. post-COVID), requiring regime-aware modeling approaches. |
| **Low Liquidity Periods**  | Some periods show zero or very low volume, which can create misleading technical indicator readings.                                                       |

### 4. Modeling Challenges

| Challenge               | Description                                                                                                                                                    |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Non-Stationarity**    | Stock price data is inherently non-stationary, requiring differencing, log-returns, or other transformations before applying statistical models (e.g., ARIMA). |
| **Outlier Sensitivity** | Machine learning models (especially neural networks) can be sensitive to the anomalous price spikes identified in the data.                                    |
| **Overfitting Risk**    | With 15+ years of data, it's tempting to build complex models that overfit to historical patterns that may not repeat.                                         |

---

## 🔗 Dataset Source

### Primary Source

| Attribute                 | Details                                                                                                                                                                                                                               |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Company**               | Saudi Telecom Company (STC)                                                                                                                                                                                                           |
| **Tadawul Ticker**        | **7010**                                                                                                                                                                                                                              |
| **Exchange**              | Saudi Stock Exchange (Tadawul)                                                                                                                                                                                                        |
| **Official Tadawul Page** | [https://www.saudiexchange.sa/wps/portal/saudiexchange/trading/equities-directory/company-details/!ut/p/z1/04_Sj9CPykssy0xPLMnMz0vMAfIjo8zi_Tx8nD0MLIy83V1DnA0czT0Cg1yDA4wMPE31I4EKzBEKDIIcTRQtSYi3g/](https://www.saudiexchange.sa/) |
| **Yahoo Finance**         | [https://finance.yahoo.com/quote/7010.SR/](https://finance.yahoo.com/quote/7010.SR/)                                                                                                                                                  |
| **Investing.com**         | [https://www.investing.com/equities/saudi-telecom](https://www.investing.com/equities/saudi-telecom)                                                                                                                                  |
| **Google Finance**        | [https://www.google.com/finance/quote/7010:TADAWUL](https://www.google.com/finance/quote/7010:TADAWUL)                                                                                                                                |

### About STC (Saudi Telecom Company)

Saudi Telecom Company (STC), rebranded as **stc** in 2021, is a Saudi Arabian telecommunications company headquartered in **Riyadh**. It is the largest mobile operator in the Middle East and has subsidiaries in Kuwait (VIVA), Bahrain (VIVA), Turkey (Turk Telekom), and other markets. STC was established in **1998** and went public on the **Tadawul exchange in 2003** under ticker **7010**.

---

## 📈 Problem Development — Step by Step

The following outlines how the core analytical problem evolved within the context of this dataset and STC's market journey:

### Step 1: Early Market Dynamics (2010–2012)

> **Problem Seed**: After the 2008 global financial crisis, Saudi equity markets were recovering. STC stock traded in the **7–8 SAR (adjusted)** range with moderate volatility. The challenge was understanding how a state-backed telecom monopoly would behave in a recovering but oil-dependent market.

### Step 2: Market Liberalization & Competitive Pressure (2012–2014)

> **Problem Growth**: The Saudi telecom market was deregulated, introducing competitors like Mobily (Etihad Etisalat) and Zain KSA. STC faced **revenue pressure** from increased competition, and the dataset shows periods of price stagnation and increased volume, reflecting market uncertainty about STC's competitive positioning.

### Step 3: Oil Price Collapse Impact (2014–2016)

> **Problem Deepening**: Oil prices crashed from $115/barrel to below $30/barrel. Although STC is a telecom company, Saudi Arabia's oil-dependent economy dragged down the entire Tadawul index. STC's stock experienced **significant declines**, and trading volumes spiked as investors re-evaluated the value of Saudi equities.

### Step 4: Vision 2030 Transformation (2016–2018)

> **Direction Shift**: Crown Prince Mohammed bin Salman announced **Saudi Vision 2030**, a sweeping economic reform plan that included diversifying away from oil, developing digital infrastructure, and opening the Saudi market to foreign investors. STC was positioned as a **key beneficiary** of the digital transformation pillar. This created new analytical questions: How would STC's stock respond to these reforms?

### Step 5: Foreign Investment Influx (2019)

> **Problem Expansion**: The Tadawul was included in the **MSCI Emerging Markets Index** in 2019, bringing a wave of foreign institutional capital. STC, as a major index constituent, experienced **increased trading volumes** and enhanced price discovery. The challenge shifted to understanding the impact of **foreign capital flows** on STC's price dynamics.

### Step 6: COVID-19 Disruption & Digital Acceleration (2020)

> **Crisis & Opportunity**: The COVID-19 pandemic caused market-wide selloffs in early 2020. However, lockdowns and remote work dramatically increased demand for telecom services. STC benefited from **accelerated digital adoption**, and its stock recovered faster than many Tadawul peers. The problem became: Can STC sustain the pandemic-driven demand surge?

### Step 7: STC Rebranding & 5G Expansion (2020–2023)

> **Strategic Evolution**: STC rebranded to **stc** and launched one of the **first 5G networks** in the Middle East. The company expanded into cloud computing, cybersecurity, and digital payments (stc pay). Stock prices reflected these strategic moves with **steady appreciation**, and the dataset captures this transformation in the upward price trend.

### Step 8: Matured Market & Sustained Growth (2023–2025)

> **Current State**: By 2023–2025, STC stock stabilized in the **40–43 SAR** range with relatively lower volatility compared to earlier periods. The challenge now centers on: Has STC reached a **mature valuation plateau**? What factors could drive the next phase of growth or decline? How do macroeconomic factors (interest rates, oil prices, global telecom trends) influence STC's future trajectory?

### Summary of Problem Evolution

```
2010 ─────→ Post-crisis recovery & price stabilization
   │
2012 ─────→ Market competition introduces revenue risk
   │
2014 ─────→ Oil crash drags all Saudi equities down
   │
2016 ─────→ Vision 2030 positions STC as digital beneficiary
   │
2019 ─────→ MSCI inclusion brings foreign capital & liquidity
   │
2020 ─────→ COVID-19 crash followed by digital demand surge
   │
2021 ─────→ Rebranding to stc + 5G + digital diversification
   │
2025 ─────→ Matured valuation — next growth catalyst unclear
```

---

> **📝 Note**: This documentation was created for Kaggle platform publication and academic/professional use. Always verify data accuracy before making financial decisions. Past performance does not guarantee future results.

---

_Last Updated: February 16, 2025_
_Dataset: STC.csv | Records: 3,891 | Columns: 6 | Format: CSV_
