# Competitor-Sales-Analysis

# Performed the following challenges:
- Data integration
- Transformation
- Modeling
- Exploratory data analysis
- DAX calculation
- Visualization
- Performance testing

# Performed DAX calculations:
- Growth over time;
  - % Growth = DIVIDE(SUM(Sales[Revenue])-([PY Sales]), ([PY Sales]))
- Sales compared to previous year;
  - PY Sales = CALCULATE(
    SUM(Sales[Revenue]),
    SAMEPERIODLASTYEAR('Date'[Date]))
- Combine Zip & Country;
  - ZipCountry = Sales[Zip] & "," & Sales[Country]
- Manufacturer revenue based on 'manufacturer ID';
  - Manufacturer Revenue = CALCULATE(
    SUM(Sales[Revenue]), Manufacturer[ManufacturerID] = 4)
- Manufacturer market share;
  - Manufacturer Market Share = DIVIDE(
    Sales[Sintec Revenue], SUM(Sales[Revenue]),0)

# Dashboards created:
- Competitor Analysis
![3y0oujbz oin](https://github.com/MarcvWaes/Datacamp-Competitor-Sales-Analysis/assets/120553175/3e1a3157-4a10-4b26-b5b4-c1234f01fac7)
- Advanced Insights
![xhew0yvy 4eo](https://github.com/MarcvWaes/Datacamp-Competitor-Sales-Analysis/assets/120553175/00e834a6-9aeb-425e-b23c-547154b742f2)
