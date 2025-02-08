# World-Bank-Indicators

### Project Overview
The goal of this project is to create an interactive performance dashboard to visualize and analyze key country-level metrics such as GDP, population, life expectancy, CO2 emissions, unemployment, and access to electricity.

![Picture1](https://github.com/user-attachments/assets/b38ac5c6-fa1d-4688-8ef8-60cfcf6c5e11)

### Data Sources

This dataset is the "World Bank Dataset.csv" file from kaggle containing a set of key economic, social, and environmental indicators for 20 countries over the period from 2010 to 2019. The dataset is designed to reflect typical World Bank metrics, which are used for analysis, policy-making, and forecasting.

### Tools

- Microsoft Excel - Data Preparation and Cleaning [Download here](https://microsoft.com)
- Python - Data Analysis
- Plotly.js - Data Visualization [Download here](https://plotly.com)
- HTML - Dashboard Development

### Data Cleaning/Preparation

In the Initial data preparation phase, we performed the following tasks:

1. Data Loading and Inspaction
2. Handling missing values
3. Data cleansing and formatting


### Exploratory data analysis
EDA involved exploring various indicators to answer key questions such as:

- How is life expectancy distributed across different countries, and are there any outliers or patterns based on population size?
- Which countries have the highest or lowest unemployment rates, and how do they compare across the dataset?
- How does access to electricity correlate with CO2 emissions, and how do countries differ based on population size?
- How has the GDP of different countries changed over time, and which countries have experienced significant growth or declines?



![newplot (6)](https://github.com/user-attachments/assets/4583c3ac-d81c-4c82-b2fc-f86c02068199)

![newplot (4)](https://github.com/user-attachments/assets/b9d7c102-4307-4139-a23f-f42a442ab614)

![Picture3](https://github.com/user-attachments/assets/c8a2e072-740b-4035-b42d-2fe2be8e766f)


### Data Analysis

```python
import pandas as pd
import plotly.express as px

# Load the JSON data
data = pd.read_json('data.json')

# Create the violin plot
fig = px.violin(data, x='Country', y='Life Expectancy', box=True, points='all', title='Population vs. Life Expectancy')
fig.show()
```

### Results/Findings

1. Developed countries tend to have higher life expectancy, lower unemployment, and higher CO2 emissions, but also more access to modern infrastructure like electricity.
2. Developing countries face challenges in economic growth, employment, and sustainable energy access, but they present opportunities for targeted development programs.
3. Sustainable development strategies should balance economic growth, environmental impact, and social well-being for long-term success.


### Recommedations

Based on the analysis, we recommend the followimg action:

- Countries with low electricity access and low emissions, like Nigeria and India, should invest in renewable energy projects (solar, wind) to expand access without significantly increasing CO2 emissions.
- Countries with high unemployment and fluctuating GDP, like Mexico, South Africa, and Nigeria, should implement job creation programs and diversify their economies to reduce dependency on volatile industries, such as natural resources.
- Countries with low and varying life expectancy, such as Nigeria and South Africa, should improve access to healthcare, nutrition, and education, particularly in rural and underdeveloped areas.

#### Limitation of Analysis

The analysis presented in this report is based on the available dataset, which may contain limitations affecting the accuracy of the results. Potential issues include incomplete records, inconsistencies in data collection methods, and limited coverage of certain regions or years.


😄
💻
