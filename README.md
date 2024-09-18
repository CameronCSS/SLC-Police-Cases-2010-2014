<a name="readme-top"></a>

![SLC Police Cases 2011-2014 (1)](https://github.com/user-attachments/assets/6501f271-371a-48e5-91fb-cb8635e5e20c)


## About The Project
Utah provides publicly accessible data on [**Police Cases between 2011-2014**](https://www.opendatanetwork.com/dataset/opendata.utah.gov/a56y-d97m), including details on case types, crime locations, and both 'Reported' and 'Closed' dates for each incident.

The goal of this project is to conduct an in-depth analysis of this data to uncover crucial insights that can enhance police policies and drive community engagement and business success for the local economy.

<br>
<br>

Detailed code analysis and findings are documented in this [notebook](https://www.kaggle.com/code/cameronseamons/slc-crime-data-2010-2014)

<br>

><p align="left"><a href="#insights"> ➡️ Jump straight to the insights</a></p>
>
><p align="left"><a href="#recommend"> ✅ View my Recommendations</a></p>
>


<hr>

## 🧹 Data Cleaning
<sub>*▼ Click arrow to view Data Cleaning Steps*</sub>

<details>
    <summary>Data Cleaning Steps</summary>
    <br>
    
- **Deal with Duplicates:**
    - Identified and removed Duplicates that were not purposeful
- **Fix or Remove NA Values:**
    - Removed rows/columns with NA values
    - Separated data into two to track same day closing, and cases that took time to close
- **Correct Incorrect Data:**
    - Some cases were listed as ‘Closed’ before they were reported
- **Handling Missing Values:**
    - Missing values are different than NA values
    - Handled a few cases of missing data (2015 was removed as it only had under 100 cases total and would skew yearly results)
- **Fix Data Types:**
    - Converted all dates to date types
    - Converted location data to longitude and latitude for mapping
- **Fix Column Names:**
    - Standardizes column names and removed for easier understanding
    - Removed irrelevant columns to simplify the data we are working with
- **Handling Outliers:**
    - Used Interquartile Range (IQR) to identify outliers
    - Split data in two with and without outliers to identify their significance
- **Standardizing Formats:**
    - Ensure consistency in date formats and numerical formats for graphing and calculations
- **Data Validation:**
    - Performed consistency checks to verify data
- **Data Aggregation:**
    - Grouped data by Crime and by dates to discover trends
    - Aggregate existing data to create new values to help identify trends
- **Documenting Steps:**
    - Keep a record of the data cleaning steps performed to ensure reproducibility and to provide clarity for your future self or other team members.
</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="insights"></a>
# 💡 Insights on Crime trends

> **Reminder:** 
Data only includes reported crime in Salt Lake City between the years 2010 and 2014.
> 

The dataset reveals a broad range of different crimes, with **LARCENY** being the most frequent, followed by **PUBLIC ORDER** and **TRAFFIC** offenses.

*The total number of recorded crimes varies significantly by type, indicating diverse criminal activities.*

### **Crime Trends by Day of the Week**

**Thursday** emerges as the day with the highest overall crime, followed closely by **Friday**.

- **LARCENY** peaks on **Monday**.
    - **Possible Explanation:** The start of the workweek may create opportunities for looting as people return to their routines. The increased activity and busier environments on Mondays might be exploited by criminals.
    - **Larceny** occurs **29% more** than traffic violations
- **TRAFFIC** offenses are most frequent on **Friday**.
    - **Possible Explanation:** The end of the workweek often brings relaxed attitudes and increased social activities, potentially leading to more traffic offenses.
- **ASSAULTS** crimes are highest on **Saturdays**.
    - **Possible Explanation:** Weekend social activities often lead to increased alcohol consumption and potential conflicts, which could explain the higher incidence of assaults.

### Longest and Average Case Processing Times

**98%** of cases are closed the same day they’re reported, while **5,462 cases took more time to process**

- **FRAUD** cases have the longest processing time, with the longest taking **1770 days** to be closed
- **EXPLOITATION** cases have the highest **average of 231 days** from report to close
- Complex cases take, on average, **50% longer** to close than other crimes.

### Seasonal Patterns

**Summer** has the highest crime count. With an **8% higher** crime rate than other seasons on average

- **Possible Explanation:** The summer is the most common time for personal activities. With so many people away from school and their regular routines it could possibly explain why most crime is reported in the summer.

*The data suggests seasonal variation in crime rates, with different types of crimes peaking in specific seasons.*

### Location trends

- There were over **4,200 Crimes** reported on the unfortunately named “Hope Ave”
- A majority of reported crimes were in the most populated areas of salt lake, often where large clusters of business were located

  <p align="right">(<a href="#readme-top">back to top</a>)</p>

<a name="recommend"></a>
# ✅ Recommendations

> Based on the data, here are a few targeted recommendations for the state to consider:
> 
1. **Enhance Security for High-Crime Days and Areas**
    - **Targeted Security:** Implement heightened security measures on Mondays (for larceny) and Saturdays (for assaults). Increase security personnel, especially in high-crime areas like Hope Ave and around popular business zones.
    - **Community Engagement:** Develop community outreach programs to foster collaboration among local businesses. This can create a business watch network that enhances safety and makes Salt Lake City a more attractive location for new businesses.
    
2. **Invest in Fraud and Embezzlement experts**
    - **Fraud Prevention Programs:** Invest in internal experts, as these complex cases have long processing times. This will help prevent and address local business more effectively, protecting our local economy from additional financial loss.
    - **Education and Awareness:** Conduct workshops or informational sessions for local employees and customers on how to recognize and report suspicious activities. This can help in reducing incidents and speeding up case resolutions.
3. **Leverage Technology**
    - **Advanced Surveillance:** Invest in surveillance technology and analytics to better monitor crime trends and respond quickly. Technologies such as AI-driven analytics can help identify patterns and potential threats more efficiently.
    - **Data Analysis Tools:** Use data analysis tools to continuously monitor and assess crime trends in relation to local business operations. This will help in making informed decisions about security and operational adjustments in our area.
  
<p align="right">(<a href="#readme-top">back to top</a>)</p>


# 📊 Graphs and Tables
> → [Data Report](https://www.canva.com/design/DAGQ3-L9EaI/pbXbXFWactecFB4y8hVrIg/view)  <sub>**Click to view the report*</sub>
>

<sub>*Use ▼ dropdown arrows to view Data*</sub>


<details>
<summary>Seasonal Patterns </summary>

### **Worst Season**

| Season | Total Crimes |
| --- | --- |
| Summer | 58704 |
| Fall | 54349 |
| Spring | 53351 |
| Winter | 49714 |

### **Worst 3 crimes per Season**

![image (1)](https://github.com/user-attachments/assets/c4cc14ae-71aa-411e-bf4a-fc9bdfa8bf77)


</details>

<details>
<summary>Worst crime by year</summary>

| Year | Worst Crime | Count |
| --- | --- | --- |
| 2010 | LARCENY | 10380 |
| 2011 | TRAFFIC | 9238 |
| 2012 | LARCENY | 11491 |
| 2013 | LARCENY | 11894 |
| 2014 | LARCENY | 12756 |

</details>

<details>
<summary>Worst day of the week</summary>

| Day of Week | Count |
| --- | --- |
| Thursday | 33575 |
| Friday | 33184 |
| Wednesday | 31949 |
| Tuesday | 30946 |
| Monday | 30585 |
| Saturday | 30559 |
| Sunday | 25320 |

</details>

<details>
<summary>Worst day of the week Per Crime</summary>

| Crime | Day of Week | Count |
| --- | --- | --- |
| LARCENY | Monday | 5907 |
| TRAFFIC | Friday | 5282 |
| PUBLIC ORDER | Friday | 5223 |
| PUBLIC PEACE | Thursday | 2722 |
| ASSAULT | Saturday | 2508 |
| ESCAPE | Thursday | 2409 |
| INV OF PRIVACY | Thursday | 1658 |
| DRUGS | Thursday | 1638 |
| DAMAGED PROP | Monday | 1605 |
| STOLEN VEHICLE | Monday | 1218 |
| BURGLARY | Monday | 1115 |
| LIQUOR | Wednesday | 1052 |
| FRAUD | Friday | 646 |
| OBST POLICE | Saturday | 440 |
| FAMILY OFFENSES | Friday | 299 |
| ROBBERY | Saturday | 251 |
| FORGERY | Tuesday | 206 |
| WEAPON OFFENSE | Friday | 182 |
| COMMERCIAL SEX | Thursday | 145 |
| MORALS-DECENCY | Thursday | 143 |
| SEXUAL OFFENSE | Thursday | 125 |
| SEXUAL ASSAULT | Sunday | 83 |
| PUB PEACE-HOST | Monday | 75 |
| STOLEN PROP | Wednesday | 74 |
| KIDNAP | Friday | 55 |
| ARSON | Friday | 43 |
| CONSERVATION | Sunday | 29 |
| HEALTH/SAFETY | Wednesday | 23 |
| OBST JUDICIAL | Wednesday | 22 |
| SEX OFFENSES | Wednesday | 19 |
| COUNTERFEITING | Monday | 17 |
| EMBEZZLEMENT | Wednesday | 12 |
| PORNOGRAPHY | Friday | 12 |
| WEAPONS | Thursday | 8 |
| PROPERTY CRIME | Tuesday | 7 |
| JUVENILE OFF | Monday | 7 |
| HOMICIDE | Saturday | 7 |
| EXTORTION | Tuesday | 7 |
| THREATS | Thursday | 7 |
| EXPLOITATION | Friday | 3 |
| RUNAWAY JUV | Tuesday | 3 |
| PUB PEACE | Saturday | 2 |
| STOLEN VEH | Wednesday | 1 |
| BRIBERY | Monday | 1 |
| CIVIL RIGHTS | Saturday | 1 |
| TAX REVENUE | Thursday | 1 |
| CRIMES AGNST PER | Monday | 1 |
| OBST JUD | Friday | 1 |
| ENTICEMENT | Friday | 1 |
| SMUGGLING | Monday | 1 |
| EXPL-HUMAN TRF | Monday | 1 |
| PRIV | Monday | 1 |
| GAMBLING | Sunday | 1 |
| IMMIGRATION | Monday | 1 |
| ABORTION | Monday | 1 |


</details>

<details>
<summary>Count of each crime</summary>

| Crime | Count |
| --- | --- |
| LARCENY | 55709 |
| PUBLIC ORDER | 43825 |
| TRAFFIC | 43171 |
| PUBLIC PEACE | 22357 |
| ASSAULT | 20331 |
| ESCAPE | 19552 |
| DAMAGED PROP | 15065 |
| DRUGS | 12502 |
| STOLEN VEHICLE | 11303 |
| INV OF PRIVACY | 10548 |
| BURGLARY | 9630 |
| LIQUOR | 7484 |
| FRAUD | 6175 |
| OBST POLICE | 3145 |
| ROBBERY | 2002 |
| FAMILY OFFENSES | 1918 |
| FORGERY | 1808 |
| WEAPON OFFENSE | 1462 |
| MORALS-DECENCY | 1012 |
| COMMERCIAL SEX | 996 |
| SEXUAL OFFENSE | 763 |
| SEXUAL ASSAULT | 750 |
| STOLEN PROP | 548 |
| KIDNAP | 333 |
| PUB PEACE-HOST | 283 |
| ARSON | 268 |
| OBST JUDICIAL | 215 |
| CONSERVATION | 176 |
| HEALTH/SAFETY | 136 |
| SEX OFFENSES | 120 |
| COUNTERFEITING | 116 |
| EMBEZZLEMENT | 62 |
| PORNOGRAPHY | 58 |
| PROPERTY CRIME | 47 |
| WEAPONS | 43 |
| EXTORTION | 41 |
| JUVENILE OFF | 31 |
| HOMICIDE | 30 |
| THREATS | 17 |
| RUNAWAY JUV | 13 |
| SMUGGLING | 7 |
| GAMBLING | 6 |
| EXPLOITATION | 5 |
| PUB PEACE | 4 |
| PRIV | 3 |
| CRIMES AGNST PER | 2 |
| IMMIGRATION | 2 |
| BRIBERY | 2 |
| STOLEN VEH | 1 |
| ABORTION | 1 |
| EXPL-HUMAN TRF | 1 |
| TEST | 1 |
| OBST JUD | 1 |
| ENTICEMENT | 1 |
| CIVIL RIGHTS | 1 |
| TAX REVENUE | 1 |

</details>

<details>
<summary>Longest time to process cases</summary>

| Crime | Case Duration |
| --- | --- |
| FRAUD | 1770 |
| PUBLIC PEACE | 1536 |
| PUBLIC ORDER | 1403 |
| EXPLOITATION | 1154 |
| LARCENY | 1134 |

</details>

<details>
<summary>Average time to process cases</summary>

| Crime | Case Duration |
| --- | --- |
| EXPLOITATION | 230.80 |
| FRAUD | 11.83 |
| EMBEZZLEMENT | 8.88 |
| KIDNAP | 4.25 |
| FORGERY | 4.04 |

</details>

### Areas of crime (Map)

Full map is best viewed on Desktop.

View full-scale map →  [LINK](https://public.tableau.com/shared/PYGJGN2XC?:display_count=n&:origin=viz_share_link)

<sub>**Map Preview*</sub>

![image](https://github.com/user-attachments/assets/9fe1414c-d4f3-4d61-b21a-5ac30164013c)


----

<a name="Contact"></a> 
## <a href="https://camdoesdata.com/#contact">Contact Me</a>

  </table>
  <p style="margin-left: auto;">
    <a href="https://drive.google.com/file/d/1YaM4hDtt2-79ShBVTN06Y3BU79LvFw6J/view?usp=sharing" target="_blank" rel="noopener noreferrer">
      <img src="https://user-images.githubusercontent.com/121735588/215364205-abdfc0ac-53db-4733-8d43-b57c1bafb802.png" alt="Resume button">
    </a>
  </p>
</div>


<p align="right">(<a href="#readme-top">back to top</a>)</p>

