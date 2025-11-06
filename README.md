# Data Visualization Project

## Data

The data I propose to visualize for my project is the airline review data sourced from airlinequality.com and https://www.kaggle.com/datasets/juhibhojani/airline-reviews. I plan to visualize the overall ratings or the accomodation ratings which could be one of seat comfort, cabin staff service, food & beverage, ground service, inflight entertainment, wifi/connectibity and value for money. I would like to utilize the horizontal bar chart to show these ratings per airline and make it customizable in that you can show different statistics like average, mode, etc and show by ascending or descending. I can make it more customizable by allowing the user to pick how many instances they want to show, compare or search individual airlines and show a timeline for a given rating. I plan to incorprate learnings of color, interation, and more from Visualization Analysis & Design, 2021.


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * How do the different types of flight accomodations affect the overall rating?
 * Is there any correlation between X and Y? Where X could be the overall rating and Y could be one of the accomodations.
 * Are there interesting temporal patterns in X?
 * Are any dates flown correlate with worse overall_ratings?

## Sketches
This sketch represents the overall ratings for different airlines across the world. Each customer is asked to rate the airline based on several accomodations and give an overall rating from 0 to 9. The average of the overall ratings is shown per airline and color coded based on green meaning higher rating down to red meaning lower ratings. The interactions will be being able to pick how many airlines are being shown, how to sort the airlines (ascending or descending), what the Y axis will be (i.e. Y being airlines or one of the accomdations to make other judgements, and being able to pick which statics to aggregate by like average, mode, min, max, etc. This relates to the questions because you will be able to compare how different accomodations affect overall ratings of airlines with X and Y changes, pick different Y values to see if a certain accomodation affects the overall rating more, use the aggregation mode to see spatial patterns in X, and see if any specific dates had worse ratings by using that mode.
<img width="1729" height="1092" alt="Airline_ReviewsVis" src="https://github.com/user-attachments/assets/29ce2e11-de69-460b-a65c-dc9f5e5b5508" />


## Prototypes

I’ve created a proof of concept visualization of this data. It's a horizontal bar chart and it shows the average overall ratings of the top X airlines in the world based on customer ratings. I have added the ability to sort by ascending, descending, or alphabetically for each rating type, the ability to slide a scale to choose how many airlines will be displayed at once, search, and choose aggregation type. You can also choose between different rating types.

### Major Redesign
A major redesign has taken place for the viz. I have standardized colors, fonts (inter family), add a more modern card layout with rounded edges and moved the options to a left hand layout instead of at the top.

[![image](https://github.com/user-attachments/assets/71f36bdb-2230-49b8-a559-9e1e80eca3ba)](https://vizhub.com/Adamisnothere/3cf27e98ac654b8ebce9116475a24fef)
(CLICK TO VIEW VIZ)

Old:
<img width="1639" height="617" alt="image" src="https://github.com/user-attachments/assets/d4689dc0-f220-43ce-b273-3b9a763ca3d7" />
New:
<img width="1906" height="762" alt="image" src="https://github.com/user-attachments/assets/2972b08d-2df0-48b6-9d86-13c65230840c" />

This is a new feature that will display the exact rating value and airline company if it was cut off.
<img width="1574" height="722" alt="image" src="https://github.com/user-attachments/assets/99b74730-4003-4e1e-a5fa-b3b02eb096fc" />

This shows the comparison feature allowing you to compare all the rating types of two specific airlines. This view allows you to choose what aggregation type (mean, median, mode). 
<img width="1148" height="662" alt="image" src="https://github.com/user-attachments/assets/af8024fe-7dcb-4709-8142-335d851cc052" />

Another new feature allows you to look a the trend of certain ratings over time. This time graph mode allows you to compare all rating types and choose your aggregation method. It is currently for ALL airlines for a specific airline. It plots month by month and if you hover over a specific circle it will show you number of reviews and date. Included is an animation that will draw the data over time. This will allow you to observe any temporal trends in the data. If you hover over any of the data points it will tell you what the date is, the rating, and number of data examples in that data point.
<img width="1235" height="573" alt="image" src="https://github.com/user-attachments/assets/d3da963e-e8d6-4e14-9bee-c026752433fe" />

<img width="1241" height="586" alt="image" src="https://github.com/user-attachments/assets/77cdfdc3-e2f4-4cf5-8b9b-b3b80162778e" />



## Open Questions
I am not sure how well I will be able to incorporate all the X and Y changes using user interactions. I want to be able to change the Y from airlines (using a bar chart) to specific aggregations of accomodations to be a scatterplot and also be able to pick the aggregation type. This might be a tough task to implement and get right so that the user will be able to use, understand, and extract information from.

One thought is that I am adding too much into this visualiztion and the individual views should be split out into several different visualization projects. On one hand I like that you have the option to look at the data in so many ways but on the other I find that it may be too overwhelming

## Milestones

Each a week a new addition should be made to the project to enhance, refactor, or iterate upon the reception of the visualization. In other words, there should be a meaningful update each week that shows effort and an improvement of the visualization.

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
* 
