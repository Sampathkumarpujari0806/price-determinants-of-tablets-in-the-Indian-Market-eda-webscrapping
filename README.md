# Price Determinants of Tablets in the Indian Market : A Web Scraping and EDA Project
## 📌 Project Overview
This project uses web-scraped product data to analyze which hardware specifications, brand positioning, and promotional offers drive tablet pricing in India. I scraped product listings from Flipkart, cleaned and standardized the data, and conducted exploratory data analysis (EDA) to identify pricing patterns, brand segments, and value-for-money recommendations for consumers.

---
## 🎯 Objectives
- Help consumers choose the right tablet based on budget, performance features, brand reputation, and specifications such as RAM, ROM, and display size.
- Identify trends in brand-wise pricing, feature distribution, and the overall positioning of tablets in the Indian market.
- Examine how specifications (RAM, ROM, battery capacity, display size, cameras, connectivity) influence minimum, maximum, and average prices.
- Correlate specifications, brand category, and customer ratings to determine which tablets offer the best balance between price and performance.
- Detect patterns such as premium pricing clusters, budget segments, and spec combinations commonly used by brands to differentiate their products.
--- 
## 🧭 Web Scraping Workflow
- Source: Flipkart (publicly available product listings) <br>

1.Scraped tablet listings from multiple Flipkart pages<br>
2.Extracted attributes:<br>
    - Brand, Model<br>
    - RAM, ROM<br>
    - Display Size<br>
    - Battery<br>
    - Rear/Front Camera<br>
    - Connectivity<br>
    - Ratings, Reviews<br>
    - Original Price, Final Price, Discount <br>
3.Stored results in a Pandas DataFrame <br>
4.Exported cleaned and raw data to CSV for further analysis

---
## 🛠️ Tech Stack

- Language: Python
-  Libraries:
   - requests, BeautifulSoup, re – for web scraping
   - pandas, numpy – for data cleaning & manipulation
   - matplotlib, seaborn – for visualization
- Environment: Jupyter Notebook


---
## 🗂️ Dataset Description
- 960 tablet records
- 17 columns, including:
   - Brand, Model
   - RAM (GB), ROM (GB)
   - Display Size (inch)
   - Connectivity (Wi-Fi / Wi-Fi + SIM)
   - Rear & Front Camera (MP)
   - Battery (mAh)
   - Ratings & Reviews
   - Original Price, Final Price, Discount%
   - Exchange Discount Price
---

## 🧹 Data Cleaning Steps
- Removed special characters from price and discount columns.
- Dropped duplicated rows.
- Identified all null values and imputed them using appropriate strategies.
- Converted all numeric and categorical fields columns into correct data types.
- Detected outliers using the IQR method.
- Retained them after confirming they represent genuine premium tablets.
- Standardized categorical columns by converting all category text to lowercase for consistency.

---
## 📊 Univariate Analysis — Key Insights
- Apple dominates the dataset, followed by Samsung; Lenovo sits mid-range; all other brands appear in small numbers.
- Prices are heavily right-skewed; most tablets fall between ₹10,000–₹30,000.
- Most tablets feature 4GB RAM and 128GB ROM, showing a shift toward mid-range hardware.
- Calling-enabled tablets (Wi-Fi + SIM) account for 56%, showing strong preference over Wi-Fi-only tablets.

---
## 🔗 Bivariate Analysis — Key Patterns
- Battery vs Price: Higher prices correlate with larger batteries, especially above 9000 mAh.
- Display Size vs Price: Prices generally rise with larger displays.
- Brand vs Price: Apple > Samsung > OnePlus dominate premium listings.
- Connectivity vs Price: Wi-Fi + SIM tablets are consistently more expensive.
- RAM vs Price: Price increases with RAM, especially 8GB+.
- ROM vs Price: Higher storage (128GB+, especially 256GB) aligns with higher pricing.
- Correlation Heatmap: Display size and camera quality show stronger correlations compared to RAM and battery.

---

## ❓ Business Questions & Insights
| Question                             | Key Insight                                   |  
| ------------------------------------ | --------------------------------------------- | 
| Which brands dominate?               | Apple and Samsung lead significantly.         |  
| What is the most common price range? | ₹10,000–₹40,000.                              |  
| Does connectivity affect price?      | Yes, calling tablets (Wi-Fi + SIM) cost more. |  
| Does display size impact price?      | Larger displays → higher prices.              |  
| Do cameras influence price?          | Moderate positive correlation.                |   

--- 

## 🧠 Conclusion
- Apple and Samsung dominate the premium tablet segment, while most other brands target the budget range.
- Tablet prices rise mainly with larger displays, higher storage (ROM), and better camera specifications.
- RAM and battery capacity impact price but are weaker predictors compared to display and storage.
- Wi-Fi + SIM models are generally priced higher than Wi-Fi-only versions.
- Price variation is driven by brand positioning and feature combinations rather than any single specification.
- Discounts and exchange offers vary widely, reflecting competitive pricing strategies across brands.

---
## ▶️ How to Run This Project
