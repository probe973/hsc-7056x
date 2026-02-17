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
    solution_text="The researchers 'collapsed' the categories into two named groups: disagreement vs. agreement. This makes the data **Nominal**."
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
    question_text="The training status of the students (trained vs. untrained) as used in an independent samples t-test to split the groups."
    options="ord::Ordinal||nom::Nominal||int::Interval/Ratio"
    correct_answer="nom"
    solution_text="The grouping variable (trained vs. untrained) is **Nominal**."
%}

---

### Section 2: Demographic Data (Table 1)

<table class="table table-bordered">
  <caption>Table 1: Distribution of the sample by demographic variables (n = 241)</caption>
  <thead>
    <tr>
      <th scope="col">Variables</th>
      <th scope="col">n (%)</th>
    </tr>
  </thead>
  <tbody>
    <tr><th scope="row" colspan="2" style="background-color: #f2f2f2;">Gender</th></tr>
    <tr><td>Male</td><td aria-label="Male participants: 64, which is 26.6 percent">64 (26.6%)</td></tr>
    <tr><td>Female</td><td aria-label="Female participants: 177, which is 73.4 percent">177 (73.4%)</td></tr>
    <tr><th scope="row" colspan="2" style="background-color: #f2f2f2;">Educational level</th></tr>
    <tr><td>Third-year</td><td aria-label="Third-year students: 36, which is 14.9 percent">36 (14.9%)</td></tr>
    <tr><td>Fourth-year</td><td aria-label="Fourth-year students: 205, which is 85.1 percent">205 (85.1%)</td></tr>
    <tr><th scope="row" colspan="2" style="background-color: #f2f2f2;">University</th></tr>
    <tr><td>University A</td><td aria-label="University A students: 123, which is 51 percent">123 (51%)</td></tr>
    <tr><td>University B</td><td aria-label="University B students: 118, which is 49 percent">118 (49%)</td></tr>
    <tr><th scope="row" colspan="2" style="background-color: #f2f2f2;">EBP training</th></tr>
    <tr><td>Yes</td><td aria-label="Trained students: 163, which is 67.6 percent">163 (67.6%)</td></tr>
    <tr><td>No</td><td aria-label="Untrained students: 78, which is 32.4 percent">78 (32.4%)</td></tr>
    <tr><th scope="row">Total</th><td aria-label="Total sample: 241 participants, 100 percent">241 (100%)</td></tr>
  </tbody>
</table>

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
    solution_text="According to the table, 163 students (67.6%) had received training."
%}

{% include question_multiple_choice.html
    id="q2c"
    title="2c"
    question_text="Approximately how many female participants were there for every male participant in this study?"
    options="opt1::1.5 females for every male||opt2::1 female for every 3 males||opt3::2.76 females for every male"
    correct_answer="opt3"
    solution_text="Divide the number of females (177) by the number of males (64). $177 / 64 \approx 2.76$."
%}

---

### Section 3: Agreement and Negative Wording (Table 2)

<table class="table table-bordered">
  <caption>Table 2: Responses to evidence-based practice belief scale by trained and untrained students (n = 241)</caption>
  <thead>
    <tr>
      <th scope="col">Your agreement to each statement:</th>
      <th scope="col">All students (n=241) n (%)</th>
      <th scope="col">Trained (n=163) n (%)</th>
      <th scope="col">Untrained (n=78) n (%)</th>
      <th scope="col">χ²</th>
      <th scope="col">p</th>
    </tr>
  </thead>
  <tbody>
    <tr><th scope="row">1. "I believe that EBP results in the best clinical care for patients".</th><td aria-label="All students: 177 (73.4%)">177 (73.4%)</td><td aria-label="Trained: 127 (77.9%)">127 (77.9%)</td><td aria-label="Untrained: 50 (64.1%)">50 (64.1%)</td><td>5.160</td><td>.023</td></tr>
    <tr><th scope="row">2. "I am sure that evidence-based guidelines can improve clinical care".</th><td aria-label="All students: 174 (72.2%)">174 (72.2%)</td><td aria-label="Trained: 121 (74.2%)">121 (74.2%)</td><td aria-label="Untrained: 53 (67.9%)">53 (67.9%)</td><td>1.038</td><td>.308</td></tr>
    <tr><th scope="row">3. "I am sure that implementing EBP will improve the care that I deliver to my patients".</th><td aria-label="All students: 167 (69.3%)">167 (69.3%)</td><td aria-label="Trained: 115 (70.6%)">115 (70.6%)</td><td aria-label="Untrained: 52 (66.7%)">52 (66.7%)</td><td>.374</td><td>.541</td></tr>
    <tr><th scope="row">4. "I believe that critically appraising evidence is an important step in the EBP process".</th><td aria-label="All students: 153 (63.5%)">153 (63.5%)</td><td aria-label="Trained: 107 (65.6%)">107 (65.6%)</td><td aria-label="Untrained: 46 (59.0%)">46 (59.0%)</td><td>1.012</td><td>.314</td></tr>
    <tr><th scope="row">5. "I believe the care that I deliver is evidence-based".</th><td aria-label="All students: 148 (61.4%)">148 (61.4%)</td><td aria-label="Trained: 102 (62.6%)">102 (62.6%)</td><td aria-label="Untrained: 46 (59.0%)">46 (59.0%)</td><td>.289</td><td>.591</td></tr>
    <tr><th scope="row">6. "I am sure about how to measure the outcomes of clinical care".</th><td aria-label="All students: 152 (63.1%)">152 (63.1%)</td><td aria-label="Trained: 109 (66.9%)">109 (66.9%)</td><td aria-label="Untrained: 43 (55.1%)">43 (55.1%)</td><td>3.123</td><td>.077</td></tr>
    <tr><th scope="row">7. "I am sure that I can implement EBP".</th><td aria-label="All students: 131 (54.4%)">131 (54.4%)</td><td aria-label="Trained: 99 (60.7%)">99 (60.7%)</td><td aria-label="Untrained: 32 (41.0%)">32 (41.0%)</td><td>8.261</td><td>.004</td></tr>
    <tr><th scope="row">8. "I am clear about the steps of EBP".</th><td aria-label="All students: 127 (52.7%)">127 (52.7%)</td><td aria-label="Trained: 95 (58.3%)">95 (58.3%)</td><td aria-label="Untrained: 32 (41.0%)">32 (41.0%)</td><td>6.302</td><td>.021</td></tr>
    <tr><th scope="row">9. "I believe that I can search for the best evidence to answer clinical questions in a time-efficient way".</th><td aria-label="All students: 144 (59.8%)">144 (59.8%)</td><td aria-label="Trained: 101 (62.0%)">101 (62.0%)</td><td aria-label="Untrained: 43 (55.1%)">43 (55.1%)</td><td>1.025</td><td>.311</td></tr>
    <tr><th scope="row">10. "I believe that I can overcome barriers in implementing EBP".</th><td aria-label="All students: 124 (51.5%)">124 (51.5%)</td><td aria-label="Trained: 87 (53.4%)">87 (53.4%)</td><td aria-label="Untrained: 37 (47.4%)">37 (47.4%)</td><td>.745</td><td>.388</td></tr>
    <tr><th scope="row">11. "I believe that EBP takes too much time".</th><td aria-label="All students: 125 (51.9%)">125 (51.9%)</td><td aria-label="Trained: 80 (49.1%)">80 (49.1%)</td><td aria-label="Untrained: 45 (57.7%)">45 (57.7%)</td><td>1.567</td><td>.211</td></tr>
    <tr><th scope="row">12. "I am sure that I can access the best resources in order to implement EBP".</th><td aria-label="All students: 121 (50.5%)">121 (50.5%)</td><td aria-label="Trained: 83 (50.9%)">83 (50.9%)</td><td aria-label="Untrained: 38 (48.7%)">38 (48.7%)</td><td>.102</td><td>.749</td></tr>
    <tr><th scope="row">13. "I believe EBP is difficult".</th><td aria-label="All students: 142 (58.9%)">142 (58.9%)</td><td aria-label="Trained: 90 (55.2%)">90 (55.2%)</td><td aria-label="Untrained: 52 (66.7%)">52 (66.7%)</td><td>2.858</td><td>.091</td></tr>
    <tr><th scope="row">14. "I know how to implement EBP sufficiently enough to make practice changes".</th><td aria-label="All students: 128 (53.5%)">128 (53.5%)</td><td aria-label="Trained: 93 (57.1%)">93 (57.1%)</td><td aria-label="Untrained: 35 (44.9%)">35 (44.9%)</td><td>3.144</td><td>.076</td></tr>
    <tr><th scope="row">15. "I am confident about my ability to implement EBP where I work".</th><td aria-label="All students: 129 (53.5%)">129 (53.5%)</td><td aria-label="Trained: 96 (58.9%)">96 (58.9%)</td><td aria-label="Untrained: 33 (42.3%)">33 (42.3%)</td><td>5.836</td><td>.016</td></tr>
    <tr><th scope="row">16. "I am sure that I can implement EBP in a time-efficient way".</th><td aria-label="All students: 138 (57.3%)">138 (57.3%)</td><td aria-label="Trained: 99 (60.7%)">99 (60.7%)</td><td aria-label="Untrained: 39 (50.0%)">39 (50.0%)</td><td>2.485</td><td>.115</td></tr>
  </tbody>
</table>

**3.** Referring to Table 2:

{% include question_numerical.html
    id="q3a"
    title="3a"
    question_text="Identify the number of the statement shown above (1–16) that had the highest level of agreement when considering all students."
    correct_answer="1"
    tolerance="0"
    solution_text="Statement 1 has 73.4% agreement across all students."
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
    question_text="In almost every row of Table 2, the Trained group has higher agreement. However, for Statements 11 ('takes too much time') and 13 ('is difficult'), the **Untrained** group has higher agreement. How should a researcher interpret this?"
    options="opt1::It is a positive finding; the training successfully reduced the students' perception of these factors as barriers to EBP.||opt2::It is a negative finding; the training was unsuccessful because it failed to increase the level of agreement in the intervention group.||opt3::It is an inconsistent finding; the reversal of the trend suggests that these two statements are less reliable than the other items."
    correct_answer="opt1"
    solution_text="Statements 11 and 13 are **negatively worded**. Lower agreement in the trained group indicates a successful outcome (viewing EBP as less difficult/time-consuming)."
%}

---

### Section 4: Significance and Notation (Table 4)

<table class="table table-bordered">
  <caption>Table 4: Scores of beliefs and implementations</caption>
  <thead>
    <tr>
      <th scope="col">Variable</th>
      <th scope="col">Trained Mean (SD)</th>
      <th scope="col">Untrained Mean (SD)</th>
      <th scope="col">t</th>
      <th scope="col">df</th>
      <th scope="col">p</th>
      <th scope="col">Mean Diff</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Total score: beliefs</th>
      <td aria-label="Beliefs, Trained Mean: 55.55, Standard Deviation: 13.29">55.55 (13.29)</td>
      <td aria-label="Beliefs, Untrained Mean: 51.74, Standard Deviation: 14.06">51.74 (14.06)</td>
      <td aria-label="Beliefs, t-statistic: 2.04">2.04</td>
      <td aria-label="Degrees of freedom: 239">239</td>
      <td aria-label="Beliefs, p-value: .042">.042</td>
      <td aria-label="Beliefs, Mean difference: 3.80">3.80</td>
    </tr>
    <tr>
      <th scope="row">Total score: implementations</th>
      <td aria-label="Implementations, Trained Mean: 27.01, Standard Deviation: 12.61">27.01 (12.61)</td>
      <td aria-label="Implementations, Untrained Mean: 21.86, Standard Deviation: 11.14">21.86 (11.14)</td>
      <td aria-label="Implementations, t-statistic: 3.08">3.08</td>
      <td aria-label="Degrees of freedom: 239">239</td>
      <td aria-label="Implementations, p-value: .002">.002</td>
      <td aria-label="Implementations, Mean difference: 5.15">5.15</td>
    </tr>
  </tbody>
</table>

**4.** Referring to Table 4:

{% include question_multiple_choice.html
    id="q4a"
    title="4a"
    question_text="Identify the statistical test indicated by the column labeled **'t'** in Table 4. What is it being used for here?"
    options="opt1::Chi-square; comparing frequencies of agreement.||opt2::Independent samples t-test; comparing the mean scores of the two groups.||opt3::Pearson correlation; measuring the relationship between belief and implementation."
    correct_answer="opt2"
    solution_text="The 't' column indicates an independent samples t-test, which compares the average (mean) scores of two separate groups."
%}

{% include question_multiple_choice.html
    id="q4b"
    title="4b"
    question_text="Look at the row for 'Total score: beliefs.' Which of the following is the correct justification for whether the training made a significant difference?"
    options="opt1::Yes; the p-value (.042) is less than 0.05.||opt2::Yes; the t-value (2.04) is greater than 0.05.||opt3::No; the mean difference (3.80) is not large enough."
    correct_answer="opt1"
    solution_text="Statistical significance is determined by the p-value. Since $0.042 < 0.05$, the result is significant."
%}

{% include question_multiple_choice.html
    id="q4c"
    title="4c"
    question_text="Compare the results for 'Beliefs' ($p = .042$) and 'Implementations' ($p = .002$). Which statement accurately summarizes the results in Table 4?"
    options="opt1::Only the implementation scores showed a significant difference.||opt2::Neither result is significant at the 5% level.||opt3::The training had a significant positive effect on both student beliefs and implementation frequency."
    correct_answer="opt3"
    solution_text="Both p-values are less than 0.05, meaning both results are statistically significant."
%}
