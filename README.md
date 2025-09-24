# Data Visualization Project

## Data

The data I propose to visualize for my project is the airline review data sourced from airlinequality.com and https://www.kaggle.com/datasets/juhibhojani/airline-reviews. I plan to visualize the overall ratings or the accomodation ratings which could be one of seat comfort, cabin staff service, food & bev, ground service, inflight entertainment, wifi/connectibity and value for money. I would like to utilize the horizontal bar chart to show these ratings per airline and make it customizable in that you can show different statistics like average, mode, etc and show by ascending or descending. I can make it more customizable by allowing the user to pick how many instances they want to show.


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * How does the different types of flight accomodations affect the overall rating of the airline?
 * Is there any correlation between X and Y? Where X could be the overall rating and Y could be one of the accomodations.
 * Are there interesting spatial patterns in X?
 * Are any dates flown correlate with worse overall_ratings?

## Sketches
(describe each sketch - how is the data visualized, what are the interactions, and how do these relate to the questions/tasks)
This sketch represents the overall ratings for different airlines across the world. Each customer is asked to rate the airline based on several accomodations and give an overall rating from 0 to 9. The average of the overall ratings is shown per airline and color coded based on green meaning higher rating down to red meaning lower ratings. The interactins will be being able to pick how many airlines are being shown, how to sort the airlines (ascending or descending), what the Y axis will be (i.e. Y being airlines or one of the accomdations to make other judgements, and being able to pick which statics to aggregate by like average, mode, min, max, etc. This relates to the questions because you will be able to compare how different accomodations affect overall ratings of airlines with X and Y changes, pick different Y values to see if a certain accomodation affects the overall rating more, use the aggregation mode to see spatial patterns in X, and see if any specific dates had worse ratings by using that mode.
<img width="1729" height="1092" alt="Airline_ReviewsVis" src="https://github.com/user-attachments/assets/29ce2e11-de69-460b-a65c-dc9f5e5b5508" />


## Prototypes

I’ve created a proof of concept visualization of this data. It's a horizontal bar chart and it shows the average overall ratings of the top 10 to 20 airlines in the world based on customer ratings.
[![image](https://github.com/user-attachments/assets/bb3419d1-2a74-423e-ad1a-6251aa6f39b4)](https://vizhub.com/Adamisnothere/0950b3c9bc7741f38fa593e3761c2f30)

## Open Questions

(describe any fear, uncertainty, or doubt you’re having about the feasibility of implementing the sketched system. For example, “I’m not sure where to get the geographic shapes to build a map from this data” or “I don’t know how to resolve the codes to meaningful names” … Feel free to delete this section if you’re confident.)

## Milestones

(for each week, estimate what would be accomplised)
