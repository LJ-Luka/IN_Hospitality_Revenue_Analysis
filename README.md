# Hospitality Revenue Insights

For final dashboard click [here](https://github.com/LJ-Luka/More_PowerBI_Projects/blob/main/Project/Hospitality_dashboard.pbix) to download the .pbix file. </br>
Metrics and DAX used for the analysis can be found [here](https://github.com/LJ-Luka/More_PowerBI_Projects/blob/main/Project/metrics%20list.xlsx) </br>
The mockup showing the stakeholder requirements can be viewed [here](https://github.com/LJ-Luka/More_PowerBI_Projects/blob/main/Project/mock%20up%20dashboard_atliq%20grands.png) </br>

## Project Summary

### About the project  

The project is an analysis of the hospitality revenue in India. Four major cities are involved, Bangalore, Delhi, Hyderabad, and Mumbai.  </br>
The stakeholder provided a set of requirements. The requirements included key metrics used in the hospitality industry, Revenue, Occupancy Rate, Realisation Rate, Average Daily Rate (ADR), Daily Sellable Room Nights (DSRN), Revenue Per Available Rooms (RevPAR), Daily Booked Room Nights (DBRN) and Daily Utilised Room Nights (DURN). The stakeholder also desired a monthly filter, weekly filter to show week on week changes, and filters for city, property, room type and platform. </br>
A mock-up was drawn to serve as a guide for the final dashboard. Halfway through the project, feedback was received on satisfaction and further expectations for the dashboard. The final dashboard was made considering all the requirements of the stakeholder.  </br>
The dashboard is interactive. It lets you interact with the data by tracking, monitoring, and displaying key business metrics. It lets you drill down into the data, filter and manipulate it.  </br>  
### The steps involved in this project

- Imported data from the source (5 .csv files)
- Used power query to transform and clean the data: checked for blanks, deleted unwanted columns, checked headers for consistency and loaded data. This demonstrates proficiency with the ETL process.
- The data was modelled using the Star Schema. This was done to establish relationships between the tables (using the primary and foreign keys).
- Data Analysis Expressions (DAX), were used to create calculated columns and measures for the analysis.
- The dashboard was created using different charts and visualisations and gives key hospitality revenue insights. Drill down and tooltips were used to show in-depth insights into some tiles. </br>

### Insights from the dashboard
The stakeholders requested for insights into Revenue, Occupancy Rate, Realisation Rate, Average Daily Rate (ADR), Daily Sellable Room Nights (DSRN), Revenue Per Available Rooms (RevPAR), Daily Booked Room Nights (DBRN) and Daily Utilised Room Nights (DURN) </br>

### KPIs
- The total revenue generated is 1.69bn
- The overall occupancy rate is 57.8%
- The DSRN is 2528.0
- The ADR is 12.7k
- The realisation rate is 75%
- The RevPAR is 7.3k
- The DURN is 1024.6
- The cancellation rate is 24.8% 
- The average rating is 3.6
- The total bookings made is 132939
</br>

### Other insights
- The highest revenue of 581.93 was generated in May compared to June and July. May also had the highest occupancy rate and RevPAR of 7.4k
- Weeks 31, 30 and 26, 23 and 21 had the lowest occupancy rates at about 51%. Week 24 had the highest at 62.4%
- Week 27 had the highest revenue at 139.73, while week 26 had the lowest at 114.1%
- The dashboard shows a higher RevPAR, occupancy rate, realisation rate and ADR on weekends than on weekdays
- 61.6% of the revenue generated came from the luxury category compared to 38.4% from the business category
- The realisation rates are close across the seven booking platforms, but bookings via the direct offline and tripster options are the highest. The direct online option is the cheapest
- The Atliq Exotica has the highest guest duration (combined days spent by guests)
- The Atliq Exotica at Mumbai (id 16559) has the highest total bookings at 7251 and the highest revenue at 117m
- The Atliq Palce, Delhi (id 16563) has the highest occupancy rate at 66.3%
- The highest average rating in the properties list is 4.3, shared by 10 properties
- The Atliq City, Bangalore (id 19560) has the highest cancellation rate at 26.5%
</br>
There are several more insights to draw from the dashboard with a lot of filtering options
