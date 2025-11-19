# Price Determinants of Tablets in the Indian Market: A Web Scraping and EDA Project
This project uses web-scraped product data to analyze which hardware specifications, brand positioning, and promotional offers drive tablet pricing in India. I scraped product listings from Flipkart, cleaned and standardized the data, and conducted exploratory data analysis (EDA) to identify pricing patterns, brand segments, and value-for-money recommendations for consumers.


## Dataset & Scope
- Source: Flipkart product listings (40 pages scraped).
- Records: 960 tablet listings, 17 standardized features (brand, model, RAM, ROM, display size, battery, cameras, connectivity, ratings, pricing, warranty, etc.).
- Tools: Python (Requests, BeautifulSoup, Pandas), regex for parsing, visualization with Matplotlib/Seaborn, and summary reporting.

## What I did
- Built a clean, analysis-ready dataset from raw HTML listings.
- Performed thorough preprocessing: removed duplicates, type conversions, imputations for missing values, outlier detection (IQR), and categorical standardization.
- Conducted univariate and bivariate EDA to surface distributional patterns and relationships between specs and price.
- Produced actionable insights and consumer-focused recommendations based on feature-price correlations and brand/segment analysis.

## Key findings
- Apple and Samsung dominate product availability and premium pricing.
- Most tablets sit in the ₹10,000–₹40,000 range; premium devices are a small share.
- Display size, ROM (storage), and camera specs are the strongest price drivers; RAM and battery show weaker correlations.
- Wi-Fi + SIM models generally command higher prices than Wi-Fi-only variants.
- Exchange offers and warranty patterns reveal pockets of better value among mid-range brands.

## How to load file
- See the original presentation for methodology and visuals:EDA_Project_Tablets.pptx
- Run the scraper (Python script) to fetch listings from Flipkart pages (use requests + BeautifulSoup).
- Load the CSV into Pandas, run the cleaning pipeline (dedupe, impute, type cast), then execute EDA notebooks to reproduce charts and correlation analyses.
