# Data Visualization Project

## Data

The data I propose to visualize for my project is the airline review data sourced from airlinequality.com and https://www.kaggle.com/datasets/juhibhojani/airline-reviews. I plan to visualize the overall ratings or the accomodation ratings which could be one of seat comfort, cabin staff service, food & bev, ground service, inflight entertainment, wifi/connectibity and value for money. I would like to utilize the horizontal bar chart to show these ratings per airline and make it customizable in that you can show different statistics like average, mode, etc and show by ascending or descending. I can make it more customizable by allowing the user to pick how many instances they want to show.


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * How does the different types of flight accomodations affect the overall rating?
 * Is there any correlation between X and Y? Where X could be the overall rating and Y could be one of the accomodations.
 * Are there interesting spatial patterns in X?
 * Are any dates flown correlate with worse overall_ratings?

## Sketches
This sketch represents the overall ratings for different airlines across the world. Each customer is asked to rate the airline based on several accomodations and give an overall rating from 0 to 9. The average of the overall ratings is shown per airline and color coded based on green meaning higher rating down to red meaning lower ratings. The interactions will be being able to pick how many airlines are being shown, how to sort the airlines (ascending or descending), what the Y axis will be (i.e. Y being airlines or one of the accomdations to make other judgements, and being able to pick which statics to aggregate by like average, mode, min, max, etc. This relates to the questions because you will be able to compare how different accomodations affect overall ratings of airlines with X and Y changes, pick different Y values to see if a certain accomodation affects the overall rating more, use the aggregation mode to see spatial patterns in X, and see if any specific dates had worse ratings by using that mode.
<img width="1729" height="1092" alt="Airline_ReviewsVis" src="https://github.com/user-attachments/assets/29ce2e11-de69-460b-a65c-dc9f5e5b5508" />


## Prototypes

I’ve created a proof of concept visualization of this data. It's a horizontal bar chart and it shows the average overall ratings of the top X airlines in the world based on customer ratings. I have added the ability to sort by ascending or descending overall rating and the ability to slide a scale to choose how many airlines will be displayed at once.
[![image](https://github.com/user-attachments/assets/bb3419d1-2a74-423e-ad1a-6251aa6f39b4)](https://vizhub.com/Adamisnothere/22d28792bbd74cd98bb74ecbf01a36a7)

## Open Questions
I am not sure how well I will be able to incorporate all the X and Y changes using user interactions. I want to be able to change the Y from airlines (using a bar chart) to specific aggregations of accomodations to be a scatterplot and also be able to pick the aggregation type. This might be a tough task to implement and get right so that the user will be able to use, understand, and extract information from.

## Milestones

Each a week a new addition should be made to the project to enhance, refactor, or iterate upon the reception of the visualization. In other words, there should be a meaningful update each week that shows effort and an improvement of the visualization.
Week1: Added sorting options, added sliding scale to pick the number of airlines to display at once on the visualization, moved the x axis to the top of the graph (as apposed to the bottom), small edits to positioning of text
