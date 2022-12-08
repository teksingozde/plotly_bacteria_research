# Plotly Bacteria Research
## Overview of Project
The customer wants the data file containing the information about the volunteers and the results of the biological analyzes obtained from the samples taken from the volunteers' stomachs to be created as a dashboard and transferred to the website. This website will contain the predetermined identification number of the volunteers, demographic information and sample results. In the Dashboard, the test results start from IDs 940 and continue until 1601. In between, the presence of lost data can also be observed. When ID is selected in the Dashboard, the demographic information of the volunteer is in the purple box with the demographic info gauge in the upper left, the top 10 bacteria cultures in the belly of the volunteer in the bar chart, all the bacterial species in the belly of the bubble chart, and a graph showing the frequency of navel washing during the week of the volunteer. The web page was first prepared in the index.html file and the dashboard title color etc was formatted in the CSS file. The related graphics and display were created in Javascript file and demographic information was created in JSON format and saved as "samples.json".

## Resources
### Software:
- HTML,
- CSS, 
- Javascript.

### Dataset: 
- samples.json

### Other Resources: 
- index.html

## Creating Web Page 

The Javascript file is the file that has the most impact on the creation of the dashboard. Because without the javascript file, there is only the dashboard title and the demographic ID filter in the upper left.
The javascript file provides a structure for the initial configuration of the dashboard. This structure selects the sample from the JSON file and then iterates each value according to the IDs of these samples. The page where the Dashboard is located is completely live and the graphics and display change according to the selected sample values.
The HTML file acts as a clipboard for users. CSS file is used for formatting this board.
Javascript commands are called in the body of the HTML. The important point to note is that the syntax of each graph should be written sequentially and separated as items.
The general website is formatted with CSS, and its color can be edited if desired.

## Results

The general access link to the created page is https://teksingozde.github.io/plotly_bacteria_research/ . In general, when the link is clicked, the page will look like the one below.

![full_page_website](https://user-images.githubusercontent.com/26927158/206582396-86522c39-4f6b-4613-98a8-9a68fabb7eed.png)

#### Table 1. Dashboard Head
<img width="842" alt="head" src="https://user-images.githubusercontent.com/26927158/206582587-f89d29bc-7ef9-453d-a8c8-aa2d20dcae71.png">
The header part seen in the table above is created from the html file. While the color of the title is decided through the CSS file, all the information is in the body part of the "index.html" file.

#### Table 2. Demographic Information
![filter](https://user-images.githubusercontent.com/26927158/206582777-14899b1c-ade5-46a1-bf0e-4b8d9a5d1d84.png)

The demographic ID part of the volunteers can be seen in this way. In the ID section, there is information about the ethnicity, gender, age, location, bbtype and wfreq of the volunteers.
Each time the ID number is changed, the information of the volunteer will change live.

#### Chart 1. Bar Chart
<img width="470" alt="bar_chart" src="https://user-images.githubusercontent.com/26927158/206582931-1094ea58-3918-4ad3-b925-a077b7daef81.png">
Bacteria ranking in the top 10 in the bacteria ranking analyzed from the sample taken from the navel of the person with the ID number 940 is shown in the graphic above. The information in this table also changes according to the sample taken from each volunteer.

#### Chart 2. Bubble Chart
<img width="1173" alt="bubble_chart" src="https://user-images.githubusercontent.com/26927158/206583031-44c997cd-74ee-4869-a23d-983cd49343bb.png">
On the bubble chart, it is seen that the bacteria in the volunteer with the ID number 940 and the bubble growing according to their volume.
Each bubble defines different bacteria among itself and their volumes change according to the bacterial value.

#### Chart 3. Gauge Chart
<img width="466" alt="gauge_chart" src="https://user-images.githubusercontent.com/26927158/206583111-e8c6368c-47a1-4de6-8fd6-52bd5c890de4.png">
The gauge chart shows the weekly belly button washing frequency. According to the IDs, the weekly washing frequency of course changes. If it is specified for the ID number 940, it is clearly seen that the weekly belly button washing frequency is 2.

## Summary 

On the website, it is seen that the ID number of the first volunteer is 940 and their demographic information is included in the relevant chart. When the user wants to select the ID of a different volunteer, he can see the information of the desired ID by clicking on the menu.
The user can also use the bubble chart to learn the OTU bacteria of each ID and their excess or value. In addition, different analyzes can be made according to the top 10 bacteria in each volunteer.














