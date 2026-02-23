# Global Education Investment vs. Economic Output (2012–2022)

## 📊 Project Overview
Does higher education spending actually drive wealth? This study analyzes a decade of longitudinal World Bank data to quantify the relationship between fiscal "input" (Education Spend) and economic "output" (GDP/PPP).

### 💡 The "Efficiency Gap" Finding
**H3 Supported:** Education is a necessary catalyst but not a standalone driver. Data reveals an "Efficiency Gap" where only **21% of nations** successfully translate high investment into high PPP. 

---

## 🛠️ Technical Execution Highlights
* **Time-Series Analysis (`SQL`):** Leveraged **Window Functions** (`LAG`) to calculate Year-over-Year (YoY) growth and absolute deltas for GDP and PPP across 190+ territories.
* **Data Integrity:** Implemented `NULLIF` and `COALESCE` logic to handle inconsistent reporting gaps, ensuring that missing World Bank data points did not skew the global medians.
* **Modular Logic:** Used **CTEs (Common Table Expressions)** to create a clean, readable pipeline for calculating the 10-year global benchmark.
* **Efficiency Benchmarking (`DAX`):** Engineered an `is_above_avg` binary flag in Power BI to isolate the "Efficiency Quadrant".

---

## 📂 Project Navigation
* [**Executive Summary (PDF)**](./docs/Executive_Memo.pdf) - High-level results and visual dashboard highlights.
* [**SQL Analysis Scripts**](./scripts/data_analysis.sql) - The "Technical Engine" featuring window functions and CTEs.
* [**Technical Deep-Dive**](./docs/Technical_Documentation.pdf) - Full 20-page methodology including Excel unpivoting steps.
* [**Cleaned Dataset**](./data/cleaned_data.csv) - Processed data ready for replication.

---

## 🚀 Key Insights
1.  **Growth Decoupling:** Global Median PPP grew by 63% over the last decade, while education investment remained stagnant at ~4% of GDP.
2.  **Lagging Indicators:** Education ROI operates on a 15–25 year cycle; current fiscal efforts act as an economic "floor" to prevent collapse rather than an immediate "elevator" to wealth.
