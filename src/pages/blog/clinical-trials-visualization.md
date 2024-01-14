
<div align="center">
  <h1>Clinical Trials Visualization (Proprietary)</h1>
</div>

## Tools and Concepts Applied
1. R
2. Tidyverse packages - dplyr, ggplot
3. Descriptive Visualization

## Introduction

My team at Edwards Lifesciences had just completed a series of clinical studies and wanted to better understand our new device’s efficacy for treating patients with various etiologies of mitral and tricuspid regurgitation. 


## Data

I was given 3 separate data sets from Early Human Use clinical studies. 

There were ~20 patients the datasets, each with ~100 features. Features included physiological measurements, ID#’s, and timestamps. The rows represented different patients (each patient had a unique ID#) and the columns represented features that were both continuous and categorical in nature.


## Data Processing

Data Transformation:
The 3 data sets were merged by unique patient ID’s. New features were engineered from preexisting features. For example, durations were calculated with timestamps and reduction in regurgitation was calculated with pre/post procedure measurements. Patients were also placed into “procedural success groups”, which were assigned based off a combination of features including: reduction in regurgitation and duration of procedure.

Data Reduction: 
Patients that did not undergo a complete procedure were removed. 


## Visual Creation 
Six descriptive visuals including basic bar charts, stacked bar charts and grouped bar charts were created.

Chart elements such as color, axes, titles, areas, gridlines, and legends were customized to fit specifications.


## Results
Six descriptive visuals including basic bar charts, stacked bar charts and grouped bar charts were created.

Chart elements such as color, axes, titles, areas, gridlines, and legends were customized to fit specifications.

