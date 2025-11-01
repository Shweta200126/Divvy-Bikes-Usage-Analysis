# Divvy Bikes Usage Analysis using Tableau</p>

## Project Background

Divvy is a bike-sharing system in Chicago, owned by the [Chicago Department of Transportation](http://www.cityofchicago.org/city/en/depts/cdot.html) (CDOT). It was launched on June 28, 2013, and later expanded north to Evanston on June 27, 2016. Since 2019, Divvy has been operated by [Lyft](https://www.lyft.com/). Divvy is North America’s largest bike-share system by service area. Divvy is considered one of the primary bike-share system in Chicago,  with over 400,000 new riders and 5.5 million rides taken in 2021.  Divvy has two primary group users, which are annual membership riders and casual riders. One of Divvy’s goals is to increase the number of annual membership riders. This project will focus on in-depth analysis of Divvy’s rider behavior and how external factors impact its ridership.

Divvy as of September 2024 has 1,014 stations in total.

## Business Goal

This project analyzes over 100,000 trips from 2019 to understand the different usage patterns of Divvy's two main customer types: "Members" (annual subscribers) and "Casual" riders.

The primary goal was to identify data-driven product and pricing opportunities to increase revenue from casual riders and support the business goal of converting them into members.

### Tableau Link - 
   [Who are the riders?](https://public.tableau.com/app/profile/shweta.anand/viz/2_3_side_by_side_17291356619870/Whoaretheriders)

   [Top Stations](https://public.tableau.com/app/profile/shweta.anand/viz/TopStations_17271951081330/TopStationsDashboard)
<br>

## Data

The data provided contains information on each trip taken on a Divvy bike in 2019, including the trip start and end time, the starting and ending station, and the rider demographics. The data has been pre-processed to exclude trips without a start or end date.

## Key Insights & Actionable Recommendations

My analysis uncovered two distinct user profiles with unique needs, leading to two key business recommendations:

### 1. Recommendation: Launch a _$15 Day Pass_ for Casual Riders

**The Insight:** Casual riders are not commuters. My analysis showed they are primarily leisure users who ride on weekends (peaking at 2 PM) and take very long trips (average 50+ minutes) clustered around tourist spots and the waterfront.

**The Problem:** The existing per-minute pricing creates anxiety and a poor user experience for these leisure riders, likely causing many potential customers to abandon the service.

**The Solution:** I proposed a new $15 Day Pass. This simple, flat-fee product aligns perfectly with their leisure behavior, reduces friction, and creates a clear "upsell" path. I projected this new product could boost revenue from this segment by 10%.

### 2. Recommendation: Optimize Bike Rebalancing Operations

**The Insight:** My temporal analysis identified Thursday at 5 PM as the absolute peak time for _Member_ (commuter) riders, with a massive flow of bikes from business districts to residential hubs.

**The Problem:** Without a plan, this creates a bike shortage at business stations during the 5 PM rush, leading to lost rides and frustrated members.

**The Solution:** I recommended a dynamic rebalancing strategy for the operations team, specifically to restock high-demand business district stations (like "Canal St & Adams St") just before the 4:30-5:00 PM peak.

## Visualizations & Dashboards

I built a series of interactive Tableau dashboards to find and present these insights:

**Cohort Analysis Dashboard:** A side-by-side comparison of _Member_ vs. _Casual_ riders, showing their different trip durations, day-of-week preferences, and peak times.

**Geospatial Heatmap:** A map dashboard visualizing that casual trips originate from tourist hubs, while member trips follow clear commute corridors.

**Temporal _Peak Times_ Dashboard:** A line chart identifying the precise _commuter rush_ (Thursday 5 PM) and the _leisure peak_ (Saturday 2 PM).

## Tools Used

**SQL:** Used to query, clean, and join over 100,000 trip records with station and weather data.

**Tableau:** Used for all data visualization, cohort segmentation, and dashboard creation.

## Datasets used in the project
- Trip data from the Divvy: https://divvy-tripdata.s3.amazonaws.com/index.html
-	Station data from Chicago Data Portal: https://data.cityofchicago.org/Transportation/Divvy-Bicycle-Stations/bbyy-e7gq/data
-	Weather data from National Weather Service: https://www.weather.gov/wrh/climate?wfo=lot
-	Population data from Chicago Data Portal: https://data.cityofchicago.org/Health-Human-Services/Chicago-Population-Counts/85cm-7uqa


## Conclusion

By using Tableau to analyze the Divvy bike trip data, we can gain valuable insights into how bikes are being used in Chicago. This information can be useful in planning future bike infrastructure and promoting sustainable transportation options. The interactive dashboards created will allow users to easily explore the data and uncover patterns and trends in bike usage.
