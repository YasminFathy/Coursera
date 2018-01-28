
Question 1:
------------
A computer program is said to learn from experience E with respect to some task T and some performance measure P if its
performance on T, as measured by P, improves with experience E.

Suppose we feed a learning algorithm a lot of historical weather data, and have it learn to predict weather. What would be a
reasonable choice for P?

-The process of the algorithm examining a large amount of historical weather data.

-The probability of it correctly predicting a future date's weather.

-The weather prediction task.

-None of these.

Answer:
-------
E: The process of the algorithm examining a large amount of historical weather data.

T: The weather prediction task.

P: The probability of it correctly predicting a future date's weather.


**-The probability of it correctly predicting a future date's weather.**

------------------------------------------------------------------------------------------------
Question 2
------------
Suppose you are working on weather prediction, and you would like to predict whether or not it will be raining at 5pm
tomorrow. You want to use a learning algorithm for this.

Would you treat this as a classification or a regression problem?

-Classification

-Regression

Answer:
-------
This problem is considered as classification problem because we have here to predict a discrete value:

0 -> it won't rain

1 -> it will rain


**-Classification**

------------------------------------------------------------------------------------------------
Question 3
------------
Suppose you are working on stock market prediction. You would like to predict whether or not a certain company will declare bankruptcy within the next 7 days (by training on data of similar companies that had previously been at risk of bankruptcy). Would you treat this as a classification or a regression problem?

-Regression

-Classification

Answer:
-------
This problem is considered as classification problem because we have here to predict a discrete value:

0 -> declare bankruptcy

1 -> doesn't declare bankruptcy

**-Classification**

------------------------------------------------------------------------------------------------
Question 4
------------
Some of the problems below are best addressed using a supervised learning algorithm, and the others with an unsupervised
learning algorithm. Which of the following would you apply supervised learning to? (Select all that apply.) In each case, assume some appropriate dataset is available for your algorithm to learn from.

-Take a collection of 1000 essays written on the US Economy, and find a way to automatically group these essays into a small number of groups of essays that are somehow "similar" or "related".

-Examine a large collection of emails that are known to be spam email, to discover if there are sub-types of spam mail.

-Given historical data of children's ages and heights, predict children's height as a function of their age.

-Given 50 articles written by male authors, and 50 articles written by female authors, learn to predict the gender of a new manuscript's author (when the identity of this author is unknown).


Answer:
-------

-Take a collection of 1000 essays written on the US Economy, and find a way to automatically group these essays into a small number of groups of essays that are somehow "similar" or "related".

**This is unspervised learning/clustering problem; it is similar to the Google News example in the video lecture (Week 1).**

-Examine a large collection of emails that are known to be spam email, to discover if there are sub-types of spam mail.

**This is unspervised learning/clustering problem where we need to cluster spam mail into sub-types. This problem is similar to the Google News example in the video lecture (Week 1).**

-Given historical data of children's ages and heights, predict children's height as a function of their age.

**This is as a supervised learning (i.e. regression) problem, where we learn from labeled data (children's ages and heights) to predict children's height given their age.**

-Given 50 articles written by male authors, and 50 articles written by female authors, learn to predict the gender of a new manuscript's author (when the identity of this author is unknown).

**This is as a supervised learning (i.e. classification) problem, where we learn from labeled data (article labelled as written by female or male) to predict gender (i.e. female, male).**


So the answers are:

**-Given historical data of children's ages and heights, predict children's height as a function of their age.**

**-Given 50 articles written by male authors, and 50 articles written by female authors, learn to predict the gender of a new manuscript's author (when the identity of this author is unknown).**


------------------------------------------------------------------------------------------------
Question 5
------------
Which of these is a reasonable definition of machine learning?

-Machine learning is the science of programming computers.

-Machine learning is the field of study that gives computers the ability to learn without being explicitly programmed.

-Machine learning learns from labeled data.

-Machine learning is the field of allowing robots to act intelligently.


Answer:
-------
This is the definiation of machine learning given by Arthur Samuel (1959), who wrote checkers playing learning program, however, he was not a good checkers player).


**-Machine learning is the field of study that gives computers the ability to learn without being explicitly programmed.**
