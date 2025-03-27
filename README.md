# CLIMATE CHANGE ANALYSIS
## Project Overview
Climate change significantly affects agricultural productivity at both local and regional scales. In Africa, it remains a critical issue, hindering progress towards achieving the United Nations Sustainable Development Goals (SDGs), particularly:
SDG 13 (Climate Action) - Addressing climate-related challenges in agriculture.
SDG 2 (Zero Hunger) - Improving food security and sustainable agriculture.
By leveraging data-driven approaches, this Datathon aims to identify actionable insights, develop innovative solutions, and contribute to global efforts to mitigate the negative impacts of climate change on agriculture for a more sustainable future.

### Table of Contents
Data source
Tools 
Project Structure
Analysis
Recommendations

### Dataset
The data was gotten from FAO Crop Production and Livestock [Download here](https://www.fao.org/faostat/en/#data/QCL) and NASA Climate data [Download here](https://climate.nasa.gov/vital-signs/global-temperature/?intent=111)

### Data Exploration and Preprocessing
The crop production and livestock dataset consisted of 16 columns and 14,596 rows.
![Screenshot 2025-03-19 222620](https://github.com/user-attachments/assets/74e7048d-485c-45d0-88ba-c764f553165e)

The temperature dataset contained 3 columns and 144 rows.

![Screenshot 2025-03-24 210000](https://github.com/user-attachments/assets/7abf721f-2d9b-467f-8e47-ecf01f504326)

### Data Cleaning and Transformation
Understanding & Selecting Relevant Columns
Data exploratory analysis the data, to understand the trend, look at what is important for the analysis.
Checked for duplicates
Mean imputation method in replacing null values
Unpivot columns to have all the values for different years just in two columns, the year and then the value for that year.
Finally column selection
Crop Production dataset, columns used for analysis: Area, Item, Element, Value, Year.
Global temperature anomalies data, not much cleaning was done there, I just explored the data and selected the years that corresponded to the year I had in the crop production and livestock data to enable a connection.
Temperature dataset, columns selected: Derived Temperature, Smoothed Temperature, Year.

### Data Standardization & Cleaning
Renamed columns for better readability (Area → Countries, Item → Crops).
Standardized data types.
Corrected country names where necessary.
Handled missing values using median imputation.
Unpivoted year columns to consolidate data into a single Year column.

### Cleaned Crop Production and Livestock data
Analysis & Observations
Scope of Analysis
Focused on African countries.
Assessed crop yield, production, and area harvested from 2000 to 2022.
![Screenshot 2025-03-19 225038](https://github.com/user-attachments/assets/4daa5b8a-f6dc-420c-b789-15b189ed158f)


### Terminologies
Temperature Anomalies
A temperature anomaly is the deviation from a long-term average.
Variance in temperature: 0.13, indicating relatively stable temperatures.
High temperature anomaly: 0.93 (warmer than baseline).
Low temperature anomaly: -0.41 (cooler than baseline).

### Key findings
Crop Production & Yield
Total Production: 26.1 million metric tons.
Total Area Harvested: 9.69 million hectares.
Total Yield: 5.78 million metric tons.
Average Crop Yield per Country: 776,000 metric tons.
Total Number of African Countries Analyzed: 54.

Impact of Temperature Anomalies on Crop Production
For the years 2000–2022 only a positive temperature deviation was recorded from the normal temperature.
This positive temperature deviation, posed a threat on crop yields as seen across different African countries that the total production per year is larger than the total yield.
Top performing crops yield in different countries and bottom crops with less yields.
There seems to be a consistency in high total yields for countries like Sudan, Egypt, Morocco, South Africa etc even when there is an increase in the temperature deviations and a low yield in countries like Eritrea, Equatorial guinea, Mauritania, Lesotho, Central African Republic, etc. These are countries that are mostly at risk of Food insecurity.

### Recommendations
Expand Modern Agricultural Practices
Adoption of precision agriculture and climate-smart farming techniques.
Use of drought-resistant crop varieties.
Implementation of smart irrigation systems.

Mechanization & Technological Adoption
Introduction of agricultural machinery and automation.
Increased investment in fertilizers and soil improvement techniques.
Government subsidies for farming equipment and feed.

Climate-Resilient Farming Strategies
Crop diversification to adapt to varying temperature conditions.
Greenhouse and hydroponic farming in regions with extreme anomalies.
Development of early warning systems for extreme weather patterns.

And of course the use of data to analyze and predict high yielding crops and climate conditions favourable to those crops.




