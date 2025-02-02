![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# Lab | Reading About Statistic Concepts

## Introduction

In the future, you will need to understand deep statistical concepts by reading technical articles. As a training for that, it is interesting to start from here. Also, as we have limited time, this is a way to have some self guided learning to understand everything better and have a wider knowledge.

This week you will find some questions here that you will need to answer by documentating yourself. So you will do a different PR for each question (you are meant to answer the questions in different days). Don't hesitate to write as many text as you need and push images if you need them.

Remember for this lab: there is a right answer. But there is no perfect way to explain it (except for in a mathematical way, but this is another story).

## Challenges

### Challenge 1: What is the difference between expected value and mean?
You know both concepts but, is there a difference? Are they synonims? Start investigating. 

Mean is defined as the sum of a collection of numbers divided by the number of numbers in the collection.
Expected value (EV) is the long-run average value of repetitions of the experiment it represents.


A probability distribution defines the relative frequency of outcomes of a random variable.
The expected value can be thought of as a weighted average of those outcomes (weighted by the relative frequency).
Similarly, the expected value can be thought of as the arithmetic mean of a set of numbers generated in exact proportion to their probability of occurring
(in the case of a continuous random variable this isn't exactly true since specific values have probability 0).

The connection between the expected value and the arithmetic mean is most clear with a discrete random variable, where the expected value is

E(X)=∑s xP(X=x)

where s is the sample space. As an example, suppose you have a discrete random variable X such that:

X= 1 with probability 1/8 and equals 2 with probability 3/8 and equals 3 with probability 1/2.

That is, the probability mass function is P(X=1)= 1/8, P(X=2)= 3/8, and P(X=3)= 1/2. Using the formula above, the expected value is

E(X)=1⋅(1/8) + 2⋅(3/8) + 3⋅(1/2) = 2.375

Now consider numbers generated with frequencies exactly proportional to the probability mass function - for example, the set of numbers
{1,1,2,2,2,2,2,2,3,3,3,3,3,3,3,3} - two 1s, six 2s and eight 3s. Now take the arithmetic mean of these numbers:

(1 + 1 + 2 + 2 + 2 + 2 + 2 + 2 + 3 + 3 + 3 + 3 + 3 + 3 + 3 + 3) / 16 = 2.375

and you can see it's exactly equal to the expected value.




As a good reference (once you have looked for some information) you have   [this](http://expected.news/value2) article.





### Challenge 2: What is the "problem" in science with p-values?
We have told you that a lot of scientifical investigations are based on p-values. The last week, Nature magazine published [an article](http://nature.social/statistical4) regarding the problem. Start digging on it!

Don't hesitate to use more articles if you want to :)


The correct interpretation of a p-value is:
Assuming that your null is true, a p-value quantifies the probability of seeing a data point at or beyond your current observation.

Basically, you calculate a 95% confidence interval of where you expect your data to be. If you observe a value that is outside these bounds,
it is unexpected as it is within the most extreme 5% of your data and supports your null hypothesis. If you want to be more lenient to variation,
you might calculate a 97.5% confidence interval and only allow observations with p-values of 0.025 to disapprove your hypothesis.
The best way to combat the fickle p-value is to increase the number of replicates that you do and see if your p-value jumps around or if it stays consistently low.






### Challenge 3: Applying testing to a specific case: A/B testing.
A/B testing is a widely used tool to understand differences between two samples. It is a way to measure the impact of something we did: 
* A marketing campaign.
* A new feature in our application. 
* A new design in our application.
* A different flow in the User Experience flow.

To do this, is very important first to design our experiment. 
* We need to know how we are measuring the impact. If people has the behaviour we want with this new implementation.
* We choose a control group (people who doesn't have/see the new change) and the group which will see the new change. 
* We think about how much data do we need.
* We measure the difference between them.

One example:
Our application has a lot of mini-games. We want people to reach the games that we think are the best but the behaviour is not the expected, they don't reach them.

So we call a designer and after a lot of work he shows us a new design for our application: we will add a botton specific for that kinf of games inviting the users to click on it:

*Click here to discover cool games!*

We think it will work but can we be sure? So instead of implementing this new botton for all users, we implement it for 10% and we compare the results with the users that didn't have it. Is there a significant difference? Is our botton working?

Read more about A/B testing with a couple of examples:

[Another example about Netflix here](http://select.video/artwork4)

[What happened to Basecamp](http://millions.social/tested7)

[An example with Python](http://math.social/tested3)

[A cool general explanation](http://arts.show/tested7)

So, take one single example in the articles you just read, which specific test/s would you apply? (We want you just to do a draft and think a little bit how to apply the tests you already know in this case)

Before the A/B Test:
1. Pick one variable to test.
2. Identify your goal.
3. Create a 'control' and a 'challenger.'
4. Split your sample groups equally and randomly.
5. Determine your sample size (if applicable).
6. Decide how significant your results need to be.
7. Make sure you're only running one test at a time on any campaign.

During the A/B Test:
8. Use an A/B testing tool.
9. Test both variations simultaneously.
10. Give the A/B test enough time to produce useful data.
11. Ask for feedback from real users.

After the A/B Test:
12. Focus on your goal metric.
13. Measure the significance of your results using our A/B testing calculator.
14. Take action based on your results.
15. Plan your next A/B test.

To simplify these steps:
First we have to define and determine our goal, then we decide which variable we will test,
then we make our hypothesis for the test, design and conduct the test and then wait for it to accumilate data,
then use the data that you have from the test to see if the test/changes were significant or not, and then take actions after,
weither to implement the new change of do another A/B test.


## Deliverables
You need to submit a markdown file with the answers to the questions above. You can create a new `.md` file or directly edit the `README.md`.

## Submission
Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.
