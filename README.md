# COVID-19 Analysis

# About COVID-19
COVID-19, caused by the SARS-CoV-2 virus, emerged in late 2019 and rapidly spread worldwide, leading to a global pandemic. It primarily affects the respiratory system, with symptoms ranging from mild, such as fever and cough, to severe, including difficulty breathing and pneumonia. The virus spreads through respiratory droplets, making it highly contagious. Governments worldwide implemented various measures such as lockdowns, social distancing, and widespread vaccination campaigns to control its spread. The pandemic has had profound effects on health systems, economies, and daily life, highlighting the need for global cooperation in public health crises.

## Purpose of the COVID-19 Analysis Project

The purpose of this COVID-19 analysis project is to provide comprehensive insights into the spread, impact, and management of the COVID-19 pandemic. The analysis is based on a day-wise dataset that includes key metrics such as:

- **Confirmed Cases**
- **Deaths**
- **Recoveries**
- **Active Cases**
- **New Cases**
- **New Deaths**
- **New Recoveries**

### Key Objectives:

1. **Track and Visualize Trends:**
   - Analyze the progression of the virus over time to understand how it spreads across different regions.

2. **Identify Patterns:**
   - Examine the data to understand the effectiveness of various public health interventions, such as lockdowns and social distancing.

3. **Assess the Impact:**
   - Evaluate the impact of COVID-19 on different regions and populations, identifying areas that have been more severely affected.

4. **Provide Actionable Insights:**
   - Deliver data-driven insights to inform the decisions of public health officials, policymakers, and researchers in managing the pandemic.

This analysis will help in evaluating the global response to the pandemic and preparing for future public health challenges.

## Dataframe: `day_wise`

- **Date**: The specific date on which the data was recorded.
- **Confirmed**: The total number of confirmed COVID-19 cases up to that date.
- **Deaths**: The total number of deaths caused by COVID-19 up to that date.
- **Recovered**: The total number of recovered COVID-19 patients up to that date.
- **Active**: The total number of active COVID-19 cases on that date (calculated as `Confirmed - Deaths - Recovered`).
- **New cases**: The number of new confirmed COVID-19 cases reported on that date.
- **New deaths**: The number of new deaths caused by COVID-19 reported on that date.
- **New recovered**: The number of new recoveries from COVID-19 reported on that date.
- **Deaths / 100 Cases**: The ratio of deaths per 100 confirmed cases.
- **Recovered / 100 Cases**: The ratio of recoveries per 100 confirmed cases.
- **Deaths / 100 Recovered**: The ratio of deaths per 100 recoveries.
- **No. of countries**: The number of countries reporting COVID-19 cases on that date (i.e., how many countries were affected by that time).

## Analysis

### Confirmed Cases
- Initially, the number of confirmed COVID-19 cases was very low. 
- Over time, the number of confirmed cases increased significantly, showing a clear upward trend as the pandemic spread across more dates.

### New Cases
- The number of new cases fluctuated over time.
- Sometimes it remained constant, while at other times it spiked or dropped.
- This inconsistency in new cases contributed to the overall increase in confirmed cases since many new cases were not immediately recovering.

### Active Cases
- The number of active cases represents the currently infected individuals at a given time.
- This number increased linearly over time, reflecting that new cases were not recovering quickly enough to offset the number of new infections.

### New Deaths
- Initially, the number of new deaths was very high, with a peak around mid-April 2020 when daily deaths reached 864.
- After this peak, the number of new deaths fluctuated, with periods of increase and decrease, likely influenced by the availability and effectiveness of treatments in different regions.

### Total Deaths
- The total number of deaths was very low around March 2020 but increased steadily over time.
- By June 2020, the total number of deaths had reached a significant peak, reflecting the cumulative impact of the pandemic.

### Recovered Cases
- The number of recovered cases showed a positive trend, increasing over time.
- Initially, recoveries were very few, but as treatments improved and more people received care, the number of recoveries grew exponentially.

### Deaths per 100 Cases
- This metric shows the proportion of deaths among every 100 confirmed cases.
- Initially, the death rate was high, peaking around May 2020.
- Over time, as the number of new cases stabilized and recoveries increased, the death rate per 100 cases decreased.

### Recovered per 100 Cases
- This metric represents the proportion of recoveries among every 100 confirmed cases.
- Initially low, it peaked in March 2020 when about 55 out of every 100 cases were recovering.
- After a brief decline, the recovery rate improved again post-April, stabilizing around 47 recoveries per 100 cases by June.

### Deaths per 100 Recovered
- This analysis shows the proportion of deaths among every 100 recoveries.
- In the early stages (February 2020), this rate was very high, with 134 deaths per 100 recoveries, indicating severe outcomes for many patients.
- Over time, this ratio decreased significantly, reflecting better treatment outcomes and increased survival rates.

### New Recovered
- The number of new recoveries started low but increased steadily over time, peaking around June 2020.
- This trend shows that more people were recovering as treatments became more effective and widely available.

### Number of Countries Affected
- This column shows the number of countries reporting COVID-19 cases.
- Initially, less than 15 countries were affected.
- By mid-2020, the virus had spread globally, with 187 countries reporting cases, indicating the widespread reach of the pandemic.

---

## Dataframe: `country_wise`

1. **Country/Region**: The specific country or region where the data was recorded.
2. **Confirmed**: The total number of confirmed COVID-19 cases in the country/region.
3. **Deaths**: The total number of deaths caused by COVID-19 in the country/region.
4. **Recovered**: The total number of recovered COVID-19 patients in the country/region.
5. **Active**: The total number of active COVID-19 cases in the country/region (calculated as `Confirmed - Deaths - Recovered`).
6. **New cases**: The number of new confirmed COVID-19 cases reported in the country/region on the latest date.
7. **New deaths**: The number of new deaths caused by COVID-19 reported in the country/region on the latest date.
8. **New recovered**: The number of new recoveries from COVID-19 reported in the country/region on the latest date.
9. **Deaths / 100 Cases**: The ratio of deaths per 100 confirmed cases in the country/region, expressed as a percentage.
10. **Recovered / 100 Cases**: The ratio of recoveries per 100 confirmed cases in the country/region, expressed as a percentage.
11. **Deaths / 100 Recovered**: The ratio of deaths per 100 recoveries in the country/region, expressed as a percentage.
12. **Confirmed last week**: The total number of confirmed COVID-19 cases in the country/region reported in the previous week.
13. **1 week change**: The change in the number of confirmed cases in the country/region over the past week.
14. **1 week % increase**: The percentage increase in the number of confirmed cases in the country/region over the past week.
15. **WHO Region**: The World Health Organization region to which the country/region belongs.

## Analysis

### Confirmed Cases
- **Overview**: This represents the total number of confirmed COVID-19 cases in each country and region.
- **Top Countries**:
  - The United States has the highest number of confirmed cases.
  - Brazil ranks second, followed by Russia and India.
  - Pakistan is at the lowest among the top 15 countries.
- **Regional Insights**:
  - The Americas region (primarily the US) leads in confirmed cases.
  - Europe, represented by Russia, is also significantly impacted.
  - India represents the South-East Asia region, ranking fourth.
- **Implication**: The high number of confirmed cases in the US and Brazil indicates a severe spread of the virus, necessitating stringent measures to control the outbreak.

### Active Cases
- **Overview**: This is calculated as the number of confirmed cases minus the number of deaths and recoveries, representing the currently active COVID-19 cases.
- **Top Countries**:
  - The United States again tops the list, followed by Brazil, the UK, Russia, and India.
  - South Africa is at the lowest among the top 15 countries.
- **Regional Insights**:
  - The Americas region (primarily the US) has the highest number of active cases.
  - The Africa region has the lowest, with South Africa representing it.
- **Implication**: High active cases in the US and Brazil highlight ongoing transmission, requiring continued public health interventions.

### New Cases
- **Overview**: This represents the number of new confirmed cases reported on the latest date.
- **Top Countries**:
  - The United States reports the highest number of new cases.
  - Brazil ranks second, with significant new cases also reported in India.
  - Sweden is at the lowest among the top 15 countries.
- **Regional Insights**:
  - The Americas region, particularly the US and Brazil, continues to report high numbers of new cases.
  - South-East Asia, represented by India, is also experiencing a notable increase.
  - Europe (Sweden) shows lower new cases compared to the top countries.
- **Implication**: The high number of new cases in the US and Brazil suggests ongoing challenges in controlling the spread, while India is also seeing a significant rise.

### Recoveries
- **Overview**: This represents the total number of recovered COVID-19 patients.
- **Top Countries**:
  - The United States and Brazil lead in the number of recoveries.
  - Russia ranks third, followed by India.
  - France is at the lowest among the top 15 countries.
- **Regional Insights**:
  - The Americas region (US and Brazil) shows the highest recovery numbers.
  - Europe, represented by Russia and France, also has significant recoveries.
  - India in South-East Asia shows substantial recoveries as well.
- **Implication**: High recovery numbers in the US and Brazil indicate effective recovery efforts despite the high number of cases.

### Deaths
- **Overview**: This represents the total number of deaths caused by COVID-19.
- **Top Countries**:
  - The United States and Brazil have the highest death tolls.
  - The UK, Mexico, and France follow.
  - India has a relatively lower death count compared to these countries.
- **Regional Insights**:
  - The Americas region (US and Brazil) again shows the highest death numbers.
  - Europe (UK, France, Spain) has also been significantly impacted.
  - India’s lower death count is notable compared to its high number of confirmed cases.
- **Implication**: The high death toll in the US and Brazil highlights the severity of the pandemic in these regions.

### WHO Region Analysis:
- **Overview**: This represents the World Health Organization region to which each country belongs.
- **Regions**:
  - The regions include Europe, the Americas, South-East Asia, and Africa.
  - The Americas region shows the highest numbers in several categories (cases, deaths, recoveries), reflecting the severe impact of COVID-19 in countries like the US and Brazil.
- **Implication**: The regional distribution highlights the varying impact of COVID-19, with the Americas being the hardest hit, followed by Europe and South-East Asia.

## Conclusion
The analysis reveals the significant impact of COVID-19 across different countries and regions. The United States and Brazil stand out with the highest numbers in confirmed cases, active cases, deaths, and recoveries. Europe, represented by countries like the UK, France, and Italy, shows higher death rates per 100 cases and recoveries, indicating more severe outcomes in these regions. India, despite being heavily affected, shows relatively lower death rates and significant recovery numbers, reflecting effective management of the pandemic. The data underscores the ongoing challenges and the need for continued public health efforts to control the spread and mitigate the impact of COVID-19 globally.
