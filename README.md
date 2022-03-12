# Where-Will-Big-Foot-Appear-Next

## Introduction:


One of the great North American mysteries that still capture the hearts and minds of tourists and enthusiasts alike is the tale of the elusive bigfoot. With a description height ranging from 6 to 15 feet tall covered head to toe with fur, Sasquatch can’t be that hard to miss. Given a plethora of data to work with, we set out to investigate what factors contributed most to Bigfoot sightings and see if we could build a model that can predict where it will appear next.

We considered factors like location, whether there were many cases of missing or unidentified persons, drug and alcohol use, proximity to campgrounds, and general population growth in the state. We gathered data from the US census Bureau, National Missing and Unidentified Persons System, the National Survey on Drugs Use and Health, and USA Campgrounds Info to bring into our analysis.


## Analysis:

Data Pre-Processing:

Importing .csv files into Jupyter Notebook
Getting rid of duplicates
Filtered for cases of illicit drug use and alcohol among the 18+ age group as seemingly the overwhelming majority of reported sightings.
Filtered census data on a state by state basis
Converting NA values to 0
Grouped by State
Sorted Sightings by Year
Our main focus centered on sightings in the year 2020


Our target is most often seen in wilderness where people can gather for a number of different reasons. Given the nature of the description and somewhat fantastical nature of the claims made by reported sightings, our team focused on human factors that may explain these sightings. Perhaps cases of missing persons misidentified, or perhaps paranoia and bad trips from drug use could explain the phenomenon. To answer those questions, we pulled dataset csvs from the US Census Bureau, US Campgrounds.info, The National Study on Drug Use and Health and the Bigfoot Researchers Organization , loaded them into Juypter notebooks and standardized them to group by state and by the years from 2001-2020, with a focus on the 2020 data. We visualized the different sets of data against BigFoot sightings to see if there were any patterns that emerged.

The states with the highest numbers of bigfoot sightings over the 20-year period are Florida, Illinois, Michigan, Missouri, Ohio, Texas, and Washington. There appears to be a high number of sightings in Washington, a state with 576 campgrounds. The map also shows that Bigfoot sightings tend to appear near coasts and rivers. A majority of bigfoot sightings are in states with higher population density.
                
## Tableau Dashboard                
https://public.tableau.com/javascripts/api/viz_v1.js';               
https://public.tableau.com/app/profile/jenny.shea/viz/BigFootSightings-HBFSStates/B

## Our Factors:


Given our mapping of different possible factors against Bigfoot sightings, we wanted to know if we could input these features and generate a prediction within a high degree of probability (mid to high .70’s)


## Conclusion:


Using sklearn, we initiated a multiple regression model. Our model was sharply below our standards of accuracy. Even with minor adjustments to our data, the testing score did not rise above 0.085. Making it less of 1% accurate.

With this failure in mind, we turn our attention on possible developments for future iterations. Given that the features we tested made many assumptions such as humans being the center cause of sightings, our approach could change to environmental factors. By implementing weather, seasons, even the time of day, we can examine whether there are more explanations for our fuzzy friend than we initially realized.

Though we could calculate the average weather, temperature conditions and aggregate locations of sightings, it is clear that there are far more factors than we realized when it comes to finally solving the mystery of the most difficult game of hide and seek in North America.

## GitHub Webpage
https://jennyshea.github.io/Where-Will-Big-Foot-Appear-Next/
