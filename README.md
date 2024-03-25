# Zomato-Resturant-Analysis-Using-Power-BI


Data Manipulation and Reporting with Power BI
Certification Project 












 

Contents
High Level Business Requirement .......................................................................................................3

Files Required for Project ....................................................................................................................3

High Level Steps ...................................................................................................................................4

Data Import ..........................................................................................................................................4

Data Transformations ...........................................................................................................................4

Data Modeling......................................................................................................................................4

Other Data Manipulations ....................................................................................................................5

Using DAX .............................................................................................................................................5

Data Visualization..................................................................................................................................6

What to Submit .....................................................................................................................................7

Result Check...........................................................................................................................................7






















High Level Business Requirement
Zomato is a restaurant search and discovery service. Operating in several countries worldwide, they provide detailed information and customer reviews of various restaurants. The owners of Zomato, want to unearth
the hidden anomalies in their business data. The final objective is to analyze the data in a way which helps them to accurately judge their business performance.

The data (sample) is currently available  in the form of a few excel files with each file containing information about several restaurants operating in a specific continent. The clients want to create a consolidated and interactive PowerBI report from where they can easily analyze the following information:

1)    Total number of restaurants across continents, countries and cities.


2)    The ability to view information at a global level. But at the same time, the ability to go down to a granular level as well.

3)    Top performing restaurants by average customer ratings.


4)    Top performing restaurants by least average cost.


5)    Ability to filter and view the restaurant details (address, cuisines served …) on the basis of:
a. Geographic dimensions like continent, country and city.
b.  If the restaurant offers services like, online delivery or table booking. 
c.   Rating colors denoting the average rating slab.

6)    Top ranking restaurants by the number of cuisines they serve.


7)    They want to create a multi-page report which matches with the company’s theme and
where navigation between pages has been made very easy.


8)    They want their users to be able to access this report using a web browser as well as their phone devices.







High Level Steps
To achieve the above-mentioned requirements, following are some of the high-level steps that need to be performed.

Data Import
1)    Import data from all the available Excel files (mentioned below) into PowerBI.
a.	Africa
b.	Asia
c.	Country-Code 
d.	Europe
e.	NAM
f.	SAM
g.	Oceania
h.	Fact Table

Data Transformations
1)    Some of the values in the “City” column, mentioned below, needs to be corrected.
a.    The word “city” needs to be taken off from every city name (wherever appears). b.    “Sí£o Paulo” should be corrected to “São Paulo”.
c.    “Cedar Rapids/Iowa City” should be corrected to “Cedar Rapids”.
d.    “ÛÁstanbul” should be corrected to “Istanbul”.


2)    Remove the columns which are not used.


3)    Make separate columns to show the “Restaurant Name” and the “Restaurant Address”.


4)    Create a separate table from where you get the list of cuisines served by each restaurant.


5)    The “Country-Code” table must contain only unique and non-blank values (as it’s a
dimension table).

Data Modeling
1)    Model your data according to the reporting requirements.


2)    While creating relationships, choose the appropriate “Cardinality” and the “Cross filter direction”
so that the aggregations can happen accurately at the report level.




Other Data Manipulations
1)    There is a list of geographic columns. Go through the list and categorize them appropriately.


2)    Create a user-defined hierarchy and include all the geographical dimensions in there.


3)    Group the countries into appropriate continents.

Using DAX
1)    There needs to be a “Rating Color” column in an appropriate table. The data rows should follow the below mentioned convention.

Aggregate rating                 Rating color
Above 4.5                             Dark Green
4 to 4.4                                 Green
3.5 to 3.9                              Yellow
2.5 to 3.4                              Orange
1.8 to 2.4                              Red
0 to 1.7                                 White


2)    Create following measures in appropriate tables. a.	Restaurant Count
b.   Average Cost
c.  Average Rating 
d.   Cuisine Count

3)    Create a new column called “Continent” in the “Country Code” table. Create the values using the below mentioned convention.
Note: The Country and Continent mapping is as follows. Please use this convention wherever needed.
a.    Africa – South Africa b.    Asia – Philippines
c.    Asia – Singapore d.    Asia – UAE
e.    Asia – India
f.     Asia – Indonesia g.    Asia – Qatar
h.    Asia – Sri Lanka i.     Asia – Turkey
j.  Europe – United Kingdom
k.  North America – United States l.     North America – Canada
m.   Oceania – Australia
n.    Oceania – New Zealand o.    South America – Brazil


4)    Wherever needed, lookup the continent column from the “Country Code” table.


Data Visualization
1)    Create the following visuals.
a)	Card visual
i.    Average Cost
ii.   Average Rating
iii.    Restaurant Count
b)    Map visual
i.    Geography  hierarchy
ii.   Restaurant Count
c)    Infographic designer
i.    Restaurant Name
ii.   Top 5 Restaurants by Average Cost
iii.    Average Rating
d) Slicer showing list of rating colours
e)    Slicer showing list of counties
f)     Slicer showing list of cities
g)    Grid showing list of restaurants
h)    Gauge showing selected restaurant’s average rating
i)     Gauge showing selected restaurant’s average cost
j)     Card showing the selected restaurant’s address
k)    Grid showing the selected restaurant’s list of cuisines
l)     Publish the report on to a service account and create a public link.









Note: The web view you created should resemble the report that can be accessed using the link below.
https://app.powerbi.com/view?r=eyJrIjoiZDU0YzIwNWUtZGU0NS00MGJkLThmNDktNjVmMzJkMzNiY2NmIiwidCI6ImZlYmNlODJhLTViNmEtNDc0NS05NmU3LTA1MDg3ZjUyZmQyZCJ9


2)    Make sure you also create a mobile view for the report that matches the screenshots shown below.

 

What to Submit
The following deliverables are expected at the end of the project.

1)    The .pbix file.
2)    A public URL using which the report can be viewed in a web browser.
3)    Screenshots of the mobile view (as many as possible to show different views of mobile device).

Result Check
The submitted projects would be considered as a successful one, only if it satisfies the following points.

1)    All the required files should be imported.
2)    All the required data transformations should be applied.
3)    All the required objects (measures, hierarchies and groups) should be created.
4)    The data modeling should be as per the reporting requirements.
5)    As per the public URL provided,
a.    All the visuals should be created.
b.    All the interaction points should be implemented (nested slicers, slicer to visual, visual as filter etc.).
c.    Navigation menu needs to be created. d.    All the values must match.
6)    A web as well as a mobile view must be created.

