# data-512-a2

# Assignment 2

## Analysis

Throughout the course of this development, I’ve been privy to learn about the entire population space of Wikipedia articles and comparing the coverage of the politicians based on the population of their respective country, based on API call requests for the data from the English Wikipedia. We also used the available data to determine how many of the articles created in each country were classified by the Wikipedia content classifier as being high quality. 

During the course of my data processing and analysis, it became very clear that the countries with extremely high populations, some of the highest in the world, are very much under covering their politicians. Coincidentally there are consistently significant levels of political strife in many of the countries that are are the bottom of the list of politician articles as a proportion of population (India, China, North Korea among others). 

This leads into the next point about how the internet and global society looks to be working hand in hand to suppress coverage about politicians in highly populated countries. We could take this analysis further and hypothesize that the reason for this extreme under-coverage is to suppress data and information about how politicians in these densely populated and politically turbulent countries are misusing their power and treating their constituents. These patterns emerge and thus bias follows. 

However, some of these discrepancies and skewed results can be attributed to the fact that using solely English Wikipedia to gather and aggregate this data is biased. To truly and properly assess which countries are under covering their politicians based on their population, we need to envelope our research around all the different languages in Wikipedia. A lot of the articles about Indian politicians could be written in Hindi, Tamil, etc. for example. Furthermore, based on the configuration of the Wikipedia content classifier and how they grade articles as being low or high quality, this could be a source of bias in determining the proportion of high quality politician articles by country. 

A question that I thought about while completing this analysis is: At what point as data scientists to we know there is no bias in both the analysis and subsequently the results? Besides reviewing our methodologies and analyzing our spread of data, what other ways can data scientists and analysts mitigate the presence of bias in the analysis. 

## The tables that are included in the analysis are documented as follows: 

Table 1: 10 highest-ranked countries in terms of number of politician articles as a proportion of country population

Table 2: 10 lowest-ranked countries in terms of number of politician articles as a proportion of country population

Table 3: 10 highest-ranked countries in terms of the relative proportion of politician articles that are of GA and FA-quality

Table 4: 10 lowest-ranked countries in terms of the relative proportion of politician articles that are of GA and FA-quality

Table 5: Ranking of geographic regions (in descending order) in terms of the total count of politician articles from countries in each region as a proportion of total regional population

Table 6: Ranking of geographic regions (in descending order) in terms of the relative proportion of politician articles from countries in each region that are of GA and FA-quality

## Data inside the repository 

1) WPDS_2020_data.csv: This csv file includes the country name, the type, the abbreviation of the country, the time frame the data was collected, the population of the country in millions, and the population of the country. 

2) page_data.csv: This csv file includes the politician article, the country that the politician is from, and the rev_id of the article. 

## Hyperlinks to documentation and data outside of the repository

1) https://figshare.com/articles/dataset/Untitled_Item/5513449: page_data.csv is sourced from this link
2) https://www.prb.org/international/indicator/population/table/: WPDS_2020_data.csv sources data from this link
3) https://en.wikipedia.org/wiki/Wikipedia:Content_assessment: Machine Learning tool that Wikipedia uses to grade articles
4) https://ores.wikimedia.org/v3/#!/scoring/get_v3_scores_context_revid_model: API Documentation for ORES used in this analysis
