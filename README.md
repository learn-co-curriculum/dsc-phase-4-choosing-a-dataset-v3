
# Phase 4 Project - Choosing a Dataset

For this phase, you will choose a project that relates to one of the following topics:

- Recommendation Systems
- Model Interpretability
- Natural Language Processing

## The Data

We have provided a dataset suitable to each topic, but you are also welcome to source your own dataset. If you choose your own dataset, **run the dataset and business problem by your instructor for approval** before starting your project.

### How to Choose a Project

When choosing a project, consider one of the following approaches:

1. **Depth:** Choose a project that similar to what you want to do for your capstone project (Phase 5). This will allow you to practice those methods in a group setting before needing to use it independently. This will help you build a better Capstone project and a portfolio that demonstrates the ability to deeply learn and implement one modeling approach.

2. **Breadth:** Choose a problem that you don't necessarily plan to use in your capstone project. This will allow you to develop applied experience with multiple modeling approaches. This will help you refine your areas of interest and build a portfolio that demonstrates the ability to learn and implement multiple modeling approaches.

If you are feeling overwhelmed or behind, we recommend you choose Topic 3: Natural Language Processing.

### Topic 1: Recommendation Systems

If you choose the Recommendation System option, you will be making movie recommendations based on the [MovieLens](https://grouplens.org/datasets/movielens/latest/) dataset from the GroupLens research lab at the University of Minnesota.  Unless you are planning to run your analysis on a paid cloud platform, we recommend that you use the "small" dataset containing 100,000 user ratings (and potentially, only a particular subset of that dataset).

Your task is to:

> Build a model that provides top 5 movie recommendations to a user, based on their ratings of other movies.

The MovieLens dataset is a "classic" recommendation system dataset, that is used in numerous academic papers and machine learning proofs-of-concept.  You will need to create the specific details about how the user will provide their ratings of other movies, in addition to formulating a more specific business problem within the general context of "recommending movies".

#### Collaborative Filtering

At minimum, your recommendation system must use collaborative filtering.  If you have time, consider implementing a hybrid approach, e.g. using collaborative filtering as the primary mechanism, but using content-based filtering to address the [cold start problem](https://en.wikipedia.org/wiki/Cold_start_(computing)).

#### Evaluation

The MovieLens dataset has explicit ratings, so achieving some sort of evaluation of your model is simple enough.  But you should give some thought to the question of metrics. Since the rankings are ordinal, we know we can treat this like a regression problem.  But when it comes to regression metrics there are several choices: RMSE, MAE, etc.  [Here](http://fastml.com/evaluating-recommender-systems/) are some further ideas.

### Topic 2: Model Interpretability

If you choose this option, you'll put everything you've learned together to build and explain a model that is trained on a dataset. In this case, your model will explain the underlying causes in vehicle crashes. The dataset comes from the [City of Chicago](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if). Note this links also to [Vehicle Data](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Vehicles/68nd-jvt3) and to [Driver/Passenger Data](https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d).

Your task is to:

> Build a model that can predict the primary contributory cause of a car accident, given information about the car, the people in the car, the road conditions etc. You might imagine your audience as a Vehicle Safety Board who's interested in reducing traffic accidents, or as the City of Chicago who's interested in becoming aware of any interesting patterns. 
> 
#### Aim for a Proof of Concept

The goal of this project isn't to build the best model possible -- it's to demonstrate your understanding of the model that works. You should try to avoid datasets and model architectures that won't run in reasonable time on your own machine. Once you're absolutely sure that you've found the best possible hyperparameters for your model, then consider leveraging model interpretability to gain insight to why the model is making predictions in that manner it does. 

At the end of the day, we want to see your thought process as you iterate and improve on a model. A project that achieves a lower level of accuracy but has clearly iterated on the model and the problem until it found the best possible approach is more impressive than a model with high accuracy that did no iteration. We're not just interested in seeing you finish a model -- we want to see that you understand it, and can use this knowledge to try and make it even better!

#### Evaluation

Evaluation is fairly straightforward for this project.  But you'll still need to think about which metric to use and about how best to cross-validate your results.

### Topic 3: Natural Language Processing (NLP)

If you choose this option, you'll build an NLP model to analyze Twitter sentiment about Apple and Google products. The dataset comes from CrowdFlower via [data.world](https://data.world/crowdflower/brands-and-product-emotions). Human raters rated the sentiment in over 9,000 Tweets as positive, negative, or neither.

Your task is to:

> Build a model that can rate the sentiment of a Tweet based on its content.

#### Aim for a Proof of Concept

There are many approaches to NLP problems - start with something simple and iterate from there. For example, you could start by limiting your analysis to positive and negative Tweets only, allowing you to build a binary classifier. Then you could add in the neutral Tweets to build out a multiclass classifier.

#### Evaluation

Evaluating multiclass classifiers can be trickier than binary classifiers because there are multiple ways to mis-classify an observation, and some errors are more problematic than others. Use the business problem that your NLP project sets out to solve to inform your choice of evaluation metrics.

### Sourcing Your Own Data

Sourcing new data is a valuable skill for data scientists, but it requires a great deal of care. An inappropriate dataset or an unclear business problem can lead you spend a lot of time on a project that delivers underwhelming results. The guidelines below will help you complete a project that demonstrates your ability to engage in the full data science process.

Your dataset must be...

1. **Appropriate for one of this phase's models.** These are time series, recommendation systems, image classification, or natural language processing.   

2. **Usable to solve a specific business problem.** This solution must rely on your model.

3. **Somewhat complex.** It should contain thousands of rows and features that require creativity to use.

4. **Unfamiliar.** It can't be one we've already worked with during the course or that is commonly used for demonstration purposes (e.g. MNIST).

5. **Manageable.** Stick to datasets that you can model using the techniques introduced in Phase 4.

#### Problem First, or Data First?

There are two ways that you can source your own dataset: **_Problem First_** or **_Data First_**. The less time you have to complete the project, the more strongly we recommend a Data First approach to this project.

**_Problem First_**: Start with a problem that you are interested in that you could potentially solve with a classification model. Then look for data that you could use to solve that problem. This approach is high-risk, high-reward: Very rewarding if you are able to solve a problem you are invested in, but frustrating if you end up sinking lots of time in without finding appropriate data. To mitigate the risk, set a firm limit for the amount of time you will allow yourself to look for data before moving on to the Data First approach.

**_Data First_**: Take a look at some of the most popular internet repositories of cool data sets we've listed below. If you find a data set that's particularly interesting for you, then it's totally okay to build your problem around that data set.

#### Potential Data Sources

There are plenty of amazing places that you can get your data from. We recommend you start looking at data sets in some of these resources first:

* [UCI Machine Learning Datasets Repository](https://archive.ics.uci.edu/ml/datasets.php)
* [Kaggle Datasets](https://www.kaggle.com/datasets)
* [Awesome Datasets Repo on Github](https://github.com/awesomedata/awesome-public-datasets)
* Local data portals for state and local government resources
    - Examples: [NYC](https://opendata.cityofnewyork.us/), [Houston](http://data.houstontx.gov/), [Seattle](https://data.seattle.gov/), [California](https://data.ca.gov/)
* [Inside AirBNB](http://insideairbnb.com/)
* [FiveThirtyEight’s data portal](https://data.fivethirtyeight.com/)
* [Data is Plural’s Archive Spreadsheet](https://docs.google.com/spreadsheets/d/1wZhPLMCHKJvwOkP4juclhjFgqIY8fQFMemwKL2c64vk/edit#gid=0)
* [Datasets Subreddit](https://www.reddit.com/r/datasets/)
* [Tensorflow Datasets](https://www.tensorflow.org/datasets/catalog/overview)
