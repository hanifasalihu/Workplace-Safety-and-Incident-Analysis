# Workplace-Safety-and-Incident-Analysis
## Project Objective
I've been hired as a Data Analyst for a manufacturing company that is concerned about the rising number of workplace incidents and safety violations across different departments and shifts. My responsibility is to clean, analyze, and present insights from the data and create an interactive Excel dashboard for management decision-making.
## TASK REQUIREMENTS
A. Data cleaning (mandatory)

B. Analysis using pivot table: Create pivot tables to answer the questions below:

● Which shift records the most incidents?

● Which department has the highest number of incidents?

● What are the top 5 most common incident types?

● What is the distribution of severity levels?

● Which cause category contributes the highest number of incidents?

● What is the average report time and average resolution time by shift and
department.

## Data Cleaning Process:

1. Duplicate data to save the original, & protect worksheet: call it Duplicate

2. Use ALT H+O+I to enlarge cells.

3. Freeze the top rows with freeze panes

4. Check for blanks and treat Column-by-Column 
- IncidentID: since it was in sequence,i dragged it all the way down to fill the blanks.

- Date & Time: Use =TEXT function to seperate date and time into seperate columns. copy and paste as value then delete old date.
- Fill in the blanks using time btw the b4 and after time of the missing time.
- Use year and month function to create columns for Year, Month, useful for charts.
- Shift Column: Use the time column to determine what shift are missing.
- Department,IncidentType, Severity: were determined based on the exact same incidents on each respective rows.
- EquipmentInvolved CauseCategory: filled with other respective rows with the exact same activities.
- NumInjured, ReportTimeMin,ResolveTimeHr: fill in the blanks as Zero and unknown
- Supervisors: Marry was changed to Mary. filled in the blanks with the corresponding incident type they previously supervised. and no supervisor.
- Comments: fill in the blanks as No comment.

5. CREATE NEW PAGE FOR PIVOT TABLE: 9 pivot tables and 4 slicers were created here. 

6. Also corresponding charts was created along side which was move to another sheet(dashboard). 
7. Use conditional formatting  for number Injured - 0 was formatted RED
       - for ReportTimeMin - everything above average of 43 was formatted GREEN
       - for ResolveTimeHr - everything above the average of 11.67 was formatted YELLOW
       - for Supervisor -  no supervisor was highlighted in BLUE
8. Then a table was inserted into the worksheet.

 
## Key Insights:

The company recorded 2,000 total incidents and 3,665 injuries,
with the longest delays occurring in incident resolution (average 11.67 hours). 
Morning (1,508) and Night (1,462) shifts had the highest incident rates. 

Incidents are concentrated in Maintenance (1,324) and Production (1,206), while the leading causes are Slip (551) and Equipment Failure (507). Most cases fall under Low or High severity, indicating a blend of recurring minor hazards and substantial high-risk events.

#### High-Risk Areas:
Maintenance and Production departments contribute more than half of all recorded incidents of 1,324 and 1,200 cases respectively. 

Slip-related incidents are the most common hazard. Morning and Night shifts show elevated incident frequencies linked to fatigue, workload intensity, and reduced supervision. 

Supervisors such as Mary (634 cases) and John (over 300 each) oversee departments with significantly higher case volumes, suggesting deeper operational challenges.


#### Trends Over Time: 
Incident and injury spikes occur in months 1, 3, 5, 7, 8, and 12, indicating seasonal workload pressure, equipment strain, or staffing gaps.
The end-of-year increase suggests cumulative operational stress.


#### Operational Observations:
Reporting is quick (43 minutes), but overall resolution is slow and varies significantly by department. 
Over 945 reports remain incomplete, pointing to gaps in documentation and follow-up, especially during high-demand shifts.


## Recommendations
1.	Strengthen High-Risk Departments: Improve safety checks, maintenance routines, and training in Maintenance and Production.

2.	Reduce Slip Incidents: Enhance floor safety, housekeeping, and PPE compliance.

3.	Improve Incident Resolution: Streamline workflow, enforce timely case closure, and ensure faster escalation.

4.	Enhance Shift Safety: Increase supervision and fatigue management during Morning and Night shifts.
## Conclusion

The dashboard reveals high incident concentration in specific shifts and departments, with delays in resolution contributing to recurring risks. Strengthening targeted controls and improving workflow efficiency will significantly enhance overall workplace safety.

