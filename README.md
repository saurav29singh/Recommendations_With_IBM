# Recommendations with IBM
In this project we will analyze the interactions that users have with articles on the IBM Watson Studio platform, and make recommendations to them about new articles.
In order to determine which articles to show to each user, we will be performing a study of the data available on the IBM Watson Studio platform.

## Dependencies
- python 3.7
- jupyter notebook
- numpy
- pandas
- matplotlib

## Descriptions
For this project we are going to use Pycharm IDE to showcases the analysis done in order to explore the dataset, the data preparation and wrangling as well as the building of recommendation engine. In IDE we are going to use Jupyter notebook which contains markdown cells to help with documentation of the steps.

For reference an HTML version of the notebook is also available.

### File Structure
```
- data/
  - articles_community.csv        #articles descriptive information
  - user-item-interactions.csv    #users interactions with articles
- Recommendations_with_IBM.ipynb  #containing implementation and analysis.
- Recommendations_with_IBM.html   #HTML format of notebook
- project_tests.py                #Python file contains solutions for test questions
- top_10.p                        #file contains top 10 articles. 
- top_20.p                        #file contains top 20 articles. 
- top_5.p                         #file contains top 5 articles. 
- user_item_matrix.zip            #Zip file containing user_item_matrix.p. Please uzip before use.
```

## Task overview

I. Exploratory Data Analysis:

    Find out the distribution of articles a user interacts within the dataset and provide a visual and descriptive statistics.

II. Rank Based Recommendations:

    Provide two functions to get n top articles names and n top articles ids.

III. User-User Based Collaborative Filtering:

    Each user should only appear in each row once.
    Each article should only show up in one column.
    If a user has interacted with an article, then place a 1 where the user-row meets for that article-column. It does not matter how many times a user has interacted with the article, all entries where a user has interacted with an article should be a 1.
    If a user has not interacted with an item, then place a zero where the user-row meets for that article-column

IV. Matrix Factorization:

    Using the user-item interactions, we will build out a matrix decomposition.

## Acknowledgement

- Udacity for providing an excellent Data Scientist training program.
- IBM for providing user interaction article dataset from IBM Watson Studio.