# ✈️ Airline Review Visualization Project

## 1. Introduction

The goal of this project is to create an interactive and insightful data visualization exploring **airline survey data** from passengers around the world.  
The visualization helps users understand how various aspects of airline service—such as seat comfort, cabin staff service, and inflight entertainment—affect overall passenger satisfaction.

By integrating interactive elements such as filtering, sorting, aggregation, and multiple views, users can explore patterns, correlations, and temporal trends within the data.


This project applies design principles from *Visualization Analysis & Design (Munzner, 2021)* to build an effective, aesthetically consistent, and user-centered interface.

---


## 2. Data

The data I propose to visualize for my project is the airline review data sourced from 
The dataset combines information from:
- [Airlinequality.com](https://www.airlinequality.com)  
- [Kaggle: Airline Reviews Dataset](https://www.kaggle.com/datasets/juhibhojani/airline-reviews)

Each record represents a customer review and includes:

**Table 1. Airline Review Attributes**
| Attribute | Description |
|------------|--------------|
| **Overall Rating** | Numerical score (0–9) given by the passenger |
| **Seat Comfort** | Comfort level of the seating |
| **Cabin Staff Service** | Quality and friendliness of flight attendants |
| **Food & Beverage** | Quality of meals and drinks provided |
| **Ground Service** | Check-in, boarding, and ground assistance experience |
| **Inflight Entertainment** | Availability and quality of entertainment systems |
| **Wi-Fi/Connectivity** | Quality of onboard internet connection |
| **Value for Money** | Overall perception of price vs. quality |
| **Date of Flight** | When the flight took place |
| **Airline Name** | Airline company being reviewed |

I plan to visualize the overall ratings and accomodation ratings which could be one of the above in table 1. I will utilize the horizontal bar chart and scatter plot to show ratings per airline and make it customizable in that you can show different aggregation types and show by ascending/descending. I can make it more customizable by allowing the user to pick how many airlines they want to show, compare or search individual airlines and show a timeline for a given rating. I plan to incorprate learnings of color, interaction, and more from Visualization Analysis & Design, 2021.

These features enable both **cross-sectional** (airline-to-airline) and **temporal** (over-time) analyses.

---

## 3. Research Questions

The following tasks and questions will drive the visualization and interaction decisions for this project:

1. **How do different flight accomodations influence overall airline ratings?**
2. **Are there measurable correlations between overall rating and specific service attributes?**  
3. **What temporal trends or patterns exist in airline reviews?**  
4. **Do certain time periods (e.g., months or years) correspond to better or worse ratings?**

Each visualization mode contributes to answering one or more of these questions.

---

## 4. Design Overview

### 4.1 Concept
This sketch is the first iteration of my visualization and displays the overall ratings for different airlines across the world. Each customer is asked to rate the airline based on several accomodations 0 to 5 and give an overall rating from 0 to 9. The average of the overall ratings is shown per airline and color coded based on green meaning a more favorable rating through red meaning less favorable ratings. The user interactions possible are picking how many airlines are being shown, how to sort the airlines (ascending or descending), interacting with the X and Y axis (i.e. Y being airlines and X the review category), and being able to pick which what aggregate by like average, mode, min, max, etc. This correlates to the research questions because you will be able to compare how different accomodations affect overall ratings of airlines and identify measureable correlations through the bar chart view and see if any specific dates or periods of time had worse ratings by changing the X axis to time/dates mode.

Users can interact with the visualization through:

- Sorting (ascending, descending, alphabetical)
- Adjusting the number of displayed airlines
- Selecting the aggregation type (mean, median, or mode)
- Searching for specific airlines
- Switching between different accommodation rating types

<img width="1729" height="1092" alt="Airline_ReviewsVis" src="https://github.com/user-attachments/assets/29ce2e11-de69-460b-a65c-dc9f5e5b5508" />

### 4.2 Goals

The following are goals that I had in mind when sketching my initial concept:
- **Comparability** — enable clear comparisons between airlines and accommodation types  
- **Flexibility** — allow user control over sorting, filtering, and aggregation  
- **Readability** — emphasize clean design with intuitive color mapping and spatial awareness 
- **Scalability** — handle multiple airlines without overwhelming the user and allow for additional views/features

---

## 5. Design Evolution and Prototypes

The project evolved through multiple iterations to improve usability, consistency, and insight extraction.

### 5.1 Early Prototype
The first prototype implemented a horizontal bar chart and it shows the average overall ratings of the top X airlines in the world based on customer ratings. I added the ability to sort by ascending, descending, or alphabetically for each rating type, the ability to slide a scale to choose how many airlines will be displayed at once, search, and choose aggregation type. You can also choose between different rating types.

- Basic horizontal bar chart of average ratings  
- Sorting options (ascending/descending)  
- Adjustable number of airlines displayed  
- Moved X-axis to the top for readability  
- Ensured full rating scale (0–9) was always visible  

#### Iteration 1 Prototype:
[![image](https://github.com/user-attachments/assets/bb3419d1-2a74-423e-ad1a-6251aa6f39b4)](https://vizhub.com/Adamisnothere/0950b3c9bc7741f38fa593e3761c2f30)


### 5.2 Iterative Improvements

The following are the aggregated enhancements included from the original prototype up until the major redesign:

- **Aggregation Options** – Users can switch between *mean*, *median*, and *mode*  
- **Comparison Mode** – Allows two airlines to be compared across all rating categories  
- **Time Graph View** – Shows monthly trends in ratings with animation and hover tooltips  
- **Search and Filter** – Enables locating specific airlines quickly  
- **Color Scheme Update** – Red–green diverging scale to represent poor–excellent ratings  
- **Tooltips** – Added full text for truncated airline names


**Click to the images to view/examine iterations:**

#### Iteration 2:
[![image](https://github.com/user-attachments/assets/cda61984-585e-4db7-928a-a3200bf72f25)](https://vizhub.com/Adamisnothere/e12609b86b454b348784607b1eca434e)

#### Iteration 3:
[![image](https://github.com/user-attachments/assets/b3a298be-8272-4146-9e60-a59ade160e1e)](https://vizhub.com/Adamisnothere/8d3a4c20c2f245e9b9ecb03b8c385a68)

#### Iteration 4:
[![image](https://github.com/user-attachments/assets/74d0dd31-21ac-4cef-95f6-18e43172d5a4)](https://vizhub.com/Adamisnothere/3cf27e98ac654b8ebce9116475a24fef)

#### Iteration 5:
This feature adds text to display the exact rating value and airline company if it was cut off.
[![image](https://github.com/user-attachments/assets/d4689dc0-f220-43ce-b273-3b9a763ca3d7)](https://vizhub.com/Adamisnothere/3cf27e98ac654b8ebce9116475a24fef)
<img width="1574" height="722" alt="image" src="https://github.com/user-attachments/assets/99b74730-4003-4e1e-a5fa-b3b02eb096fc" />

This feature shows the comparison mode view allowing you to compare all the rating types of two specific airlines. This view allows you to choose what aggregation type (mean, median, mode) similar to the primary view. Additionally if you hover over a legend item it will highlight that airlines bars in the bar chart. This feature will allow you to take a deeper dive into any two airlines and compare their individual survey results. Note that if an airline does not display a value for a category it means that there is no data.
<img width="1148" height="662" alt="image" src="https://github.com/user-attachments/assets/af8024fe-7dcb-4709-8142-335d851cc052" />

This feature allows you to look at the trend of certain airline ratings over time. This time graph mode allows you to compare all rating types and choose your aggregation method. It is currently for ALL airlines OR for a specific airline and plots month by month. This will allow you to observe any temporal trends in the data. If you hover over any of the data points it will tell you what the date is, the rating, and number of data examples in that data point.
<img width="1235" height="573" alt="image" src="https://github.com/user-attachments/assets/d3da963e-e8d6-4e14-9bee-c026752433fe" />


<img width="1241" height="586" alt="image" src="https://github.com/user-attachments/assets/77cdfdc3-e2f4-4cf5-8b9b-b3b80162778e" />


### 5.3 Major Redesign and Most Recent Changes

A full redesign standardized the **visual identity** of the project.

- **Typography**: Unified to *Inter* font for modern readability  
- **Layout**: Shifted controls to a left-hand panel for cleaner space usage  
- **Card-Based Interface**: Rounded corners, borders, and gradients for modern UI feel  
- **AUC Fill in Time Graphs**: Added shaded areas under curves for trend clarity
- **Animations**: Included is an animation that will draw the data over time
- **Scroll Bars**: Added scroll bars to easily navigate menus when in a lower resolution than required
- **Angled Dates**: Added angled dates to time graph to better read the date for a point
- **Hover Cards**: Updated hover cards to include number of ratings
- **Options**: Added option to select a min and max rating

**(Click image to examine/view visualization.)**
https://vizhub.com/Adamisnothere/509b66cbd6d74cc6a5b8dfbdaec6649f
[![image](https://github.com/user-attachments/assets/71f36bdb-2230-49b8-a559-9e1e80eca3ba)](https://vizhub.com/Adamisnothere/509b66cbd6d74cc6a5b8dfbdaec6649f)

<img width="1906" height="762" alt="image" src="https://github.com/user-attachments/assets/2972b08d-2df0-48b6-9d86-13c65230840c" />

<img width="1905" height="873" alt="image" src="https://github.com/user-attachments/assets/054e132a-12d1-447e-8545-145469d22336" />

<img width="1907" height="799" alt="image" src="https://github.com/user-attachments/assets/41a456e1-06bd-44ca-a2f3-90b08e55c006" />

<img width="1918" height="798" alt="image" src="https://github.com/user-attachments/assets/296139b3-175a-449a-a8e0-bf0e3071862a" />

<img width="1912" height="794" alt="image" src="https://github.com/user-attachments/assets/7b45266e-0e28-4e8e-92c5-251d71ac31ff" />


Scroll Bar:
<img width="1915" height="913" alt="image" src="https://github.com/user-attachments/assets/4ba3be03-c1dd-48d0-bafb-db3329d6ba71" />


Angled Dates:
<img width="1656" height="762" alt="image" src="https://github.com/user-attachments/assets/c5238dd2-537a-4ed6-b1d3-fa91f9e4ce81" />


Number of Ratings:
<img width="1915" height="727" alt="image" src="https://github.com/user-attachments/assets/58021209-bad9-4720-97ec-d19937b68218" />


Options Min/Max Ratings:
<img width="1894" height="689" alt="image" src="https://github.com/user-attachments/assets/d66efded-f380-40a8-b358-8d6ba81abe3d" />



## 6. Visualization Features
Near final features:

**Table 2. Visualization Features**
| Feature | Description | Purpose |
|----------|--------------|----------|
| **Sorting Controls** | Ascending, descending, or alphabetical | Compare airline rankings easily |
| **Aggregation Selector** | Mean, median, or mode | Switch between statistical summaries |
| **Comparison Mode** | Compare two airlines across attributes | Direct side-by-side analysis |
| **Timeline View** | Time-series with hover data | Observe trends over time |
| **Search Function** | Locate airlines instantly | Improve user navigation |
| **Display Controls** | Adjust visible airline count | Prevent visual clutter |

## 7. Iteration Timeline
The following is the timeline of each update (once per week) and the major changes incorporated.

### Week1: 
* Added sorting options by ascending or descending
* Added sliding scale to pick the number of airlines to display at once on the visualization (5 to 30)
* Moved the x axis to the top of the graph (as apposed to the bottom)
* Small edits to positioning of text
* Ensured that the max overall rating value of 9 is always visible even if the max is not as high.

### Week2:
* Added scrolling feature to see cutoff data
* Removed erroneous data at the end of the data file (leftover from previous visualization that wasnt removed)
* Added different aggregation methods and a drop down box to choose (mode, median, average)
* Cleaned up fonts and added a settings area to the top of the visualization
* Added comparison mode for 2 different airlines for all rating types
* Added search bar to search for specific airlines
* Added ability to select which rating type to use

### Week3:
* Cleaned up titles in all modes
* Changed the color range in the primary graph to be diverging from dark reds up to dark greens
* Added feature to highlight the airline if you hover over the legend color in compare mode
* Removed limit on number of airlines shown (up to max now)
* Added feature to sort airlines alphabetically
* Added time graph feature to see trends over time of each rating type for all airlines

### Week4:
* Added loading animation and replay button for the time graph data
* Added grid lines to the time graph for easier viewing
* Added the option to aggregate ALL airlines or choose a specific one in the time graph
* Updated other parts of read me and added more images

### Week5:
* Major redesign of the dashboard for each view
* Standardized font family to inter
* Implemented a card based design for a more modern look with rounded edges, borders, and gradients
* Added a AUC fill to the time graph

### Week6:
* Overhaul and update of the readme

### Week7:
* Added number of ratings to each airlines popup bar
* Added scroll bars to both the options and graph cards
* Corrected display bug due to truncated names of airlines
* Modified time view x-axis to be an angled (Month Year) format
* Added ability to type in airline combo boxes to skip to that letters first airline in the list

---

## 8. Reflections and Open Questions
1. I am not sure how well I will be able to incorporate all the X and Y changes using user interactions. I want to be able to change the Y from airlines (using a bar chart) to specific aggregations of accomodations to be a scatterplot and also be able to pick the aggregation type. This might be a tough task to implement and get right so that the user will be able to use, understand, and extract information from.

**Response 1:** I have decided to scrap the idea of being able to change the Y axis to any other data but each airline and have incorporated multiple views to solve my initial concerns. I had initially wanted to keep everything in one view but split it out into three major view designs which helped to segregate analysis types and steer users to each view for use in analysis of different questions. The first view is to analyze **ALL** airlines (or as many as you choose) and to search for a specific one and have only a given category be present. The second view is to compare all the categories for **TWO** different airlines. The final third view is to be able to analyze temporal data through the use of a scatterplot with the X axis being time and the Y being a review category.

2. One thought is that I am adding too much into this visualiztion and the individual views should be split out into several different visualization projects. On one hand I like that you have the option to look at the data in so many ways but on the other I find that it may be too overwhelming. While the visualization now supports rich interactions and multiple analytical views, there are tradeoffs in complexity. Adding numerous modes (bar, comparison, time-series, scatter) risks overwhelming users without a structured navigation design.

**Response 2:** I think that since I have split the viz into three distinct views its okay that they are all in one visualization because they are separated well enough not to confuse a user too much. It helps that I swapped the check boxes for radio buttons so there is no confusion that more than view can be used at once. Its now easy to swap to a different analysis mode by choosing the view you think is most useful for your analysis question.

**Open considerations:**
- Should these views be split into separate, smaller dashboards?  
- How can transitions between modes be simplified for usability?  
- Would user testing help validate layout and interaction choices?

Despite these challenges, the project effectively showcases how interactive visualizations can reveal nuanced insights about passenger satisfaction and airline performance.

---

## 9. Conclusion

This project demonstrates the end-to-end process of designing, implementing, and refining an interactive data visualization.  
The final visualization enables users to:

- Explore airline performance across multiple service categories  
- Identify relationships between service attributes and overall satisfaction  
- Observe how reviews evolve over time or in response to certain events in time 

The iterative improvements, guided by visualization design principles, resulted in a clean, responsive, and informative visualization tool that bridges data and user insight.

---

## 10. Milestones

Each a week a new addition should be made to the project to enhance, refactor, or iterate upon the reception of the visualization. In other words, there should be a meaningful update each week that shows effort and an improvement of the visualization.

## 11. References

- Munzner, T. (2021). *Visualization Analysis & Design*. CRC Press.  
- [Airlinequality.com](https://www.airlinequality.com)  
- [Kaggle: Airline Reviews Dataset](https://www.kaggle.com/datasets/juhibhojani/airline-reviews)

---


