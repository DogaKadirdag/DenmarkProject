#Denmark CO2 Emissions & GDP per Capita

This project investigates the relationship between **carbon dioxide (CO₂) emissions** and **GDP per capita** in Denmark using R. This project includes correlation analysis, simple linear regression, significance test, and residual.

#Project Structure

```
denmark-emissions-analysis/
├── data/
│   └── Denmark Project.xlsx
├── scripts/
│   └── analysis.R
├── output/
│   ├── scatter_plot.png
│   ├── regression_line.png
│   └── residual_plot.png
├── README.md
└── .gitignore
```

#Analysis Overview 

- **Scatter Plot:** Plotted CO₂ emissions against GDP per capita (income).
- **Correlation:** Finding correlation coefficient: `r = 0.1865502`
- **Regression:**
  - Writing the regression model with the values; `emission = 9.5146 + 0.2237 * income`
  - Slope not statistically significant: `p = 0.1768`
- **Fitted Values:** Stored and examined for most recent observation.
- **Regression Line:** Added to scatter plot for visual fit.
- **Significance Testing:**
  Test if slope is significant at 5% level.
  Hypotheses:
  Ho = β1 = 0
  H1 = B1 ≠ 0
​  If the p-value is > than 0.05 and the CI (confidence interval) includes 0 , we fail to reject H0.
- **Residuals:** Analyzed for randomness and variance

- #Findings end of the project

- Weak positive correlation between GDP per capita (income) and CO₂ emissions.
- Obtained linear relationship solution is; **not statistically significant**.
- Residuals show no clear pattern, but slightly heteroskedasticity may exist. Graphically, when income is increasing, residuals become more spread out.
- Model’s explanatory power is limited, suggest to adding other variables on the model (e.g., industry share, energy mix) may be more informative.

#Libraries and Studio system

- **R**: for data analysis, modeling, visualization
- **ggplot2**: for create plotting
- **readxl**: for reading Excel files

