---
name: Don't Drink and Study? Alcohol Consumption and Grades for Students in Portugal 
tools: [Python, Altair]
image: assets/pngs/finalProject.png
description: IS 445 Final Project
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# Don't Drink and Study? Alcohol Consumption and Grades for Students in Portugal 
*Author: Lara Terpetschnig*

## The Data
### Student Outcomes 
The primary dataset is sourced from a study of machine learning methods to predict student grades: ["Using data mining to predict secondary school student performance"](https://www.researchgate.net/publication/228780408_Using_data_mining_to_predict_secondary_school_student_performance) and contains information about students in two public high schools and their grades for each trimester of their in math and Portuguese classes. The data was collected during the 2005 - 2006 school year from school records and a survey distributed to the students. 

### European Health Interview Survey 
The secondary dataset is sourced from the European Health Interview Survey. The survey has been distributed three times, starting with the first wave which took place from 2006 - 2009. Unfortunately, Portugal was not one of the 17 EU states who participated. However, in 2013 onwards, EU members were required to participate. Data from Portugal exists for 2014 (second wave) and 2019 (third wave). 

## Visualizations 
I used the [hex codes for the Portugal flag](https://www.flagcolorcodes.com/portugal): #046A38 (green) and #DA291C (red) to color some of the visualizations. 

### Grades and Drinking in Portugal 
<div class="alert alert-info" role="alert">
  <i class="fas fa-info-circle"></i> This chart is interactive! Click on the squares in the heatmap to update the histogram.
</div>
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_project_interactive_heatmap.json" style="width: 100%"></vegachart>

This plot contains a linked heatmap and histogram. By clicking one of the cells in the heatmap, you can see the final grade distribution for students based on the combination of their weekday and weekend drinking levels, which range from 1 to 5 (1 being "very low" and 5 being "very high"). In Portugal, as in many European countries, students are graded on a 20 point scale. 

The worst outcome occurs with a weekend drinking level of 2 and a weekday drinking level of 4; however, the histogram reveals that this is just one student. Similarly, the best outcome that occurs with a weekday drinking level of 3 and a weekend drinking level of 1 is also one student. 

Most of the data is clustered around very low weekday and weekend drinking levels, but it's worth noting that this data suffers from response bias: students may not want to reveal a high level of drinking during the weekdays and/or weekend and may have chosen smaller numbers as a result. 

From this dataset, it's not clear if student outcomes are affected by drinking at these particular schools. 

### Changes in Drinking Habits 
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_project_grouped_bars.json" style="width: 100%"></vegachart>

This chart shows the frequency of alcohol consumption for Portuguese citizens aged 15 to 24 in 2014 and 2019. There is a slight increase in drinking "every day" and "every week" but an even greater increase in drinking "never" from 2014 to 2019, suggesting that more young people in Portugal are moving towards abstinence. 

This data could be compared with standardized testing outcomes to see if there is any correlation. 

### Comparison with Other EU Countries 
<div class="alert alert-info" role="alert">
  <i class="fas fa-info-circle"></i> This chart is interactive! Click on the legend to reorder the bars. The previously clicked selections will move to the end. 
</div>
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_project_stacked_bars.json" style="width: 100%"></vegachart>

This chart shows the frequency of alcohol consumption for the top five countries in the European Union (by population) and Portugal. The chart contains data from 2019 for citizens aged 15 to 19, which is typically the duration of high school in Europe. The bars can be rearranged by clicking on the legend for easier comparison. 

Compared to other countries, Portugal does not have as many students drinking "every day" and "every week". Standardized tests scores could be compared between countries to see if differences occur based on alcohol consumption. 

## Citations 
Cortez, Paulo & Silva, Alice. (2008). Using data mining to predict secondary school student performance. EUROSIS. 

European Commission, Eurostat, Reference Metadata in Euro SDMX Metadata Structure (ESMS), Publication Office of the European Union, https://ec.europa.eu/eurostat/cache/metadata/en/hlth_det_esms.htm#

<div class="left">
{% include elements/button.html link="https://archive.ics.uci.edu/dataset/320/student+performance" text="The Data: Student Performance" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/LaraTerpetschnig/LaraTerpetschnig.github.io/blob/main/python_notebooks/final_project_3.1.ipynb" text="The Analysis" %}
</div>

<div class="left">
{% include elements/button.html link="https://ec.europa.eu/eurostat/databrowser/view/hlth_ehis_al1c/default/table?lang=en" text="The Data: European Health Interview Survey" %}
</div>


