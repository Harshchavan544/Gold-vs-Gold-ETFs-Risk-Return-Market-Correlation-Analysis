# Gold vs Gold ETFs: A Risk, Return & Market Correlation Analysis

An exploratory financial data analysis project comparing **Gold, five Gold ETFs, and the Sensex** to understand their performance, volatility, risk-adjusted returns, and relationships with each other.

The project uses Python and financial market data to investigate whether different Gold ETFs behave differently, how closely they track Gold, and whether Gold provides diversification benefits relative to the equity market.

---

## 📌 Project Overview

Gold is often considered a defensive asset and a potential diversification tool during periods of equity-market uncertainty. However, investors accessing gold through ETFs may wonder:

* Do different Gold ETFs perform differently?
* Which Gold ETF is more stable?
* How closely do Gold ETFs track Gold prices?
* Does Gold provide diversification against equity-market movements?
* How does risk and return change across different periods?
* Which asset provides better risk-adjusted performance?

This project attempts to answer these questions using historical price data and statistical analysis.

---

## 🎯 Objectives

The main objectives of this project are to:

1. Compare the performance of five Gold ETFs.
2. Analyze the volatility of each ETF.
3. Measure the correlation between Gold ETFs.
4. Compare Gold prices with Gold ETFs.
5. Analyze the relationship between Gold and the Sensex.
6. Compare risk-adjusted performance using the Sharpe Ratio.
7. Analyze monthly and yearly performance patterns.
8. Examine how the relationship between Gold and equities changes over time.
9. Identify whether historical price performance alone is sufficient to select a Gold ETF.

---

## 📊 Assets Analyzed

The analysis covers:

* Gold
* SBI Gold ETF
* HDFC Gold ETF
* Nippon Gold ETF
* ICICI Gold ETF
* Kotak Gold ETF
* Sensex

The dataset covers the available period from **2024 to March 2026**, with 2025 representing the complete calendar year and 2024/2026 representing partial periods.

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical calculations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Jupyter Notebook**
* **Statistical analysis**
* **Financial performance metrics**

---

## 🔍 Analysis Performed

### 1. Data Cleaning & Preparation

* Imported historical market data
* Checked and handled missing values
* Converted date columns
* Aligned datasets across assets
* Prepared data for return and correlation analysis

### 2. Return Analysis

Daily and monthly returns were calculated to understand the performance of Gold, Gold ETFs, and the Sensex.

### 3. Correlation Analysis

Correlation matrices were used to measure the relationship between:

* Gold ETFs
* Gold and Gold ETFs
* Gold and Sensex

### 4. Volatility Analysis

Standard deviation of returns was used as a measure of historical volatility.

### 5. Year-wise Analysis

Performance and volatility were compared across different years to identify changes in market conditions.

### 6. Monthly Analysis

Monthly returns were analyzed to identify strong and weak periods and to examine how ETFs reacted during significant movements in Gold.

### 7. Sharpe Ratio

The Sharpe Ratio was used to compare risk-adjusted performance.

A **6% risk-free rate** was used in the analysis.

### 8. Gold vs Sensex Analysis

Gold and Sensex returns were compared to understand whether Gold and equities moved together or independently during different periods.

---

# 📈 Key Findings

## 1. Gold ETFs are highly similar

The five Gold ETFs showed extremely high correlations with each other, with pairwise correlations of approximately **0.977–0.990**.

This indicates that the ETFs exhibited very similar price movements during the analyzed period.

---

## 2. SBI was marginally more stable

Among the five ETFs:

| ETF    | Daily Volatility |
| ------ | ---------------: |
| SBI    |        **1.67%** |
| Kotak  |            1.69% |
| Nippon |            1.72% |
| ICICI  |            1.72% |
| HDFC   |        **1.73%** |

SBI recorded the lowest historical volatility, while HDFC recorded the highest.

However, the difference was relatively small, suggesting that the ETFs had broadly similar risk characteristics.

---

## 3. Gold showed the strongest calculated risk-adjusted performance

Gold recorded:

* **54.5% calculated annualized average daily return**
* **24.7% annualized volatility**
* **1.962 Sharpe Ratio**

The ETFs had Sharpe Ratios ranging from approximately **1.56 to 1.60**.

Based on these calculations, Gold delivered the strongest risk-adjusted performance in the analyzed dataset.

> Note: The annualized return in this project is based on annualizing the average daily return rather than calculating CAGR.

---

## 4. Gold and Gold ETFs do not perfectly track each other daily

Daily Gold–ETF correlations ranged from approximately **0.58 to 0.62**.

However, monthly correlations were considerably stronger, ranging from approximately **0.75 to 0.83**.

This suggests that Gold ETF movements tend to align more closely with Gold over longer periods, while short-term differences may be influenced by factors such as:

* Different trading hours
* Market holidays
* Currency effects
* Market timing

---

## 5. Gold and Sensex showed low overall correlation

The overall Gold–Sensex correlation was approximately:

**0.16**

This indicates relatively low co-movement between Gold and the equity market during the analyzed period.

This suggests that Gold may provide potential diversification benefits when combined with equity exposure.

---

## 6. The Gold–Sensex relationship changed over time

During early 2026:

| Month    |        Gold |      Sensex |
| -------- | ----------: | ----------: |
| January  | **+10.50%** |  **−2.84%** |
| February |  **+9.85%** |  **−1.19%** |
| March    | **−10.01%** | **−11.49%** |

Gold rose while the Sensex declined during January and February.

However, both Gold and the Sensex declined sharply in March.

This demonstrates that Gold can behave differently from equities, but it is **not a guaranteed hedge against equity-market declines**.

---

## 7. Risk increased significantly in 2026

Volatility increased sharply during the available 2026 period.

For example:

| Year  |      HDFC |       SBI |      Gold |
| ----- | --------: | --------: | --------: |
| 2024  |     0.91% |     0.91% |     1.11% |
| 2025  |     1.24% |     1.24% |     1.41% |
| 2026* | **3.57%** | **3.37%** | **2.56%** |

*January–March 2026

This indicates a substantial change in market risk conditions during early 2026.

---

## 8. ETF selection requires more than historical returns

Since the five ETFs showed extremely similar price movements, historical price performance alone does not provide a strong reason to prefer one ETF over another.

For a complete ETF-selection decision, additional factors should be considered, such as:

* Expense ratio
* Tracking error
* Liquidity
* Bid-ask spread
* Assets Under Management (AUM)

---

# 📌 Important Limitations

This analysis has several limitations:

* The dataset represents a limited historical period.
* 2024 and 2026 are partial periods.
* Correlation does not imply causation.
* Historical performance does not guarantee future performance.
* ETF price performance alone does not capture expense ratios, tracking error or liquidity.
* Gold and Indian-market instruments may have different trading hours and currency effects.
* The Sharpe Ratio uses a 6% assumed risk-free rate.
* The annualized return calculation is based on average daily returns rather than CAGR.

---

# 🧠 Conclusion

The analysis shows that the five Gold ETFs behaved very similarly, with correlations above **0.97**, while differences in their volatility and risk-adjusted performance were relatively small.

Gold itself showed the strongest calculated risk-adjusted performance during the analyzed period, with a **1.962 Sharpe Ratio**.

The low overall Gold–Sensex correlation of approximately **0.16** suggests potential diversification benefits. However, the behavior observed in early 2026 also demonstrates that Gold is **not a guaranteed hedge against equity-market declines**.

Overall, the analysis highlights that selecting a Gold ETF should not rely solely on historical returns. Since the ETFs showed very similar market behavior, factors such as **tracking error, expense ratio, liquidity and trading costs** should also be considered.

---

## 👨‍💻 Author

**Harsh Chavan**

Data Analyst | Python | SQL | Excel | Data Visualization

---
