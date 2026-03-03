
# NYC Traffic Accidents Analysis 
## **Overview**
This project analyzes NYC Accidents records sourced from Kaggle, focusing on accident volume, geographic distribution, temporal trends, vehicle involvement, street hotspots, causes of collision, and road users affected. The goal is to uncover patterns, highlight risk factors, and provide actionable recommendations for improving road safety.

## **Dataset & Preprocessing**
### **Dataset Source**
- Based on NYC Accidents records.
- Obtained from Kaggle: [Global Traffic Accidents Dataset - NYC_Accidents.csv.](https://www.kaggle.com/datasets/adilshamim8/global-traffic-accidents-dataset?select=NYC_Accidents.csv)

- Contains:
- Date & time of crash
- Borough and street location
- Contributing factors (causes of collision)
- Vehicle types involved
- Road users affected
- Injury and fatality counts
## **Preprocessing Steps**
- **Handling Missing**-  Values → Replaced missing boroughs/streets with “Unspecified.”
- Standardizing Categories → Unified vehicle type names.
- **Date & Time Formatting** → Converted timestamps into Month, Day of Week, Time of Day.
- **Aggregation** → Grouped accident counts by borough, street, month, and vehicle type.
- **Derived Metrics** → Calculated totals for injuries, fatalities, and percentages of road users affected.
- **Filter Creation** → Built filters for Crash Day and Time of Day.
## **Data Flow into Power BI**
- **Raw Data Import** → Accident dataset loaded into Power BI.
- **Transformations** → Applied Power Query steps for cleaning and formatting.
- **Modeling** → Dataset kept as a single table (no relationships created).
- **Visualizations** → Built charts, KPIs, and filters to highlight key findings.

## Key Findings
### Accident Volume & Impact
|Metric  | Value | 
| :----- | -------: |
| Total Accidents | ~74K | 
| Road Users Killed |~125K  | 
|Road Users Injured| 753 |
| Cause of Collision | 38 | 
| Vehicle of Collision | 141 | 


### Geographic Distribution
|Borough | Total Accidents | 
| :----- | -------: |
|Unspecified |  ~26K |
| Brooklyn |  ~17K|  
| Queens|~14K| 
|Bronx|  ~9K |
|Manhattan | ~7K  | 
| Staten Island | ~1K | 



### Temporal Trends
|Month | Total Accidents | 
| :----- | -------: |
|January| ~14.2K |
| February | ~13.6K|  
| March|~11K| 
|April| ~4.1K |
|May | ~6.1K | 
| June | ~7.6K |
|July | ~9.1K || 
| August| ~8.7K|

Crash Day and Time of Day are available as filters.


### Vehicle Involvement
|Vehicle Type | Total Accidents | 
| :----- | -------: |
|Sedan |  ~47K |
| Station Wagon |  ~39K|  
| Taxi|~4K| 
|Pick-up Truck|  ~4K |
|Bike | ~3K  | 
| Armored Truck | ~3K | 
| Bus|~2K| 



### Street Hotspots
|Street| Total Accidents | 
| :----- | -------: |
|Unspecified |  ~19.2K |
| Belt Parkway |  ~1.2K|  
| Brooklyn Queens Expresssway|~0.8K| 
|Long Island Expressway|  ~0.7K |
|Federal Streetway | ~0.7K  | 
| Cross Bronx Expressway| ~0.7K | 
| Major Deegan Expressway|~0.6K| 
|Grand Central Expressway |  ~0.6K |
| Broadway |  ~0.6K|  
| Atlantic Avenue|~0.5K| 



### Causes of Collision
|Cause of Collision| Total Accidents | 
| :----- | -------: |
|Unspecified |  ~60K |
| Driver Distraction |  ~20K|  
| Improper Lane Usage|~12K| 
|Following Too Closely|  ~9K |
|Backing Unsafely| ~3K  | 
|Other Vehicular| ~3K | 
| Unsafe Speed|~2K| 
|Traffic Control Disregarded |  ~2K |
| Driver Inexperience |  ~1K|  
| Reaction to Uninvolved Vehicle|~1K| 


### Road Users Affected
|Road User| Total Accidents | 
| :----- | -------: |
|Pedestrians |  33.3% | 
| Motorists|33.3%|
| Cyclists | 33.3%|  


### Visualizations
Screenshots of the Power BI dashboard are included in the /Screenshots folder:

- Accident Volume Summary →  
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Accident%20Volume%20Summary.png" width="500"/>
  </p>
  
- Geographic Distribution →
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Geographic%20Distribution.png" width="500"/>
  </p>
  
- Temporal Trends →
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Temporal%20Trends.png" width="500"/>
  </p>
  
- Vehicle Involvement →
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Vehicle%20Involvement.png" width="500"/>
  </p>
  
- Street Hotspots →
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Street%20Hotspots.png" width="500"/>
  </p>
  
- Causes of Collision →
   <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Causes%20Of%20Collision.png" width="500"/>
  </p>
  
- Road Users Affected →
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Road%20Users%20Affected.png" width="500"/>
  </p>
  
Full dashboard available in:
<p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/NYC%20TRAFFIC%20ACCIDENT%20%20DASHBOARD.png" width="500"/>
  </p>

  
## Insights & Recommendations
### Key Insights
- High accident counts concentrated in Brooklyn and Queens.
- Seasonal peaks in January and February.
- Sedans and station wagons dominate accident involvement.
- Belt Parkway and BQE are major hotspots.
- Driver distraction and lane misuse are leading causes.
- Equal impact across pedestrians, motorists, and cyclists.
Recommendations
- Improve data quality (reduce “unspecified” entries).
- Target high‑risk roads with stricter monitoring.
- Address driver behavior through awareness campaigns.
- Increase patrols during winter months.
- Enhance pedestrian crossings and cycling lanes.
- Stricter enforcement of speed limits and traffic control compliance.

### Conclusion
This project provides a comprehensive analysis of NYC traffic accidents using Kaggle data and Power BI. By combining structured tables, interactive visuals, and actionable recommendations, it highlights critical safety challenges and opportunities for intervention. The findings emphasize the need for better data quality, targeted road safety measures, and behavioral change initiatives to reduce accidents and protect all road users.


 

