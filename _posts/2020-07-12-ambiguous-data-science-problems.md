# Identifying and Solving Ambiguous Data Science Problems

![Image for post](/images/2020-07-12-ambiguous-data-science-problems/media/image1.jpeg)

In data science, and really science in general, the problems that need to be solved are often not clear. If you do not work in the sciences you may find this surprising. When you read research papers it often may seem that solving the problems addressed in the paper is a natural next step in the field, but that is often not the case and it often takes a lot of creativity to just reach the point of deciding what questions to answer. The same applies in industry if not more so. Many companies have large repositories of data but don’t know what they can do with this data (i.e., they don’t know the questions they should be asking), but that’s OK! Fortunately for companies there are people they can hire that are experts in finding value in data — data scientists. A good data scientist is comfortable working in areas of uncertainty and is able to identify and solve problems that bring value to the company.

In terms of training to identify and solve these types of problems, it is a continuous learning process that is often acquired through experience. For me, I currently work as a data scientist in industry, but I mostly gained training in working in areas of uncertainty while completing my PhD. I often worked with datasets that were collected by another researcher that was no longer working at the university and the problem to be solved was not always clear. But still, it is a continuous learning process.

Even though I believe it is best to learn this skillset through experience, to get you started, here, I am going to share a few strategies I have found useful in identifying and solving ambiguous data science problems.

## 1\. Identify high-impact problems that can be solved with data science

Typically, when working with businesses, data scientists are trying to help increase profits. There are likely many problems if solved would lead to increased profits, but since there are only so many hours in the day, it’s beneficial to identify high-impact problems that will likely benefit from data science. When trying to identify high-impact problems to solve, I often will probe the client for problems that will lead to either an increase in revenue or decrease in cost. A couple of examples could be building a recommender system to increase sales or optimizing a distribution workflow to decrease costs. Many scenarios should be explored and discussed. It’s also important to consider the feasibility of the problem, which is where step \#2 comes into play.

## 2\. Identify data available or resources to collect new data

After identifying a few candidate problems, the next step is to identify the data that can be used to solve this problem. For a data science problem to be solved, there typically needs to be data. This may be data that the company already owns or possibly an open-source dataset (or even a combination of both!). There may also be cases where it is best to collect new data. Depending on what type of data is being collected, this may not be as difficult as you think with the use of services such as [Amazon Mechanical Turk](https://www.mturk.com/). It’s also OK if the data is not perfect. Many data scientists have extensive experience working with messy data, so this is nothing new to us; also, in step \#4, I will discuss how we can improve datasets over time. After reviewing the data sources, the next step is to choose the first problem to target!

## 3\. Solve the problem

The next step is to solve the problem! With most of my work, this involves training a machine learning classifier, but it’s really important to realize that training a model is typically only part of the solution. Rather than just model predictions, often model interpretation is the most important step. For example, you may train a model that is going to predict if you will retain a customer or not, but that prediction alone is useless. You need to identify what features you can manipulate to change your customers’ behavior. This is where utilizing model interpretation techniques and running simulations often come into play. I discuss this in more detail in my [previous blog post](https://towardsdatascience.com/machine-learning-algorithms-are-not-black-boxes-541ddaf760c3).

## 4\. Iterate

Depending on the type of problem, often even after the problem is “solved” there is still more work to be done. First, in step \#2, I mentioned that you often want to improve the dataset over time. For example, you may want to elicit feedback from users to continue increasing the size of your dataset. As your dataset grows and the quality improves, you may want to try more sophisticated machine learning approaches. Also, related to eliciting feedback from users, depending on the type of problem, you likely will have to monitor for model drift (i.e., making sure model performance remains at an expected level).

## Conclusions

I hope you find these steps useful. Again, becoming comfortable in areas of uncertainty is a learning process, so it’s OK if you struggle at first. If you are an aspiring data scientist, I think the first step in terms of learning this skillset is simply realizing that many company’s don’t know the exact questions they should be answering to extract value out of their data, so you’ve already completed the first step! Lastly, if you think your company can benefit from my services, feel free to reach out to me (my contact information is available on my [website](https://zachmonge.github.io/)).
