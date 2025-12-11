---
name: Final Project Part 3.1
tools: [Python, Altair, vega-lite]
image: assets/pngs/final_project.png
description: IS 445 Final Project
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# Alcohol Consumption and Grades Among Students in Portugal 
*Author: Lara Terpetschnig*

<vegachart schema-url="{{ site.baseurl }}/assets/json/final_project_interactive_heatmap.json" style="width: 100%"></vegachart>

This plot contains a linked heatmap and histogram. By clicking one of the cells in the heatmap, you can see the final grade distribution for students based on the combination of their mother and father's job. The job of a student's parents can be considered a proxy for income. Significant difference between student outcomes can be observed based on parents' occupation. However, confounders (variables that hide the true relationship between income and grades) such as teachers being better equipped to help their children succeed at school, should be noted. Another possible confounder is alcohol consumption. 

Chart 2 from contextual dataset:
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_project_grouped_bars.json" style="width: 100%"></vegachart>

This chart shows the frequency in alcohol consumption for Portuguese citizens aged 15 to 24 in 2014 and 2019. This data is sourced from The European Health Interview Survey. A link to the dataset can be found [here](https://ec.europa.eu/eurostat/databrowser/view/hlth_ehis_al1c/default/table?lang=en). The increase in high school and college-aged citizens drinking "every day" and "every week" can be compared with standardized testing outcomes to see if there is any correlation. 

Chart 3 from contextual dataset and interactive:
<vegachart schema-url="{{ site.baseurl }}/assets/json/final_project_stacked_bars.json" style="width: 100%"></vegachart>

This chart shows the frequency of alcohol consumption for the top five countries in the European Union (by population) and Portugal. This data is sourced from The European Health Interview Survey. A link to the dataset can be found [here](https://ec.europa.eu/eurostat/databrowser/view/hlth_ehis_al1c/default/table?lang=en). The data covers 2019 only, and focused on citizens aged 15 to 19, which is typically the duration of high school in Europe. Compared to other countries, Portugal does not have as many students drinking "every day" and "every week". Standardized tests scores could be compared between countries to see if differences occur based on alcohol consumption. 

<div class="right">
{% include elements/button.html link="https://github.com/LaraTerpetschnig/LaraTerpetschnig.github.io/blob/main/python_notebooks/final_project_3.1.ipynb" text="The Analysis" %}
</div>


