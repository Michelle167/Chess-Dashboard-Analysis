
# Chess Dashbard Analysis 
## **Overview**
This project analyzes competitive chess game data to uncover the key factors influencing match outcomes beyond player rating. The analysis focuses on outcome distribution, opening selection, rating differentials, time pressure levels, and upset frequency patterns.

The goal is to identify how strategy, time control, and psychological performance interact to shape results, demonstrating that rating alone is not a sufficient predictor of success.

## **Dataset & Preprocessing**
### **Dataset Source**
- Obtained from Kaggle: [Chess Game Dataset (Lichess)](https://www.kaggle.com/datasets/datasnaek/chesshttps)
- Contains:
- Game ID;
- Rated (T/F);
- Start Time;
- End Time;
- Number of Turns;
- Game Status;
- Winner;
- Time Increment;
- White Player ID;
- White Player Rating;
- Black Player ID;
- Black Player Rating;
- Moves;
- Opening Eco;
- Opening Ply
 
## **Preprocessing Steps**
- **Data Cleaning** → Removed duplicates and standardized categorical values.
- **Rating Differential Calculation** → Computed rating gap between players.
- **Upset Identification** → Flagged games where lower-rated player won.
- **Pressure Categorization** → Classified games into Low and Moderate pressure levels.
- **Opening Grouping** → Aggregated openings by ECO code and name.
- **KPI Derivation** → Calculated volatility, conversion rates, and neutralization rates..

## **Data Flow into Power BI**
- **Raw Data Import** → Dataset loaded into Power BI.
- **Power Query Transformations** → Applied cleaning and calculated columns.
- **Data Modeling** → Structured as a fact table with derived measures.
- **DAX Measures Created**:
    - Upset Frequency Rate
    - Opening Volatility Index
    - Pressure Conversion Rate
    - Average Rating Differential
    - Draw Neutralization Rate
- **Visualizations Built** → KPI cards, stacked bars, clustered columns, and line charts. 

## Key Findings
### Overall Outcome Distribution
|Outcome  | Percentage | 
| :----- | -------: |
| White wins | 52% | 
| Black Wins | 43%  | 
| Draws | 5% |

White maintains a slight first-move advantage, but matches remain highly competitive with low draw frequency.


### Upset, Rating & Pressure Dynamics
|Metric | Value | 
| :----- | -------: |
|Upset Frequency Rate |  42.14% |
| Average Rating Differential| 251.35 |  
| Draw Neutralization Rate|5.41%| 
| Pressure Conversion Rate|  52.04% |

- **Upset Frequency Rate (42.14%)** shows a highly volatile competitive environment where lower-rated players frequently outperform expectations.

- **Average Rating Differential (251.35)** suggests rating gaps are moderate — large enough to set expectations but small enough to allow competitive disruption.

- **Pressure Conversion Rate (54.05%)** indicates that just over half of high-pressure situations are successfully converted into wins. This reflects moderate psychological resilience, highlighting decision-making under time constraints as a key performance driver.

- **Draw Neutralization Rate (5.41%)** reveals that defensive stabilization is rare, meaning games tend to end decisively rather than through strategic neutralization.


### Opening & Strategic Influence
- **Opening Volatility Index (95.32)** confirms that opening selection strongly shapes match trajectory and decisiveness.

- Certain ECO codes generate significantly higher upset frequencies, reinforcing the influence of structural and tactical complexity over rating advantage.


### Time Pressure & Game Volume
|Format | Low Pressure | Moderate Pressure|
| :----- | :-----: | -------: |
|Blitz |  8.5K | 4.6K |
| Rapid |  4.9K| 336 |
| Classical| 204 | — |

Blitz dominates total volume and moderate pressure conditions, increasing cognitive load and decisiveness.


## Visualizations
Screenshots of the Power BI dashboard are included in the /Screenshots folder:

- Overall Game Outcome Distribution →  
  <p align="center">
    <img src="https://github.com/Michelle167/Chess-Dashboard-Analysis/blob/main/Screenshots/Overall%20Game%20Outcome%20Distribution.png?raw=true" width="500"/>
  </p>
  
- Game Outcome By Opening →
  <p align="center">
    <img src="https://github.com/Michelle167/Chess-Dashboard-Analysis/blob/main/Screenshots/Game%20Outcome%20By%20Opening.png?raw=true" width="500"/>
  </p>
  
- Draw Rate By Opening →
  <p align="center">
    <img src="https://github.com/Michelle167/Chess-Dashboard-Analysis/blob/main/Screenshots/Draw%20Rate%20By%20Opening.png?raw=true" width="500"/>
  </p>
  
- Game Volume By Category & Pressure Level →
  <p align="center">
    <img src="https://github.com/Michelle167/Chess-Dashboard-Analysis/blob/main/Screenshots/Game%20Volume%20By%20Category%20&%20Time%20Pressure.png?raw=true" width="500"/>
  </p>
  
- Total Upsets By ECO Code →
  <p align="center">
    <img src="https://github.com/Michelle167/NYC-Traffic-Accident-Analysis/blob/main/Screenshots/Street%20Hotspots.png" width="500"/>
  </p>
  
- KPI Summary Cards →
   <p align="center">
    <img src="https://github.com/Michelle167/Chess-Dashboard-Analysis/blob/main/Screenshots/KPI%20Summary.png?raw=true" width="500"/>
  </p>
  
Full dashboard available in:
<p align="center">
    <img src="https://github.com/Michelle167/Chess-Dashboard-Analysis/blob/main/Screenshots/Chess%20Game%20Dashboard.png?raw=true" width="500"/>
  </p>

  
## Insights & Recommendations
### Key Insights
- Chess outcomes are highly volatile despite rating differences.
- Opening choice significantly influences match trajectory.
- Blitz format intensifies unpredictability due to time pressure.
- Moderate rating gaps create fertile ground for upsets.
-Decisive play dominates over defensive strategies.

### Recommendations
- Develop predictive models incorporating opening and time control.
- Analyze player-specific resilience under pressure.
- Incorporate opening risk profiling into performance preparation.
- Expand analysis into longitudinal rating progression.

### Conclusion
This project demonstrates that chess performance is multi-dimensional. While rating provides a baseline expectation, opening strategy, time pressure exposure, and psychological conversion under stress are decisive factors in determining outcomes.

The interactive Power BI dashboard transforms raw match data into actionable performance insights, offering a structured framework for strategic and analytical evaluation of competitive chess.


 

