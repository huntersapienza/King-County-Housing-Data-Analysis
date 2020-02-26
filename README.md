
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

<img src='Images/OSEMN _framework.png'>

## Findings

Below, we provide several key visualizations developed throughout the exploratory data analysis, as well as our findings from the multivariate linear modeling process with regards to the top factors contributing to increased housing value.

**King County Home Sizes**
<img src='Images/housing_size.png'>

The above scatterplots display the correlation between different housing size factors and the selling price. Based on the twelve scatterplots, we notice that 'sqft_living15', 'sqft_living', and 'sqft_above' show the highest positive linear correlation with the selling price of the house. This indicates that larger living spaces reflect higher selling prices.

**Zip Codes**
<img src='Images/zip_codes.png'>

In the above barplot, several zip codes rise to the top with much higher average selling prices per home than the mean selling price for all homes in King County (appoximately 540 thousand dollars). Notable zip codes include those containing the following neighborhoods: Medina, Mercer Island, Madison Park, Montlake, and Capitol Hill. Some of these neighborhoods are shown in the images below. As you can see, many of these are large waterfront homes!

98039, 98040, 98004, and 98112 maintain the highest average selling prices for homes, with all four at a mean over 1 million dollars. 98039 is the zipcode for Medina, a neighborhood within Bellevue with residents such as Bill Gates and other extremely wealthy technology and business billionaires. 98004 is located just adjacent to 98039 and contains very high-end homes as well, at a lower mean than those in Medina, however, possibly due to its location slightly inland, as opposed to Medina's waterfront homes. 98040, located within Mercer Island, is well-known for extremely high-end housing, with easy access to Seattle jobs in the city center just across Lake Washington via the I-90 bridge. 98112, encompasing the Madison Park, Montlake, and north Capital Hill neighborhoods in Seattle, is well known for it's large mansions and extraordinarly high home prices. Kurt Kobain is a notable former resident of the neighborhood, with his memorial located at a park within 98112. The zipcode, located on the west side of Lake Washington contains a large number of waterfront homes and a very desirable location within the city with easy access to jobs and city attractions.

Medina
<img src='Images/medina.jpeg' width="2000">

Madison Park
<img src='Images/madison-park-neighborhood.jpg' width="2000">

Mercer Island
<img src='Images/mercer_island.jpg' width="2000">

**Housing Grade**
<img src='housing_grade.png'>

According to the King County Department of Assessments, grades are provided to houses and residential units as a "classification by construction quality which refers to the types of materials used and the quality of workmanship. Buildings of better quality (higher grade) cost more to build per unit of measure and command higher value" (King County, 2019). As a measure of housing quality, these grades  reflect significant trends associated with average selling price of these houses, as the value increases exponentially with increasing grade levels.

**Top Predictors of Housing Value**
<img src='Images/top_predictors.png'>

By examining a sorted list of feature coefficients from our final multivariate linear model, we identified which variables most affect the selling price of houses.

Just like in our EDA, the zip codes from Medina, Mercer Island, and Madison Park appear at the top, indicating that location is key in the value and selling price of a house. At 8th on the list of top features, 'waterfront_1.0' boasts a fairly high impact on selling price with a correlation coefficient of 0.843. Houses on the water are prime real-estate anywhere, but especially within Seattle and all of King County, where waterfront neighborhoods hold some of the highest value. Additionally, features associated with King County housing grades 11-13 appear within the top 25 predictors while grades 4-7 can be found near the bottom of the list. This indicates that higher-grade houses are positively correlate with price, while those of lower grade tend to result in lower prices.

Ultimately, as displayed in the illustration above, when predicting the selling price of a home, zipcode, waterfront location, and grade/condition rankings will provide the most useful indicators of value.