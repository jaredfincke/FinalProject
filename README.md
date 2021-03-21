 # Is it worth it get Sports Cards Graded #


## Overview ##
With people spending more time inside due to the Covid-19 Pandemic, the sports cards industry is experiencing a boom. Packs of cards are so popular that major retailers are struggling to keep them in stock. This scarcity has led to increased prices in second-hand marketplaces like Ebay. Some of the most valuable and popular cards are star players' Rookie Cards, their first major league card. However, not all Rookie Cards are valued the same. Collectors appear to demand cards that are in the best condition. 

The most certain way to know that one is buying a card in good condition is to buy "graded" cards. Cards that are graded are giving a score out of 10 indicating their condition. A perfect 10 means the card has no imperfections in any way. Such cards can be rare to find as the fragility of their cardstock makes it difficult for cards to remain in this condition. The most popular grading service is PSA. In order for a card to receive a grade, the owner of the card must send their card to PSA to have the card's condition inspected for a fee. 

As an avid sports card collector I do own many star players rookie cards. I try my best to store my valuable cards in hard-plastic cases to ensure that they remain in the best possible condition. In the future, I may want to sell some of these cards and would like to make sure I am getting the highest return value possible. I would like to know how to achieve the said highest value. I have never had one of my cards graded, but would be interested if it was financially smart. 

## Goals ##

This project aims to answer what is the value of getting a card graded when it is graded at a 10, 9, or 8 compared to an ungraded card. I will be using Ebay sales data to look at recent sales of star player's rookie cards in each of the four major sports leagues (MLB, NBA, NFL, MLB). I will be trying to identify the value of each grade in each league and if it is worth to get rookie cards graded in all the sports.


## Data ##
I collected my data from Ebay.com using a third-party web scraping product called [Parsehub](https://www.parsehub.com/).
Utilizing Parsehub, I look at the past 90 days of sales (10/14/2020 to (1/13/2021) of specific sports cards (one of their popular Rookie Cards) for a star-athlete in each major sport. I used my knowledge of sports cards to identify these athletes and card to search. I then added the condition of the card being graded by PSA and receiving either a 10, 9, or 8 grade, or being ungraded. I downloaded each scrape (4 for each player or 16 total) into a csv file with the title of the card, the url, the sale price.

Although Parsehub was quite useful in collecting the data, there was a lot of work in wrangling the data. The [Data folder](https://github.com/jaredfincke/FinalProject/tree/main/Data) in my github contains a folder with the [raw data files](https://github.com/jaredfincke/FinalProject/tree/main/Data/Original_Raw_Data), and a folder with those [files in csv format](https://github.com/jaredfincke/FinalProject/tree/main/Data/Seperate_CSV_Files). I then combined the data into one [combined file](https://github.com/jaredfincke/FinalProject/blob/main/Data/combined_csv.csv). There was still work to be down to get rid of items that matched my search criteria, but were not useful for other reasons such as multiple cards being sold in one listing. My work in identifying these listings and removing them can be found in the notebook called [Data_Retrieval](https://github.com/jaredfincke/FinalProject/blob/main/Notebooks/Data_Retrieval.ipynb). This [filtered data file](https://github.com/jaredfincke/FinalProject/blob/main/Data/Filtered_Data.csv) was then then analyzed in the [techinal notebook](https://github.com/jaredfincke/FinalProject/blob/main/Notebooks/Technical_Notebook.ipynb).

## Table of Content ##
[Project Repo](https://github.com/jaredfincke/FinalProject)
   - [Data](https://github.com/jaredfincke/FinalProject/tree/main/Data)
        - [Original Raw Data - 16 files](https://github.com/jaredfincke/FinalProject/tree/main/Data/Original_Raw_Data)
        - [Seperate CSV Files](https://github.com/jaredfincke/FinalProject/tree/main/Data/Seperate_CSV_Files)
        - [Combined File](https://github.com/jaredfincke/FinalProject/blob/main/Data/combined_csv.csv)
        - [Filtered Data](https://github.com/jaredfincke/FinalProject/blob/main/Data/Filtered_Data.csv)
    
   - [Notebooks](https://github.com/jaredfincke/FinalProject/tree/main/Notebooks)
        - [Data Retreival](https://github.com/jaredfincke/FinalProject/blob/main/Notebooks/Data_Retrieval.ipynb)
        - [Technical Notebook](https://github.com/jaredfincke/Project-1/blob/main/Notebooks/Technical%20Notebook.ipynb)

## Packages and Software ##
Languages : Python
Tools/IDE : Anaconda
Libraries : pandas, numpy, seaborn, matplotlib, statistics, sklearn

Referenced: 
[FreecodeCamp.org](https://www.freecodecamp.org/news/how-to-combine-multiple-csv-files-with-8-lines-of-code-265183e0854/), 
[Matplotlib.org](https://matplotlib.org/stable/tutorials/introductory/pyplot.html), 
[Kaggle.com](https://www.kaggle.com/pmarcelino/comprehensive-data-exploration-with-python), 
[Stackoverflow.com](https://stackoverflow.com/questions/44469313/price-column-object-to-int-in-pandas)