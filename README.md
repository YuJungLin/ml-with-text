## Tutorial: Machine Learning with Text using Python

Adapted from some of the content from [Kevin Markham](http://www.dataschool.io/about/).

Instructor: [Vaibhav Srivastav](https://www.linkedin.com/in/vaibhavs10/)

### Description

Although numeric data is easy to work with in Python, most knowledge created by humans is actually raw, unstructured text. By learning how to transform text into data that is usable by machine learning models, you drastically increase the amount of data that your models can learn from. In this tutorial, we'll build and evaluate predictive models from real-world text using scikit-learn.

### Objectives

By the end of this tutorial, attendees will be able to confidently build a predictive model from their own text-based data, including feature extraction, model building and model evaluation.

### Required Software

Attendees will need to bring a laptop with [scikit-learn](http://scikit-learn.org/stable/install.html) and [pandas](http://pandas.pydata.org/pandas-docs/stable/install.html) (and their dependencies) already installed. Installing the [Anaconda distribution of Python](https://www.continuum.io/downloads) is an easy way to accomplish this. Both Python 2 and 3 are welcome.

I will be leading the tutorial using the IPython/Jupyter notebook, and have added a pre-written notebook to this repository. I have also created a Python script that is identical to the notebook, which you can use in the Python environment of your choice.

### Tutorial Files

* IPython/Jupyter notebooks: [tutorial.ipynb](tutorial.ipynb), [tutorial_with_output.ipynb](tutorial_with_output.ipynb), [exercise.ipynb](exercise.ipynb), [exercise_solution.ipynb](exercise_solution.ipynb)
* Python scripts: [tutorial.py](tutorial.py), [exercise.py](exercise.py), [exercise_solution.py](exercise_solution.py)
* Datasets: [data/sms.tsv](data/sms.tsv), [data/yelp.csv](data/yelp.csv)

### Prerequisite Knowledge

Attendees to this tutorial should be comfortable working in Python, should understand the basic principles of machine learning, and should have at least basic experience with both pandas and scikit-learn. However, no knowledge of advanced mathematics is required.

### Abstract

It can be difficult to figure out how to work with text in scikit-learn, even if you're already comfortable with the scikit-learn API. Many questions immediately come up: Which vectorizer should I use, and why? What's the difference between a "fit" and a "transform"? What's a document-term matrix, and why is it so sparse? Is it okay for my training data to have more features than observations? What's the appropriate machine learning model to use? And so on...

In this tutorial, we'll answer all of those questions, and more! We'll start by walking through the vectorization process in order to understand the input and output formats. Then we'll read a simple dataset into pandas, and immediately apply what we've learned about vectorization. We'll move on to the model building process, including a discussion of which model is most appropriate for the task. We'll evaluate our model a few different ways, and then examine the model for greater insight into how the text is influencing its predictions. Finally, we'll practice this entire workflow on a new dataset, and end with a discussion of which parts of the process are worth tuning for improved performance.

### Detailed Outline

1. Model building in scikit-learn (refresher)
2. Representing text as numerical data
3. Reading a text-based dataset into pandas
4. Vectorizing our dataset
5. Building and evaluating a model
6. Comparing models
7. Examining a model for further insight
8. Practicing this workflow on another dataset
9. Tuning the vectorizer (discussion)

### About the Instructor

Vaibhav Srivastav is a Data Scientist currently working with Deloitte Consulting LLP. He has a demonstrated experience of more than 3 plus years in building large scale Machine Learning and Natural Language Processing solutions for Fortune Technology 10 clients.

In his free time he teaches Machine Learning/ Data Science to young coders! If Python is what floats your boat then hit him up on any of the channels below:  

* Email: [Vaibhavs10@gmail.com](mailto:vaibhavs10@gmail.com)
* Twitter: [@Vaibhavsriv10](https://twitter.com/vaibhavsriv10)

### Recommended Resources

**Text classification:**
* Read Paul Graham's classic post, [A Plan for Spam](http://www.paulgraham.com/spam.html), for an overview of a basic text classification system using a Bayesian approach. (He also wrote a [follow-up post](http://www.paulgraham.com/better.html) about how he improved his spam filter.)
* Coursera's Natural Language Processing (NLP) course has [video lectures](https://class.coursera.org/nlp/lecture) on text classification, tokenization, Naive Bayes, and many other fundamental NLP topics. (Here are the [slides](http://web.stanford.edu/~jurafsky/NLPCourseraSlides.html) used in all of the videos.)
* [Automatically Categorizing Yelp Businesses](http://engineeringblog.yelp.com/2015/09/automatically-categorizing-yelp-businesses.html) discusses how Yelp uses NLP and scikit-learn to solve the problem of uncategorized businesses.
* [How to Read the Mind of a Supreme Court Justice](http://fivethirtyeight.com/features/how-to-read-the-mind-of-a-supreme-court-justice/) discusses CourtCast, a machine learning model that predicts the outcome of Supreme Court cases using text-based features only. (The CourtCast creator wrote a post explaining [how it works](https://sciencecowboy.wordpress.com/2015/03/05/predicting-the-supreme-court-from-oral-arguments/), and the [Python code](https://github.com/nasrallah/CourtCast) is available on GitHub.)
* [Identifying Humorous Cartoon Captions](http://www.cs.huji.ac.il/~dshahaf/pHumor.pdf) is a readable paper about identifying funny captions submitted to the New Yorker Caption Contest.
* In this [PyData video](https://www.youtube.com/watch?v=y3ZTKFZ-1QQ) (50 minutes), Facebook explains how they use scikit-learn for sentiment classification by training a Naive Bayes model on emoji-labeled data.

**Naive Bayes and logistic regression:**
* Read this brief Quora post on [airport security](http://www.quora.com/In-laymans-terms-how-does-Naive-Bayes-work/answer/Konstantin-Tt) for an intuitive explanation of how Naive Bayes classification works.
* For a longer introduction to Naive Bayes, read Sebastian Raschka's article on [Naive Bayes and Text Classification](http://sebastianraschka.com/Articles/2014_naive_bayes_1.html). As well, Wikipedia has two excellent articles ([Naive Bayes classifier](http://en.wikipedia.org/wiki/Naive_Bayes_classifier) and [Naive Bayes spam filtering](http://en.wikipedia.org/wiki/Naive_Bayes_spam_filtering)), and Cross Validated has a good [Q&A](http://stats.stackexchange.com/questions/21822/understanding-naive-bayes).
* My [guide to an in-depth understanding of logistic regression](http://www.dataschool.io/guide-to-logistic-regression/) includes a lesson notebook and a curated list of resources for going deeper into this topic.
* [Comparison of Machine Learning Models](https://github.com/justmarkham/DAT8/blob/master/other/model_comparison.md) lists the advantages and disadvantages of Naive Bayes, logistic regression, and other classification and regression models.