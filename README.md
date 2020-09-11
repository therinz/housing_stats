![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# Aircraft bird strikes

Dataset analysis in Tableau.
<br>Ironhack Berlin week 4 project
<br>Rinze Douma
<br>05/09/2020

## Content
- [Project description](#Project-description)
- [Workflow](#Workflow)
- [Organization](#Organization)
- [Links](#Links)

## Project description

This is a project as part of the Ironhack Data Analytics course. The goal is to get familiar with Tableau. 
The dataset concerns aircraft bird strikes between 2005 and 2011. I have made several slides to indicate the scope and impact. 

## Workflow
- I browsed on Kaggle for a suitable dataset, with vague ideas in my head leading my search. Since I am highly familiar with aviation, I thought it would be nice to analyze some data in that field. 
- This dataset did not have any description, but the overview was clear from the Kaggle website and appeared usable.
- After downloading I imported the data into Tableau, to explore the different aspects and to see what sort of connections would be possible. 
- The data only had the name of an airfield, without other location data. Because the way the name is written can vary greatly, I used the Google maps API to get coordinates for the ca 1500 airports.
- I found out that the data is mainly based on data from the USA, meaning certain connections with proximity to the sea would be difficult.
- There is one column in the dataset for time of day, which was interpreted by Tableau as a float. I created another Jupyter notebook in order to make this column into a datetime object.
- While doing this I also created a new column to bin the time by hour, but this was not necessary in the end because Tableau can take care of this. 
- After plotting several graphs, I collected them in dashboards.
- These dashboards were bundled in a story.
- Finally, I added notes to point out certain interesting facts, and added a few pictures.

## Organization

#### Data
The csv's that were downloaded and created are in a folder named data. The csv resulting from the time cleanup is the same filename as the product of the location retrieval. This is because Tableau would then update the data source without losing information in the worksheets.

#### Notebooks
There are two Jupyter Notebooks I used to clean the dataset. These are in a folder called Notebooks

#### Other material
Aside from a folder containing 3 images, there is one file containing the Tableau work in the root of the repository. 

## Links
- [Repository](https://github.com/therinz/birdstrike_analysis)
- [Tableau public presentation](https://public.tableau.com/shared/X342GD97G?:display_count=y&:origin=viz_share_link)
- [Kaggle dataset](https://www.kaggle.com/breana/bird-strikes)
- [Wikipedia on bird strikes](https://en.wikipedia.org/wiki/Bird_strike)

