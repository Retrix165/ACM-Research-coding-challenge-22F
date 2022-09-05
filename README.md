# ACM Research coding challenge (Fall 2022) by Reid Smith
My README description of my project for my ACM Research application

## My Goal
> I haven't worked with large data sets in a while, so I had to take a lot of time to refamiliarize myself with how to use/read them in the first place. After experimenting with the data set for a bit, I tried to find out if there was a relationship between the SellerRating and Price columns. I predicted it would be a positive relationship and wanted to visualize it using a PyPlot graph. This was just a starting task though. I tried to create my own question/problem but the suggested one of *"What car color is the most expensive?"* seemed just right in the end. I did add onto the initial task though by wanting to see if I could add any additional parameters that would make the most expensive/cheap result more realistic if it wasn't already.


*TLDR:* I ended up focusing on determining the most cheap/expensive car colors, and how the way I sanitized the data would affect the results
## Code Description

I have 3 main code sections (as shown by the 'code blocks' in the code file). 
**Run the first section before either section two or three.**

1. *First Section*: This is the setup portion of my code. Contains my import statements, loading the data file as a Pandas DataFrame, and modifying the Price column to hold integer representations of the car price instead of a string.


2. *Second Section*: This portion has the code that answers my main goal. Creates a dictionary that keys each car color to a list of prices of cars of the same color, displays a box and whisker plot of the prices of a certain car color (ordered alphabetically), outputs the 5 most and least expensive car colors based purely on their mean price without any data sanitization, and outputs the same but with better data sanitization.


3. *Third Section*: This was the starting experiment code to refamiliarize myself with large data sets/graphing. It simply displays a scatterplot of all cars SellerRating versus their respective Price columns.

I spent about 2.5-3 hours on this code in total.

## Results

**Scatterplot of Seller Ratings versus Car Prices (The Experimental Graph)**

![alt text](https://github.com/Retrix165/ACM-Research-coding-challenge-22F/blob/main/SellerRatingVPrice.png "SellerRatingVPrice.png")

>*The scatterplot has a slight positive correlation between the two variables, possibly quadratic, but I would have to perform a regression to be certain of that observation*


**Box and Whisker Plot of Car Colors and Their Prices (Ordered Alphabetically by Color Name)**

![alt text](https://github.com/Retrix165/ACM-Research-coding-challenge-22F/blob/main/ColorVPrice.png "ColorVPrice.png")

>*Actually reading this graph seems impossible to see specific colors and their price ranges due to high volume of color names to display. However, displaying slices of the data (not shown in code) does indeed display legible box and whisker pieces.*


**Cheapest and Most Expensive Car Colors Results (Both Simple and 'Better')**

```
Simple Mean Sorting:
5 Cheapest Car Colors on Average: ('Vista Blue Metallic', 3995.0), ('Atlantis Blue Metallic', 8990.0), ('Arctic Ice', 9991.0), ('Basalt Black Metallic', 9995.0), ('Ash Black', 10799.0)

5 Most Expensive Car Colors on Average: ('Grigio Nimbus Metallic', 262500.0), ('Rosso Mars Metallic', 274435.0), ('Grigio Lynx Metallic', 279950.0), ('Grigio Lynx', 284990.0)


Better Mean Sorting:
5 Cheapest Car Colors on Average: ('Quartz White Pearl', 17453.14285714286), ('Black Noir Pearl', 23301.666666666668), ('Bellanova White Pearl', 23692.0), ('Black Sand Pearl', 23984.777777777777), ('Blaze Blue', 25412.333333333332)

5 Most Expensive Car Colors on Average: ('Eiger Grey', 68894.15384615384), ('Santorini Black', 69669.44680851063), ('Deep Blue Metallic', 70741.77777777778), ('Nardo Gray', 72356.0)
```
 >*The Simple Mean Sorting Results are based purely on the cheapest averagely priced color while the Better Mean Sorting Results only considers colors that have been sold at least 5 times. This change is an improvement because a sports car that has a specific rare color that is only sold once could be considered an outlier compared to a slightly less expensive (still pricey) color that is sold much more often.*

## Future Work?
If I could continue working on this project, I would work to find ways that would better sanitize the inputs for the Cheapest and Most Expensive Car Colors investigation. Possibly, I would only consider colors that are sold on multiple cars (not just a single vehicle), or do that but with similar colors such as Pearl White and Snow White being grouped together to find their means. I'm not sure how it would change the results but it is interesting. Additionally, finding better ways to statistically analyze the data and draw better results would be satisfying.

## Sources
Apart from referencing Matplotlib and Python 3 documentation a lot to know what I could actually do in those areas, the only code I used that wasn't my own was the starting comments and imports that came with starting a new notebook on the "CarsForSale" Kaggle webpage.
