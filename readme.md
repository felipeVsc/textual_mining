
## Problem Description

### What is the problem you want to solve?

Classification of journalistic texts into predefined categories/topics.

This project involves the persona of a journalist who is in the process of writing a news article. They need help classifying their article into different topics (e.g., politics, economy, and others), as well as generating impactful headlines and summaries that convey the most relevant information.

The main focus will be on **classifying news articles into predefined categories**. However, it should also generate other relevant information such as: *news headline, news summary, keywords*.

In other words, given a text, the system should be able to provide:

* Categories
* Headline
* Summary
* Keywords

## Dataset Used

### Specify the dataset that will be used. Include the source and link (if applicable). Provide relevant descriptive statistics.

The dataset used for this project is the "News Category Dataset", available on Kaggle: [https://www.kaggle.com/datasets/rmisra/news-category-dataset](https://www.kaggle.com/datasets/rmisra/news-category-dataset)

The dataset contains 210 thousand news articles from 2012 to 2022, taken from HuffPost, a traditional U.S.-based news aggregator. It includes news data from over 42 categories, such as politics, wellness, travel, style & beauty, among others.

It consists of the following attributes:

* `category`: category in which the news article was published
* `headline`: title of the news article
* `authors`: list of authors
* `link`: link to the original news article
* `short_description`: summary of the news article
* `date`: publication date

There are some details about the dataset, such as the fact that there are about 10 thousand news articles from 2018 to 2022, but 200 thousand from 2012 to 2018. However, since we will not address the temporal aspect in this project, this fact should not influence the results.

Citation: Misra, Rishabh. "News Category Dataset." *arXiv preprint arXiv:2209.11429* (2022).

## Goals and Success Criteria

The category classification step, which is the core of this project, should achieve an accuracy rate above 38%. This value corresponds to the result obtained by a DummyClassifier for the three main categories. This result was achieved using only data embeddings, without any preprocessing.

### Explain how you plan to evaluate the results and what you consider as minimum success.

The category classification step should achieve an accuracy rate above 38%. This value corresponds to what a DummyClassifier would achieve on this task, for the three main classes, within a scope of 900 items.

For summarization tasks (headline generation, summary generation), distance metrics will be used on training and test datasets to evaluate how close the AI-generated texts are to those written by journalists.

## Additional Comments

The idea behind this project was not only to perform a classification task, but also, given the opportunity to deliver a demo, to include features that could be applied in a real-world context and actually help someone.
