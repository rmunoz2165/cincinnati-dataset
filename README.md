# City of Cincinnati Fleet Preventive Maintenance and Repair Work Orders dataset

## OVERVIEW

This is a Tableau final capstone project for an on-line Data Analytics course taken at [General Assembly](https://generalassemb.ly/education/data-analytics/san-francisco). 
The data is a compilation of the City of Cincinnati Fleet Preventive Maintenance and Repair Work Orders, updated daily, with over 270,000+ rows of unique work orders and 37 columns of features from 2008 to present.

## Motivation

I was looking for data that I could use to showcase my Tableau skills while using past experience in maintenance and reliability. The City of Cincinnati's data set was such a treasure to find as I was also able to connect with the Office of Performance and Data Analytics with questions that were very helpful. My main goal was to focus on determining mean-time-between-failures yet there were also plenty of other avenues to explore as discussed below.

## Technical Aspects
<a href="url"><img src="https://github.com/rmunoz2165/cincinnati-dataset/blob/master/images/DownloadData.png" align="right" height="150" width="500" ></a>
**1. Data Download**

Go to the City of Cincinnati Fleet Preventive Maintenance and Repair link [here](https://data.cincinnati-oh.gov/Thriving-Neighborhoods/Fleet-Preventative-Maintenance-Repair-Work-Orders/2a8x-bxjm).
There you'll find a description of the data and a download of the [Data Dictionary](https://data.cincinnati-oh.gov/api/views/2a8x-bxjm/files/d5a81f3e-b274-44c7-8569-458883d0cc5f?download=true&filename=Fleet%20Preventative%20Maintenance%20&%20Repair%20Work%20Orders-%20Data%20Profile%20-%203b.Data%20Dictionary.pdf). The data set is also accessible via 'live' with OData. Click [here](https://support.socrata.com/hc/en-us/articles/115005364207) to obtain information on external source connection via Odata for the Cincinnati Fleet Dataset and [here](https://support.socrata.com/hc/en-us/articles/115011744048-Open-A-Socrata-Dataset-In-Tableau-Desktop) specifically for external connection using Tableau.
</br>
</br>
**2. Tableau users**

You can view my Tableau Public repository for this [project](https://public.tableau.com/profile/robert.d.munoz#!/vizhome/CincinnatiFleetServices/Main?publish=yes). I would be interested in your approach, visualizations and feedback.

</br>
</br>

**3. Dashboards overview:** <a href =  "url"><img src="https://github.com/rmunoz2165/cincinnati-dataset/blob/master/images/FleetTreemap.png"  align="right" height="300" width="500"></a> 
- The [Treemap](https://help.tableau.com/current/pro/desktop/en-gb/buildexamples_treemap.htm) is a relatively simple view that uses dimensions to define the structure of the treemap, and measures to define the size or colour of the  individual rectangles. For this visual, the top 8 Departments are shown in the treemap using sum of 'Total Cost' Feature for both size and color. Other helpful tags shown are ( using Year and Department dropdown filters ): 
     * Average Total cost per vehicle by Department
     * Average Labor Hrs per vehicle by Department
     * Total Cost of Preventive/Repair Work  
     
     </br>
     </br>
     </br>
     </br>
     </br>
         
- The [Pareto Analysis](https://help.tableau.com/current/pro/desktop/enus/pareto.htm#:~:text=Applies%20to%3A%20Tableau%20Desktop%2C%20Tableau,is%20represented%20by%20the%20line.)  <a href =  "url"><img src="https://github.com/rmunoz2165/cincinnati-dataset/blob/master/images/FleetPareto.png"  align="right" height="300" width="500"></a>chart can be used to show where 20% of the fleet vehicles are responsible for 80% of the cost. Good visualization features to explore would be a filter on Vehicle ID to see what part of the curve, above or below 20/80, a particular vehicle is located or add color to distinguish between Departments on the curve.
</br>
</br>
</br>
- A [Sparkline](https://playfairdata.com/how-to-make-sparklines-in-tableau/) chart is meant to present trends and variations associated with some measurement, in a simple and condensed way.  In this visual, we see filtered the top 8 Departments listed by highest Total Cost. In  this example we are using a Table Calculation to display the last or latest measurment for Total Cost distinguished by the unique 'sun' shape. Hover will show a breakdown per Quarter.<a href =  "url"><img src="https://github.com/rmunoz2165/cincinnati-dataset/blob/master/images/FleetSparklines.png" align="right" height="300" width="500"></a>
