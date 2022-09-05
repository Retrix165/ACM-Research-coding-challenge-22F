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


## Sources
Apart from referencing Matplotlib and Python 3 documentation a lot to know what I could actually do, the only code I used that wasn't my own was the starting comments and imports that came with starting a new notebook on the "CarsForSale" Kaggle webpage.
