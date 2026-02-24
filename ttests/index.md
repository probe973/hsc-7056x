---
layout: default
title: t Tests
---

<div class="explanation" markdown="1">

# T-tests

T-tests are used to compare a sample mean with a population mean, or to compare two sample means, to infer whether there are differences in the population.

</div>

<div class="explanation" markdown="1">
  
## One-sample t-test

A one-sample t-test is used to test whether a sample mean is different from a hypothesised mean.

</div>

The mean IQ is known to be 100.  A researcher wants to test whether people in Norwich have a different mean than 100.  They collect a sample of 10 students and give them an IQ test.  The results were:

110, 98, 103, 99, 95, 112, 120, 100, 112, 101

{% include question_numerical.html
id="ttestq1"
title="1"
question_text="Find the mean IQ score for the sample of Norwich people."
correct_answer="105"
tolerance="0.5"
solution_text="$\text{sample mean} = \frac{110+ 98+ 103+ 99+ 95+ 112+ 120+ 100+ 112+ 101}{10}=105$"
%}

{% include question_numerical.html
id="ttestq2"
title="2"
question_text="How many IQ points difference is there between this sample mean and the population mean (100)?"
correct_answer="5"
tolerance="0.5"
solution_text="$105-100=5$"
%}

<div class="explanation" markdown="1">

### Standard Error of the Mean

When estimating a population mean from a sample mean there will be error in our estimate (the **standard error**).  The **standard error of the mean** is related to how spread out the data are and how big the sample is.

$$\text{standard error of the mean} = \frac{s}{\sqrt{n}}$$

Where $s$ is the sample standard deviation and $n$ is the sample size.

Higher standard deviations (greater spread in the sample) lead to higher standard error.

Higher sample sizes lead to lower standard error.

</div>

{% include question_numerical.html
id="ttestq3"
title="3"
question_text="Given that the standard deviation of the sample above is 7.6, calculate the standard error of the mean.  Give your answer correct to 2 decimal places."
correct_answer="2.40"
tolerance="0.005"
solution_text="$\text{SEM} = \frac{7.6}{\sqrt{10}}=2.40$"
%}

<div class="explanation" markdown="1">

### The t Statistic

The **t statistic** can be thought of as a type of standardised measure of difference between two values.  The bigger the t statistic, the bigger the difference.  For a **one-sample t-test** it can be calculated with the formula:

$$t = \frac{\bar{x} - \mu}{\text{SEM}}$$

Where $\bar{x}$ is the sample mean and $\mu$ is the population mean.

Another importance calculation is the degrees of freedom (df).  For a one-sample t-test the degrees of freedom are sample size minus 1.

</div>

{% include question_numerical.html
id="ttestq4"
title="4"
question_text="Calculate the t-statistic for the difference between the sample mean and the hypothosised mean of 100 from the data above.  Given you answer correct to 2 decimal places."
correct_answer="2.08"
tolerance="0.005"
solution_text="$t=\frac{105-100}{2.4}=2.08$"
%}

{% include question_numerical.html
id="ttestq5"
title="5"
question_text="Calculate the degrees of freedom of this t statistic"
correct_answer="9"
tolerance="0"
solution_text="$\text{df}=10-1=9$"
%}

<div class="explanation" markdown="1">

### p-values

Using the t-statistic and the degrees of freedom, a p-value can be calculated.  The p-value can be used to determine whether there is evidence of a difference in the population.  Conventionally, p-values of less than 0.05 are considered evidence of a difference.

A p-value of less than 0.05 is considered evidence of a difference **at the 5% level**

</div>

{% include question_multiple_choice.html
    id="ttestq6"
    title="6"
    question_text="For this IQ experiment: $t = 2.08$, $\text{df} = 9$, $p = 0.0673$.  <br> Would these statistics give evidence that the people of Norwich have a significantly different IQ to 100, at the 5% level."
    options="no::Not enough evidence of a difference in IQ from 100||yes::There is evidence of a difference in IQ from 100"
    correct_answer="no"
    solution_text="No, since for this case $p=.0673 \gt 0.05$, there is not enough evidence of a difference from 100."
%}

---

A similar study is conducted using a sample of students from UEA.  The question is whether UEA students have a different IQ than 100.  A sample of size 30 is taken, and statistics are calculated:

Sample mean = 105; Sample SD = 7.6

{% include question_numerical.html
id="ttestq7"
title="7"
question_text="Calculate the standard error of the mean. Give your answer correct to 2 decimal places."
correct_answer="1.39"
tolerance="0.005"
solution_text="$\text{SEM} = \frac{7.6}{\sqrt{30}}=1.39$"
%}

{% include question_numerical.html
id="ttestq8"
title="8"
question_text="Calculate the t-statistic for the difference between the sample mean and the hypothosised mean of 100 from the UEA data.  Given you answer correct to 2 decimal places."
correct_answer="3.60"
tolerance="0.005"
solution_text="$t=\frac{105-100}{1.39}=3.60$"
%}

{% include question_multiple_choice.html
    id="ttestq9"
    title="9"
    question_text="The results come out as t = 3.60, df = 29, p = 0.00116.  Is there evidence of a difference, at the 5% level, between UEA IQ and the value of 100?"
    options="no::Not enough evidence of a difference in IQ from 100||yes::There is evidence of a difference in IQ from 100"
    correct_answer="yes"
    solution_text="Yes, since for this case $p=.000116 \lt 0.05$, thre is evidence of a difference from 100."
%}

{% include question_dropdown.html
    id="ttestq10"
    title="10"
    question_text="Given that there was a difference of 5 in both studies and the standard deviation of the two samples were both 7.6, why do you think that the p-value was smaller in the second study?"
    solution_text="The sample size, n, in the second case is bigger"
%}

---

<div class="explanation" markdown="1">

## Independent-samples T-test

T-tests can also be used to determine whether there is evidence of a difference between two groups.  

For example, you may be looking to see if there is a difference in a mobility score between a group that received treatment and a group that did not receive treatment.  Again, you are looking for p-values to be lower than a value (typically 0.05) to say there is evidence of a difference.

### t-statistic

For an independent-samples t-test:

$$t=\frac{\bar{x}_1 - \bar{x}_2}{\text{SE of difference}}$$

Where $\bar{x}_1$ and $\bar{x}_2$ are the sample means of groups 1 and 2.

### Degrees of Freedom

For an independent-samples t-test:

$$\text{df}=n_1+n_2-2$$

Where $n_1$ and $n_2$ are the sample sizes of groups 1 and 2.

</div>

A treatment group and a control group are compared on systolic blood pressure levels.  There are 20 patients in both groups.

Mean (treatment) = 109

Mean (control) = 122

{% include question_numerical.html
id="ttestq11"
title="11"
question_text="Calculate the number of degrees of freedom"
correct_answer="38"
tolerance="0"
solution_text="$20+20-2=38$"
%}

{% include question_numerical.html
id="ttestq12"
title="12"
question_text="Calculate the difference between the two sample means"
correct_answer="13"
tolerance="0"
solution_text="$122-109=13$"
%}

It is found that

$$t = 2.03, p=.0493$$

{% include question_multiple_choice.html
    id="ttestq13"
    title="13"
    question_text="Given the information above, is there evidence of a difference in blood pressures between the control and the treatment groups?"
    options="no::Not enough evidence of a difference in IQ from 100||yes::There is evidence of a difference in IQ from 100"
    correct_answer="yes"
    solution_text="Yes, since for this case $p=.0493 \lt 0.05$, there is evidence of a difference between the two groups, at the 5% level."
%}
