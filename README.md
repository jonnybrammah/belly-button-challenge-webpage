# belly-button-challenge-webpage
-----

<p align="center">
<img src="https://cdn-prod.medicalnewstoday.com/content/images/articles/320/320706/image-of-belly-button-why-does-my-belly-button-smell.jpg">
</p>

Image Taken from [Medical News Today](https://www.medicalnewstoday.com/articles/320706).


## Project Description

This project is diving into the surprisingly disgusting world of belly buttons. The goal of this project was to visualize data about the microbes found in the belly buttons of different people in a dataset to show the most common microbes found, as well as the whole range, and the belly button washing frequency.

This data was represented in three different visualizations and deployed to a website which you can find here: https://jonnybrammah.github.io/belly-button-challenge-webpage/. 
The user can select the id of the person of interest from the dropdown menu at the top of the page.

An image of the intialized webpage is also shown below:

<p align="center">
<img src="https://raw.githubusercontent.com/jonnybrammah/belly-button-challenge-webpage/main/Images/initalized_webpage_screenshot.png">
</p>

-----

## Data Extraction

The data was pulled from an [API of belly button information](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.1/14-Interactive-Web-Visualizations/02-Homework/samples.json). This API contained an array of "names" which were actually anonymized ids (like 940). This array of names was used to create the elements in the dropdown menu on the webpage so that the user could select the person they were interested in and the visualizations would change to represent their data.

The API also contained a dictionary for each of these people containing some metadata. Finally, another dictionary contained an array all the microbe ids and labels for each person in the sample. This data was pulled and then stored as different variables in the app.js file.

-----

## Data Visualization

The data was then analyzed and represented in three different ways.

### 1. Bar Chart of Most Common Microbes

A bar chart that shows the most common microbes found in the selected person's belly button was generated with the microbe ID as the y-axis and the number of samples of that microbe found on the x-axis:

<p align="center">
<img src= https://raw.githubusercontent.com/jonnybrammah/belly-button-challenge-webpage/main/Images/initialized_bar_chart.png>
</p>

### 2. Bubble Chart of all Microbes

A bubble chart was then generated to show all the microbes found in the selected person's belly button. In this case, the Microbe ID (which was a number) is plotted on the x-axis and the number of that microbe detected was plotted on the y, as well as being represented by the size of the bubble:

<p align="center">
<img src= https://raw.githubusercontent.com/jonnybrammah/belly-button-challenge-webpage/main/Images/initialized_bubble_plot.png>
</p>

### 3. Gauge Chart of Belly Button Washing Frequencies

A gauge chart was also created to show how often the selected person washes their belly button:

<p align="center">
<img src= https://raw.githubusercontent.com/jonnybrammah/belly-button-challenge-webpage/main/Images/initialized_gauge_chart.png>
</p>

### 4. Metadata

Finally, the metadata for the selected person was written to the website to show more demographic information about them:

<p align="center">
<img src= https://raw.githubusercontent.com/jonnybrammah/belly-button-challenge-webpage/main/Images/initalized_demographic_info.png>
</p>
