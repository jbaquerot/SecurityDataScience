# SecurityDataScience
Apache Spark 2.2.0 (pyspakr) exercises of Security Data Science Course. 
The exercises of this course are based on KDD 99 competition

# KDD 99 Competition
The competition task was to build a network intrusion detector, a predictive model capable of distinguishing between "bad" connections, called intrusions or attacks, and "good" normal connections

This database contains a standard set of data to be audited, which includes a wide variety of intrusions simulated in a military network environment.

You can find more information in http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html 

# The NSL-KDD Data Set
The data set used in the course is not the original KDD 99 competition but NSL-KDD data set.

The NSL-KDD data set has the following advantages over the original KDD data set:
* It does not include redundant records in the train set, so the classifiers will not be biased towards more frequent records.
* There is no duplicate records in the proposed test sets; therefore, the performance of the learners are not biased by the methods which have better detection rates on the frequent records.
* The number of selected records from each difficulty level group is inversely proportional to the percentage of records in the original KDD data set. As a result, the classification rates of distinct machine learning methods vary in a wider range, which makes it more efficient to have an accurate evaluation of different learning techniques.
* The number of records in the train and test sets are reasonable, which makes it affordable to run the experiments on the complete set without the need to randomly select a small portion. Consequently, evaluation results of different research works will be consistent and comparable.

# How to run the exercises
The course environment is based in Docker. Just go to the folder where you download the project and run (it takes several minutes):

## on MacOs and Linux:
```
docker run -it --rm -p 8888:8888 -v “$(pwd)”:/home/jovyan/work jupyter/all-spark-notebook:4ebeb1f2d154
```

## on Windows:
``` 
docker run -it --rm -p 8888:8888 -v ${PWD}:/home/jovyan/work jupyter/all-spark-notebook:4ebeb1f2d154 
```

