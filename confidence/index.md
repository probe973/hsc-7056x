---
layout: default
title: Confidence Intervals Workshop
---

<div class="explanation" markdown="1">

# Confidence Intervals

In this workshop you will perform some calculations to create confidence intervals for the mean.  You will also explore what factors influence the size of a confidence interval.

Researchers often want to estimate a measure, such as the mean, of a population.  Measures that describe a population are known as parameters.  If everyone in the population can be measured (i.e. a census) then there is no need to estimate parameters.  However, samples from a population are more often used and statistics are calculated from the sample.  These statistics are then used to estimate the population parameters.

</div>

<div class="instructions" markdown="1">

### Point and Interval Estimates

A **statistic** means something that is calculated from a sample.  For example, when we calculate the mean score from a sample, this score is known as a **statistic**

A **parameter** is a measure from the population, and is often unknown.  When you calculate statistics from a sample you are often trying to estimate the value of a **population parameter**

The **mean** is often a useful piece of information to know about a population.  A **sample mean** can be used to estimate the **population mean**.  So if a sample of 80 people in a particular population of interest gives a mean score of 52, you would estimate the population mean to be 52.  This is known as a **point estimate**

Point estimates are good for giving readers a precise answer, but you have no confidence that this is the **true** value in the population.  This is because:

$$\text{true score} = \text{sample estimate} \pm \text{error}$$

Researchers will often also give **interval estimates** of the population parameter, so a range of possible values it can take.  It will also be associated with a **level of confidence** in the interval.  A commonly used interval is a **95% confidence interval**.  So a 95% confidence interval for a population mean may be given as:

$$52 \pm 6$$

This means that we can be 95% confident that the true mean lies between $52 - 6 = 46$ and $52+6=58$, so the confidence interval may also be written $(46, 58)$.

It's 95%, or whatever percent is given, because when a researcher calculates the 95% confidence interval from their sample, 95% of samples will correctly 'trap' the true mean.

</div>

Let’s say that a researcher is interested in the mean length of time people had symptoms of a particular virus.  They collect a sample from the population of people who had the virus and calculate the mean length to be 6.4 days.  

{% include question_numerical.html
    id="ciq1"
    title="1"
    question_text="With the information given, what would be the researcher’s estimate of the population mean number of days people were ill with the virus?"
    correct_answer="6.4"
    tolerance="0.01"
    solution_text="The best estimate for the population mean would be the sample mean: 6.4 days"
%}

Using other statistics collected from the sample, the researcher also calculates a 95% confidence interval for the population mean.  It is calculated as (4.6, 8.2).

{% include question_multiple_choice.html
    id="ciq2"
    title="2"
    question_text="What is the interpretation of this confidence interval?"
    options="wrong1::We are 5% confident that the true mean is between 4.6 and 8.2 days||correct::We are 95% confident that the true mean is between 4.6 and 8.2 days||wrong2::We are 95% confident that the true mean is outside of 4.6 and 8.2 days||wrong3::We have no idea how many days people had the virus for on average"
    correct_answer="correct"
    solution_text="We are 95% confident that the true mean is between 4.6 and 8.2 days"
%}
