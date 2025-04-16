---
layout: default
permalink: /
title: UFO Sightings Visualization
---
## UFO Sightings Visualizations

### Bar Chart: Sightings by Shape
<vegachart schema-url="{{ site.baseurl  }}/assets/json/shape_bar.json" style="width: 100%" />
This bar chart shows the number of reported UFO sightings by the shape of each object. Each bar shows a unique shape. For example, 'light' being the most common means that an unusual light was seen in the sky. The bar height shows how many of these objects are in the dataset. I used a bar chart to show the differences by shape. The x axis encodes the shape, and the y axis shows the count. I used a categorical color scheme to distinguish the bars. I dropped missing data for shapes and time, and used value_counts in pandas to get the frequency before accessing them with Altair.

### Line Chart: Sightings Over Time by Shape
<vegachart schema-url="{{ site.baseurl  }}/assets/json/time_chart.json" style="width: 100%" />
This is my interactive line chart, which shows how UFO sightings varied over time for each shape. I added a dropdown for interactivity, and it allows you to select what shape you would like to see the chart for. I plotted it by month for simplicity's sake. Time is on the x axis and the frequency is on the y axis. I grouped the data using pandas and used alt.param() in altair to bind the dropdown menu to a filter.

---

### Resources
[The Data](https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/ufo-scrubbed-geocoded-time-standardized-00.csv)
[The Analysis](https://github.com/jamesjs4/jamesjs4.github.io/blob/main/python_notebooks/Workbook.ipynb)


{% include landing.html %}