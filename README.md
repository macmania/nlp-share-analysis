# Status: [![Build Status](https://travis-ci.org/macmania/recommendation-engine.svg?branch=master)](https://travis-ci.org/macmania/recommendation-engine)
## Goal
Make a recommendation engine that will allow users to type a few words
then give them a list of recommendations from all of the research papers stored
in Open Science or any meta data source.

Hopefully, this library will be able to accommodate other meta data sources such as articles,
essays, etc. that needs to be categorized properly.

After sanitizing and storing all of the categories in the system, implementing Naive Bayes
classifier and SVM to effectively categorize the research papers that may not be specific
enough.

Run a testing suite to check the performance accuracy between svms or naive bayes and what
other techniques with the data that improved, if any.

## Pitfalls:
  - over-estimation, since we're working on small data-set as of now, there is a great
    chance that we might be taking into consideration just a sub-set and over-estimating the
    performance accuracy of only one subject. A way to prevent this is to collect a normalized
    quantity of samples from other fields
  - how to determine how much of the features are garbage and which are not.
    How to compensate losing the features that do need to be accommodated for.

## How to get started:
  src/tagging_corpus.py - has all of the code needed to categorize and get the features
  from the data set.

  data_dump/* - are the subject folders and under that are .json files.


