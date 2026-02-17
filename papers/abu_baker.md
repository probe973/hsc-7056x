---
layout: default
title: Reading Statistics in Papers - Abu-Baker
---

<div class="explanation" markdown="1">
# Workshop: Reading Statistics in Papers
**Example from Abu-Baker et al. (2021)**

This workshop focuses on interpreting statistical methodology and results from a real research paper on Evidence-Based Practice (EBP). We will analyze how researchers choose their tests, read demographic data, and interpret clinical significance in tables.
</div>

---

### Section 1: Methodology and Data Types

#### **Extract: Data Analysis**
> Descriptive statistics (e.g., means, standard deviations, frequencies, and percentages) were performed to describe the demographic characteristics of the participating students and the main study variables. For the belief scale, the two agreement categories (4 = agree, 5 = strongly agree) were collapsed to one category to indicate a positive belief. For the implementation scale, the three categories (2 = 4–5 times, 3 = 6–8, and 4 ≥ 8 times in the past 8 weeks) were collapsed to one category as (≥ 4 times) to indicate frequent implementation. Pearson’s correlation test was used to determine the relationship between the total scores of the EBP belief and implementation scales. A chi-square test was used to examine the difference between trained and untrained students in terms of agreement toward each EBP belief (disagreement vs. agreement) and in terms of frequency of each EBP implementation (less than 4 times vs. 4 times or more in the past 8 weeks). Finally, an independent samples t-test was used to examine the difference between trained and untrained students in terms of the total mean scores of EBP beliefs.

**1.** The extract above describes how the researchers treated their data. Assuming the authors used the correct tests for their variables, identify the **level of measurement** (Nominal, Ordinal, or Interval/Ratio) for each of the following:

{% include question_multiple_choice.html
    id="q1a"
    title="1a"
    question_text="Student agreement toward EBP beliefs (categorized as disagreement vs. agreement)."
    options="ord::Ordinal||int::Interval/Ratio||nom::Nominal"
    correct_answer="nom"
    solution_text="The researchers 'collapsed' the categories into named groups: disagreement vs. agreement. This makes the data **Nominal**."
%}

{% include question_multiple_choice.html
    id="q1b"
    title="1b"
    question_text="The total scores of the EBP belief and implementation scales (analyzed using Pearson’s correlation)."
    options="int::Interval/Ratio||nom::Nominal||ord::Ordinal"
    correct_answer="int"
    solution_text="Total scores analyzed using Pearson's correlation require **Interval/Ratio** data."
%}

{% include question_multiple_choice.html
    id="q1c"
    title="1c"
    question_text="The training status of the students (trained vs. untrained) as used in an independent samples t-test."
    options="ord::Ordinal||nom::Nominal||int::Interval/Ratio"
    correct_answer="nom"
    solution_text="This is a grouping variable used to split the sample into two named categories, which is **Nominal** data."
%}

---

### Section 2: Demographic Data (Table 1)

**Table 1: Distribution of the sample by demographic variables (n = 241)**

| Variables | n (%) |
| :--- | :--- |
| **Gender** | |
| Male | 64 (26.6%) |
| Female | 177 (73.4%) |
| **Educational level** | |
| Third-year | 36 (14.9%) |
| Fourth-year | 205 (85.1%) |
| **University** | |
| University A | 123 (51%) |
| University B | 118 (49%) |
| **EBP training** | |
| Yes | 163 (67.6%) |
| No | 78 (32.4%) |
| **Total** | **241 (100%)** |

**2.** Referring to Table 1:

{% include question_numerical.html
    id="q2a"
    title="2a"
    question_text="How many subjects in total were part of this study?"
    correct_answer="241"
    tolerance="0"
    solution_text="The total sample size (n) is 241."
%}

{% include question_numerical.html
    id="q2b"
    title="2b"
    question_text="What percentage of the participants had received EBP training?"
    correct_answer="67.6"
    tolerance="0"
    solution_text="The table shows 163 students said 'Yes' to training, which is 67.6%."
%}

{% include question_multiple_choice.html
    id="q2c"
    title="2c"
    question_text="Approximately how many female participants were there for every male participant in this study?"
    options="opt1::1.5 females for every male||opt2::1 female for every 3 males||opt3::2.76 females for every male"
    correct_answer="opt3"
    solution_text="Divide females (177) by males (64). $177 / 64 \approx 2.76$."
%}

---

### Section 3: Agreement and Negative Wording (Table 2)

**Table 2: Responses to evidence-based practice belief scale (n = 241)**

| Your agreement to each statement: | All students n (%) | Trained n (%) | Untrained n (%) | $\chi^2$ | p |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1. EBP results in best clinical care | 177 (73.4%) | 127 (77.9%) | 50 (64.1%) | 5.160 | .023 |
| 7. I am sure I can implement EBP | 131 (54.4%) | 99 (60.7%) | 32 (41.0%) | 8.261 | .004 |
| 8. I am clear about the steps of EBP | 127 (52.7%) | 95 (58.3%) | 32 (41.0%) | 6.302 | .021 |
| 11. EBP takes too much time | 125 (51.9%) | 80 (49.1%) | 45 (57.7%) | 1.567 | .211 |
| 13. I believe EBP is difficult | 142 (58.9%) | 90 (55.2%) | 52 (66.7%) | 2.858 | .091 |
| 15. I am confident about my ability | 129 (53.5%) | 96 (58.9%) | 33 (42.3%) | 5.836 | .016 |

*(Note: Table 2 has been condensed to focus on key statements for this exercise)*

**3.** Referring to Table 2:

{% include question_numerical.html
    id="q3a"
    title="3a"
    question_text="Identify the number of the statement shown above that had the highest level of agreement when considering all students."
    correct_answer="1"
    tolerance="0"
    solution_text="Statement 1 has 73.4% agreement, the highest in the 'All students' column."
%}

{% include question_numerical.html
    id="q3b"
    title="3b"
    question_text="What is the **percentage points difference** between the trained and untrained students for Statement 1?"
    correct_answer="13.8"
    tolerance="0.1"
    solution_text="$77.9\% - 64.1\% = 13.8$ percentage points."
%}

{% include question_multiple_choice.html
    id="q3c"
    title="3c"
    question_text="In almost every row, the Trained group has higher agreement. However, for Statements 11 ('takes too much time') and 13 ('is difficult'), the **Untrained** group has higher agreement. How should a researcher interpret this?"
    options="opt1::It is a positive finding; the training successfully reduced the students' perception of these factors as barriers to EBP.||opt2::It is a negative finding; the training was unsuccessful because it failed to increase the level of agreement in the intervention group.||opt3::It is an inconsistent finding; the reversal of the trend suggests that these two statements are less reliable than the other items."
    correct_answer="opt1"
    solution_text="Statements 11 and 13 are **negatively worded**. Lower agreement in the trained group is the desired outcome, as it shows they see fewer barriers to EBP."
%}

---

### Section 4: Significance and Notation (Table 4)

**Table 4: Scores of beliefs and implementations**

| Variable | Trained Mean (SD) | Untrained Mean (SD) | t | df | p | Mean Diff |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Total score: beliefs | 55.55 (13.29) | 51.74 (14.06) | 2.04 | 239 | .042 | 3.80 |
| Total score: implementations | 27.01 (12.61) | 21.86 (11.14) | 3.08 | 239 | .002 | 5.15 |

**4.** Referring to Table 4:

{% include question_multiple_choice.html
    id="q4a"
    title="4a"
    question_text="Identify the statistical test indicated by the column labeled **'t'** in Table 4. What is it being used for here?"
    options="opt1::Chi-square; comparing frequencies of agreement.||opt2::Independent samples t-test; comparing the mean scores of the two groups.||opt3::Pearson correlation; measuring the relationship between belief and implementation."
    correct_answer="opt2"
    solution_text="The 't' indicates a t-test. It is comparing the average (mean) scores of the two independent groups."
%}

{% include question_multiple_choice.html
    id="q4b"
    title="4b"
    question_text="Look at the row for 'Total score: beliefs.' Which of the following is the correct justification for whether the training made a significant difference?"
    options="opt1::Yes; the p-value (.042) is less than 0.05.||opt2::Yes; the t-value (2.04) is greater than 0.05.||opt3::No; the mean difference (3.80) is not large enough."
    correct_answer="opt1"
    solution_text="Significance is determined by the p-value. Since $0.042 < 0.05$, the difference is statistically significant."
%}

{% include question_multiple_choice.html
    id="q4c"
    title="4c"
    question_text="Compare the results for 'Beliefs' ($p = .042$) and 'Implementations' ($p = .002$). Which statement accurately summarizes the results?"
    options="opt1::Only the implementation scores showed a significant difference.||opt2::Neither result is significant at the 5% level.||opt3::The training had a significant positive effect on both student beliefs and implementation frequency."
    correct_answer="opt3"
    solution_text="Both p-values are below 0.05, so both results are statistically significant."
%}
