# **README**

# **Population Density and Housing Price Dynamics**  
### *A Comparative Analysis of the Southeastern and Midwestern United States*

<small>

**Author:** Christian McIntire  
**View Full Repository:** [github.com/christianmcintire/DACapstone](https://github.com/christianmcintire/DACapstone)

---

## **Introduction**

Housing affordability remains a pressing issue across the United States, particularly in regions experiencing rapid urbanization and population growth. The Southeastern U.S. has seen significant population increases, whereas the Midwest has remained more stable or seen decline ([Biernacka-Lievestro & Fall, 2023](https://www.pewtrusts.org/en/research-and-analysis/articles/2023/05/17/southern-states-gain-residents-the-fastest)).

This study investigates the relationship between population dynamics and housing prices in these two regions.

### **Regions Studied**

- **Southeastern U.S.**: AR, LA, KY, TN, MS, AL, GA, FL, NC, SC, VA, WV  
- **Midwestern U.S.**: MN, WI, MI, OH, IN, IL, IA, MO

---

## **Research Questions**

1. How has population density historically affected housing prices in the Southeastern and Midwestern U.S.?
2. How can these patterns be measured to predict future changes in the U.S. housing market?

---

## **Methodology**

This project combines spatial visualization, econometric modeling, and forecasting:

- **Choropleth Maps** – County-level visualizations using TIGER/Line shapefiles  
- **Hedonic Regression Models** – Decomposing housing prices into population, mortgage, and fixed effects  
- **Panel Data Estimation** – Handling state-level variation  
- **ARIMA Forecasting** – Projecting home prices through 2030

---

## **Key Findings**

### Regional Housing Trends

- **Southeast** shows higher price inflation, especially in metro counties (e.g., FL, NC, TN)  
- **Midwest** remains more stable and affordable across most counties

### ARIMA Forecasting (2024–2030)

- Southeast expected to see faster growth and greater volatility  
- Midwest projected to grow steadily and with less uncertainty  
- Confidence intervals show higher forecast risk in the Southeast

### Hedonic Regression Results

- **Monthly mortgage payment** is the most statistically significant predictor of median price (`p < 0.001`)
- **log(Population)** is *not* statistically significant (`p = 0.5`)
- **State fixed effects** reveal regional price variations even after controlling for population and mortgage:

  - Virginia & Missouri have significantly lower prices than Alabama (reference)
  - Florida, North Carolina, and Tennessee show mixed effects

### County-Level Trends

- Southeastern counties show a wider distribution in both population growth and prices  
- Midwestern counties are clustered within lower price/growth ranges  
- Choropleth and scatter plots confirm these patterns visually

---

## **Data Sources**

- **National Association of Realtors** – Q3 2024 median home prices and mortgage rates
- **Federal Reserve Bank of St. Louis (FRED)** – HPI data (1975–2024)  
- **U.S. Census Bureau** – County population estimates (2020–2023)  
- **Zillow Research** – ZHVI (Zillow Home Value Index)  
- **TIGER/Line Shapefiles** – [Download Here](https://www2.census.gov/geo/tiger/TIGER2024/)

---

## **Visual Output**

- Visualizations and Tables included  
- Regional Choropleths, ARIMA Forecasts, Scatterplots  
- Cleanly formatted using the MDPI LaTeX journal style

---

## **GitHub Repository**

View the full LaTeX report, R code, datasets, and figures:  
[https://github.com/christianmcintire/DACapstone](https://github.com/christianmcintire/DACapstone)

---

## **References**

- [Pew Research – Southern States Growth](https://www.pewtrusts.org/en/research-and-analysis/articles/2023/05/17/southern-states-gain-residents-the-fastest)  
- [National Association of Realtors](https://www.nar.realtor/)  
- [Federal Reserve Bank of St. Louis](https://fred.stlouisfed.org/)  
- [U.S. Census Bureau](https://www.census.gov/)  
- [Zillow Research](https://www.zillow.com/research/data/)  
- [TIGER/Line Shapefiles](https://www2.census.gov/geo/tiger/TIGER2024/)  
- [R Graph Gallery – Choropleth](https://r-graph-gallery.com/327-chloropleth-map-from-geojson-with-ggplot2.html)

---

*Built using R, ggplot2, and LaTeX*

</small>
