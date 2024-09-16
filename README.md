<a name="readme-top"></a>

![SLC Police Cases 2011-2014 (Letter Sized)](https://github.com/user-attachments/assets/aa1fae39-27ca-42b8-9af4-1ef9175a6e85)


## About The Project
My goal is to analyze the crime data to identify and understand trends over time and across different locations in Salt Lake City.
Using Kaggle and a publicaly available dataset [Salt Lake City Police Cases 2011-2014](https://www.opendatanetwork.com/dataset/opendata.utah.gov/a56y-d97m), I performed data cleaning, processed the data to add months, years, season, and even process the location data for a [Tableau Map.](https://public.tableau.com/views/SLCCrimeReports2010-2014/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
<br>
<br>
The whole detailed analysis and findings are documented in this [notebook](https://github.com/CameronCSS/SLC-Police-Cases-2011-2014/blob/main/SLC-crime-data-2010-2014.ipynb)
<br>
<br>

<hr>

### Data Cleaning/Processing Steps


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



# 💡 Insights on Crime trends

---

### **Crime Counts**

The dataset reveals a broad range of crime types, with **LARCENY** being the most frequent, followed by **PUBLIC ORDER** and **TRAFFIC** offenses.

*The total number of recorded crimes varies significantly by type, indicating diverse criminal activities.*

### **Crime Trends by Day of the Week**

**Thursday** emerges as the day with the highest overall crime, followed closely by **Friday**.

- **LARCENY** peaks on **Monday**.
    - **Possible Explanation:** The start of the workweek may create opportunities for looting as people return to their routines. The increased activity and busier environments on Mondays might be exploited by criminals.
- **TRAFFIC** offenses are most frequent on **Friday**.
    - **Possible Explanation:** The end of the workweek often brings relaxed attitudes and increased social activities, potentially leading to more traffic offenses and public disturbances.
- **ASSAULTS** crimes are also highest on **Saturdays**.
    - **Possible Explanation:** Weekend social activities often lead to increased alcohol consumption and potential conflicts, potentially resulting in a higher incidence of assaults.

### Longest and Average Case Processing Times

**98%** of cases are closed on the same day they’re reported, while **5,462 cases took more than 1 day**

- **FRAUD** cases have the longest processing time, with the highest taking **1770 days** to close
- **EXPLOITATION** cases have the highest **average of 231 days** from report to close

### Seasonal Patterns

**Summer** has the highest crime count.

- **Possible Explanation:** The summer is the most common time for personal activities. With so many people away from school and their regular routines it could possibly explain why most crime is reported in the summer.

*The data suggests seasonal variation in crime rates, with different types of crimes peaking in specific seasons.*

## Conclusion

- The data reveals that crime patterns are strongly influenced by the day of the week and seasonal variations. Mondays and Fridays are associated with distinct crime types possibly due to transitions between work and personal life, while weekends see increased crime rates linked to social activities.
- Understanding these patterns can inform targeted crime prevention strategies, such as focused policing on peak days and addressing specific crime types prevalent on different days.
- Additionally, recognizing seasonal trends can help in planning resource allocation throughout the year.

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

