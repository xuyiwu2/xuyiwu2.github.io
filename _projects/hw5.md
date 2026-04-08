---
layout: project
title: "HW5 Visualization"
date: 2026-04-09
description: "Interactive Vega-Lite visualizations for IS445 HW5."
img: /assets/pngs/hw5_preview.png
tags: [Python, Altair, Vega-Lite, Jekyll]
importance: 1
category: school
---

<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

## Visualization 1: Building Status Distribution

<div id="vis1"></div>

<script>
vegaEmbed('#vis1', '/assets/json/chart1.json');
</script>

This visualization shows the distribution of buildings by their status. The x-axis represents different building status categories, while the y-axis shows the count of buildings in each category. I used color encoding to distinguish between categories, which improves readability and allows easier comparison. The data was aggregated by counting the number of buildings in each category.

---

## Visualization 2: Building Size vs Acquisition Year

<div id="vis2"></div>

<script>
vegaEmbed('#vis2', '/assets/json/chart2.json');
</script>

This visualization explores the relationship between building size and acquisition year. The x-axis represents the year acquired, and the y-axis represents square footage. I implemented an interactive brush selection that allows users to highlight subsets of the data. Additionally, tooltips provide detailed information such as agency name, location, and building size when hovering over points. This enhances user exploration and helps identify patterns over time.

---

## Data

[building_inventory.csv](https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/building_inventory.csv)

## Analysis

[IS445_HW5.ipynb](https://github.com/xuyiw2/is445_HW5/blob/main/IS445_HW5.ipynb)
