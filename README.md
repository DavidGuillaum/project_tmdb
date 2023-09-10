<h1 align="center">The Movie Data Base Project</h1>

<p align="center">
This repository contains a project with the TMDB dataset. This project is part of the Data Analysis nanodegree by Udacity.
<br>
This dataset comes from the [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) website but it's originally from [IMDB](https://datasets.imdbws.com/) (Internet Movie Database). I choose this dataset because my brothers are actually filmmakers too and it could be interesting to discover the recipe for success. The dataset contains 21 columns (features) and 10866 rows (observations or films). The original files contain JSON objects. A JSON object is a kind of dictionary. This is a list of values and their keys. But in the given file these JSON objects are transformed into simple values with "|" symbol to separate the values. 
After a quick analysis of the data frame and its features, it became clear that I want to create a variable representing the "profit". The best way is to subtract "revenue" from "budget". I could also use the variable "popularity" but as an economist, I prefer this way of doing it. These 2 variables are correlated. If a movie becomes more popular, the revenue will increase and so will the profit. 
I'll directly get rid of the columns "revenue" and "budget" because the inflation adjustments are more relevant.  
__dependant variable:__ "profit" = "revenue" - " budget"  
__independent variables:__ "budget", "director", "runtime", "genres", "release_date", "vote_average", "release_year"  
I choose to answer the following questions:
- Wich features are positively correlated with profit?
- Is the "runtime" on "profit" following a normal shape (people don't like too long or too short movies)?
- What's the best "runtime"?<br>

I'll try to answer those questions in this notebook. I hope you find it interesting and have fun reading my work.

<br>
  <a href="https://www.udacity.com/course/data-analyst-nanodegree--nd002?gclid=Cj0KCQjw0vWnBhC6ARIsAJpJM6eLjKPmFMpZ5a8i4fEyLOcUltz5eTdk3WYaNGnq_FrUZUlSFVMQOAQaApdJEALw_wcB&utm_campaign=19167921312_c_individuals&utm_keyword=udacity%20data%20analyst_e&utm_medium=ads_r&utm_source=gsem_brand&utm_term=143524475759"><strong>Udacity nanodegree</strong></a>
  <br>
  <a href="https://medium.com/@guillaume.david11"><strong>My blog post</strong></a>
  <br>
</p>

## Table of contents

- [How to run the project](#How-to-run-the-project)
- [Motivation and goals](#Motivation-and-goals)
- [Structure](#Structure)
- [Author and acknowledgement](#author-and-acknowledgement)

## How to run the project


Clone the GitHub repository and use Anaconda distribution of Python 3.11.

    $ git clone https://github.com/DavidGuillaum/project_tmdb.git

In addition This will require pip installation of the following:

     pip install pandas
     pip install numpy
     pip install matplotlib
     pip install seaborn


1. Just open the project.ipynb file with jupyter notebook.


## Motivation and goals

The goals of this project are the following:
- Wrangling of data
- Exploration of data 
- Answer 3 questions

## Structure
This project  structure is the following (it was one of my first project and it could optimized by adding a folder "data"):  

- tmdb-movies.csv #cleaned data
- project.ipynb #main project file
- README.md


<br>


## Author and acknowledgement
I'm David Guillaume, currently studying for a master's degree in Data Analytics and Economics at the University of Fribourg (Switzerland). I'm very interested in data sciences and economics in particular (bachelor's degree in Political Economy). I hope you'll like my project. I would like to thank Udacity for overseeing this program.
<br>
<a href="https://www.linkedin.com/in/david-guillaume-a7bb1b201/"><strong>Here is my Linkedin</strong></a>
<br>