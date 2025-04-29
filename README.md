### Business Understanding

The aviation industry presents complex risks that require data-driven insights to inform operational decisions. 

This analysis leverages the National Transportation Safety Board's aviation accident dataset (1962-2023) to evaluate risk patterns and guide strategic recommendations for entering the aviation sector. 

The dataset includes critical attributes such as accident timelines, aircraft purpose, weather conditions, engine configurations, and injury severity, which will be analyzed to identify low-risk aircraft profiles.

## Data Pre-processing

I did Data Pre-processing, Cleaning and Manipulation to fully understand our data set before delving into comprehensive Data Analysis.Thereafter, we will draw actionable insights and recommendations from the data analysed and advise the company on the possible risks and how to avoid them.

The Aviation Accident Database & Synopses, up to 2023 Data was downloaded from Kaggle as a Zip file and later extracted into CSV files 
The data was provided by  the National Transportation Safety Board .Below is the link to the Data source:
**Source**: [**Dataset**] (https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses)

It contained aviation accident data from 1962 to 2023 about aviation accidents in the U.S and aviation waters.The Aviation data was later loaded to Jupyter notebook as a data frame for further cleaning, manipulation and analysis

I loaded the aviation dataset and :
1.Cleaned the column names, fixing date formats, and adding a "Year" column 
2.Removed columns with too much missing information 
3.Imputation of important columns such as engine types, models
4.Checked for duplicates and standardized the categories
5.Prepared a clean, well-structured dataset ready for trend analysis and studying flight risks.
6.Finally imported the cleaned data set



### Business Goal
The business aims at:
### 1.Risk Profiling:
This would be helpful to Quantify how factors like weather instrumentation, engine count, and flight purpose correlate with accident likelihood and severity to prioritize safer aircraft models.

### 2.Understanding the trends hence need for proper Trend Analysis
Identify historical patterns in accidents such as  temporal trends, geographic hotspots to avoid high-risk operational conditions.

### 3.Obtaining Actionable Recommendations:
We will Provide evidence-based guidance for selecting low-risk aircraft and optimizing operational protocols.



### Questions to Address:
1. Has the number of accidents decreased over time due to technological or regulatory improvements?
2. Do certain flight purposes (e.g., personal, commercial) correlate with higher accident rates?
3. Which is the safest Make and Model of aircraft?
4. Do Instrument Meteorological Conditions (IMC) contribute to accidents compared to Visual Meteorological Conditions (VMC)?
5. Does the number of engines impact accident severity?


### Data Analysis
The analysis was done on the Aviation Analysis.ipynb Python Notebook

### Key Findings
Below is a summary of the key findings:
Aircraft accidents before 1980 were extremely minimal, suggesting both very few accidents occurred during this time or that data collection and record-keeping systems were either weak or non-existent. Accurate accident reporting likely gained momentum post-1980 when aviation oversight improved globally.

Starting from 1980, there was a sharp rise in the number of recorded aircraft accidents, reaching a peak shortly afterward. However, from the early 1980s to 2020, we observe a steady and significant decline in accident numbers, reducing to approximately 1,600 by 2020. This sharp and consistent decrease strongly suggests major improvements in aviation safety over time. While multiple factors could contribute to this positive trend, one notable driver has been technological advancement, from better navigation systems, automated control systems, to stricter maintenance and operational standards.

The historical accident data show that personal-use and instructional aircraft have the highest accident rates. In contrast, public (and by extension, commercial) aircraft experience significantly fewer accidents. This finding suggests that aircraft operated under strict regulatory environments, professional maintenance schedules, and with highly trained pilots are associated with markedly lower risk.

When we examine country-level accident distribution, the United States stands out significantly with the highest number of aircraft accidents compared to other countries, which reported relatively lower numbers. This could be explained by the much larger number of aircraft movements, a vast network of private pilots, and the widespread use of personal aircraft in the U.S. compared to other nations.

In terms of aircraft usage, personal aircraft accounted for the highest proportion of accidents, closely followed by instructional (training) aircraft. Public aircraft, on the other hand, recorded the least number of accidents. This raises important questions about the experience levels of pilots operating personal aircraft, the frequency and quality of maintenance conducted on personal aircraft, and possibly, the lower regulatory scrutiny in private aviation compared to public or commercial aviation sectors.

Further analysis into flight operation conditions reveals that accidents were more rampant when pilots operated under Visual Meteorological Conditions (VMC) — that is, flying based on visual reference rather than relying on instruments. In contrast, accidents that occurred under Instrument Meteorological Conditions (IMC) were significantly fewer. This finding suggests that reliance on visual cues, possibly in adverse or misleading conditions, increases the risk of accidents, highlighting the importance of strong instrument training and certification for pilots.

When considering the extent of damage, accidents under VMC often resulted in substantial aircraft damage or destruction. In comparison, incidents under IMC conditions were less severe in terms of aircraft damage. This could indicate that pilots operating in IMC are more likely to adhere to strict operational procedures, or it could point to the effectiveness of instruments and structured flight paths under such conditions.

Additionally, training aircraft are naturally prone to higher accident risks due to the nature of flight training — student pilots practicing maneuvers, frequent takeoffs, and landings, all inherently riskier activities. However, the high accident rate among personal-use aircraft is more concerning. It hints at deeper systemic issues such as lax maintenance routines, less formal pilot training, older aircraft technology, and potentially more relaxed attitudes toward flight safety.

Commercial aviation, in contrast, enjoys much stronger safety records, which can be attributed to stringent regulatory requirements, technological sophistication, highly trained crews, and a culture of routine inspections and risk management. This underscores the critical role of regulation, training, and maintenance in ensuring aviation safety.

Looking at engine types, reciprocating  engines were found to be the most common among aircraft involved in accidents. These engines are typically found in smaller, older aircraft, again reinforcing the idea that older, privately owned aircraft may present greater risks. 

All the Models of Cessna are prone to accidents and have the highest number of accidents since 1981. The company needs to be careful when purchasing any model of Cessna. Piper PA-28-140 is also prone to accident and has a higher number of accidents of 932 compared to Cessna 50 which has 829 accidents.
All the Models of Fairchild(KR-31,M 62A-3,M-62A (PT-19), M62A (PT-19)) and Zwicker Murray R have only had 1 cases of accidents since 1981 indicating how risk free and safer they are.The company should consider purchasing either Fairchild or Zwicker Murray R.

Furthermore, aircraft with only one engine were associated with the highest accident rates. While two- and four-engine aircraft also experience accidents, the rates are much lower. Interestingly, the data shows that adding more engines doesn't linearly reduce accident risk — for instance, four engines do not guarantee four times the safety compared to one engine. This suggests that operational practices, pilot competence, and maintenance quality play more crucial roles than simply the number of engines.

The findings were visually presented in a Tableau dashboard with the link below:
**View Dashboard**: [**Interactive Dashboard**](https://public.tableau.com/views/AviationRiskAnalysis_17458568467580/Dashboard?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Furthermore, a quick view of the notebook gives the following visuals:
![alt text](<Purpose of Aircraft against Number of Accidents.png>) 
![alt text](<Accident Trends.png>) 
![alt text](<Accidents and Weather Condition Tools.png>) 
![alt text](<Aircraft Accident Frequency by Engine Count.png>) 
![alt text](<Most Accident Prone Aircraft.png>) 
![alt text](<Number of Injured and Uninjured.png>) 
![alt text](<Purpose and Engine Types vs Number of Accidents.png>)



#### Key Recommendations


 1. The company should consider purchasing either Fairchild or Zwicker Murray R.The company needs to be careful when purchasing any model of Cessna. Piper PA-28-140 is also prone to accident and has a higher number of accidents of 932 compared to Cessna 50 which has 829 accidents.

All the Models of Fairchild(KR-31,M 62A-3,M-62A (PT-19), M62A (PT-19)) and Zwicker Murray R have only had 1 cases of accidents since 1981 indicating how risk free and safer they are.

2. The company should invest in Aircrafts with 6 or 8 Engine Count and avoid Single-Engine with Reciprocating  Engines Aircraft 

 Do not invest single-engine piston aircraft commonly used for personal purposes, as they are linked to significantly higher accident rates.

3. With the higher risks associated to the Personal Aircrafts, the company should consider investing more in Commercial Aircrafts.
4. The company should heavily invest in Instruments Metereological Conditions Tools and encourage their pilots to always use IMC as opposed to VMC


### References
1. https://www.youtube.com/c/LukeBarousse
2. Class work
3. https://www.youtube.com/@DataWithBaraa
