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

