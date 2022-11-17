# Fake Reviews Detection (Bootcamp_final_project)

## Table of Contents

- [Background](#background)
- [Python Libraries](#python-libraries)
  - [Web Scrapping](#web-scrapping)
  - [Data Analysis](#data-analysis)
- [Usage](#usage)
- [Performance Overview](#performance-overview)

## Background

This is a bootcamp final project. In this case we will use NLP(natural language processing) to create a NaiveBayes classified model. The target of this project is to detect whether the given review is CG(computer-generated) or not. The project consists of two parts. One is Amazon web scrapping (get the validated data) and the other is data analysis.

## Python Libraries

### Web Scrapping

- BeautifulSoup
- requests
- pandas
- re
- time 
- random

### Data Analysis

- pandas
- nltk
- nltk.stem
- nltk.corpus
- nltk.tokenize
- numpy
- seaborn
- matplotlib.pyplot

## Usage

If you want to create your own NLP classified model. Then you need to open the python-file and run the NLP.ipynb. After the NLP part you will get a new model, but it will take you long time. Instead of creating your own model you can just use the model i built. You just need to load the pickle file and you will get the model.
To the web scrapping part you can directly run the get_review function. You can enter any product links from Amazon, then you will get all reviews of this product.For example https://www.amazon.com/Apple-iPhone-64GB-Space-Gray/product-reviews/B08BHTPV2T/ref=cm_cr_getr_d_paging_btm_next_2?ie=UTF8&reviewerType=all_reviews&pageNumber=1

## Performance Overview

The accuracy of my model is just over 70%. There are some reasons. First of all is the size of the dataset not big enough. Due to the limit of my computer performance i just pick 10k rows randomly from the original dataset. Secondly is when i build the NaiveBayesClassifier Model i just choose the top 5000 most common words. If i enlarge this word-features maybe the result will be improved.
