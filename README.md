
# King County Housing Data


## Introduction

In the following project, we examine and analyze data to determine the factors that most significantly contriubte to increased housing value. We will employ the OSEMN (obtain, scrub, explore, model, and interpret) data science process to determine the effect of various features on housing sales prices via a multivariate linear model.

The housing data utilized throughout this project comes from King County, Washington (shown below). King County comprises the greater Seattle area, including the city of Seattle and many surrounding suburbs to the North, East, and South. It is the most populous county in the state, with over 2 million residents, and the 12 most populous in the country.

<img src='Images/King_County_WA.png'>

<img src='Images/King_County_Seattle.jpg'>

## Objectives
Throughout this project we will aim to answer the following questions through exploratory analysis:
* How does **living space** affect the selling price of a home?
* How do **zip code** and **location** affect the selling price of a home?
* How do **age** and **time** affect the selling price of a home?
* How does the **ranking** assigned by King County affect a house's value?
* How does the **number of views** a house receives correlate with its value?
* How does the **condition ranting** of a house affect its selling price?

Ultimately our analysis and modeling process will culminate by answering the following essential question:
#### **Which factors most significantly contribute to increased housing value?**

## Data Science Process

Across the scope of the project, we touch upon various components of our data science process, depending on the research question at hand. However, the overall project from start to finish adheres to the OSEMN framework:

1. Obtain
2. Scrub
3. Explore
4. Model
5. Interpret

<img src='Images/OSEMN_framework.png'>

## Findings

Below, we provide several key visualizations developed throughout the exploratory data analysis, as well as our findings from the multivariate linear modeling process with regards to the top factors contributing to increased housing value.

**King County Home Sizes**
<img src='Images/housing_size.png'>

The above scatterplots display the correlation between different housing size factors and the selling price. Based on the twelve scatterplots, we notice that 'sqft_living15', 'sqft_living', and 'sqft_above' show the highest positive linear correlation with the selling price of the house. This indicates that larger living spaces reflect higher selling prices.

**Zip Codes**
<img src='images/zip_codes.png'>

In the above barplot, several zip codes rise to the top with much higher average 
