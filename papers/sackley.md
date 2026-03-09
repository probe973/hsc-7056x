---
layout: default
title: Reading Statistics in Papers - Sackley et al.
---

<div class="explanation" markdown="1">
# Workshop: Reading Statistics in Papers
## Example from Sackley et al. (2016)

This workshop uses data from the research paper: *“An occupational therapy intervention for residents with stroke related disabilities in UK care homes (OTCH): cluster randomised controlled trial”* by Sackley et al. 
</div>

---

### Section 1: Baseline Characteristics (Table 1)

<table class="table table-bordered">
  <caption>Table 1: Details of clusters and personal and baseline assessment information for participants. Values are numbers (percentages) unless stated otherwise.</caption>
  <thead>
    <tr>
      <th scope="col">Characteristics</th>
      <th scope="col">Intervention group</th>
      <th scope="col">Control group</th>
    </tr>
  </thead>
  <tbody>
    <tr><th scope="row" colspan="3" style="background-color: #f2f2f2;">Care home type</th></tr>
    <tr>
      <th scope="row">Residential care</th>
      <td aria-label="Residential care, Intervention: 53 out of 114, 46 percent">53/114 (46)</td>
      <td aria-label="Residential care, Control: 54 out of 114, 47 percent">54/114 (47)</td>
    </tr>
    <tr>
      <th scope="row">Nursing care</th>
      <td aria-label="Nursing care, Intervention: 61 out of 114, 54 percent">61/114 (54)</td>
      <td aria-label="Nursing care, Control: 60 out of 114, 53 percent">60/114 (53)</td>
    </tr>
    <tr>
      <th scope="row">Mean (SD) cluster size</th>
      <td aria-label="Mean cluster size, Intervention: 5, Standard Deviation: 3.7">5 (3.7)</td>
      <td aria-label="Mean cluster size, Control: 4.2, Standard Deviation: 3.0">4.2 (3.0)</td>
    </tr>
    <tr><th scope="row" colspan="3" style="background-color: #f2f2f2;">Personal details</th></tr>
    <tr>
      <th scope="row">Mean (SD) age (years)</th>
      <td aria-label="Mean age, Intervention: 83.1 years, Standard Deviation: 9.9">83.1 (9.9)</td>
      <td aria-label="Mean age, Control: 83.6 years, Standard Deviation: 9.5">83.6 (9.5)</td>
    </tr>
    <tr>
      <th scope="row">Men</th>
      <td aria-label="Men, Intervention: 203 out of 568, 36 percent">203/568 (36)</td>
      <td aria-label="Men, Control: 174 out of 474, 37 percent">174/474 (37)</td>
    </tr>
    <tr>
      <th scope="row">White</th>
      <td aria-label="White ethnicity, Intervention: 517 out of 568, 91 percent">517/568 (91)</td>
      <td aria-label="White ethnicity, Control: 445 out of 474, 94 percent">445/474 (94)</td>
    </tr>
    <tr><th scope="row" colspan="3" style="background-color: #f2f2f2;">Comorbidities</th></tr>
    <tr>
      <th scope="row">Cardiovascular disease</th>
      <td aria-label="Cardiovascular disease, Intervention: 342 out of 530, 65 percent">342/530 (65)</td>
      <td aria-label="Cardiovascular disease, Control: 278 out of 446, 62 percent">278/446 (62)</td>
    </tr>
    <tr>
      <th scope="row">Fall history</th>
      <td aria-label="Fall history, Intervention: 203 out of 495, 41 percent">203/495 (41)</td>
      <td aria-label="Fall history, Control: 200 out of 427, 47 percent">200/427 (47)</td>
    </tr>
  </tbody>
</table>

<p style="font-size: 0.9em; margin-top: -10px;">
*Sheffield screening test for acquired language disorders.<br>
†EuroQol group 5-dimension self report questionnaire (three levels).
</p>

{% include question_multiple_choice.html
    id="s_q1"
    title="1"
    question_text="Look at the values in brackets across Table 1. Do they always represent the same thing?"
    options="no_var::No; they represent percentages for 'Care home type' but Standard Deviations (SD) for 'Age'.||yes_perc::Yes; they always represent the percentage of the group.||no_se::No; they represent Standard Errors in all rows."
    correct_answer="no_var"
    solution_text="In rows like 'Residential care', the brackets show percentages. In rows labeled 'Mean (SD)', they represent the Standard Deviation."
%}

{% include question_numerical.html
    id="s_q2"
    title="2"
    question_text="What was the **mean age** for the participants in the control group?"
    correct_answer="83.6"
    tolerance="0"
    solution_text="Look at 'Mean (SD) age' in the Control group column: 83.6."
%}

{% include question_numerical.html
    id="s_q3"
    title="3"
    question_text="What was the **standard deviation** of age for the participants in the control group?"
    correct_answer="9.5"
    tolerance="0"
    solution_text="The value in brackets for age in the control group is 9.5."
%}

{% include question_numerical.html
    id="s_q4"
    title="4"
    question_text="What **percentage** of the intervention group had cardiovascular disease?"
    correct_answer="65"
    tolerance="0"
    solution_text="For cardiovascular disease in the intervention group, the brackets show (65)."
%}

{% include question_numerical.html
    id="s_q5"
    title="5"
    question_text="What **percentage** of the intervention group had **not** had a fall history?"
    correct_answer="59"
    tolerance="0"
    solution_text="The table shows 41% had a fall history. Therefore, 100% - 41% = 59% had not."
%}

{% include question_multiple_choice.html
    id="s_q6"
    title="6"
    question_text="From the descriptive statistics in Table 1 alone, do the two groups seem similar at baseline?"
    options="yes_sim::Yes; the means and percentages for age, gender, and comorbidities are very close across both groups.||no_diff::No; the intervention group is significantly older than the control group.||no_gender::No; there is a major imbalance in the number of men between groups."
    correct_answer="yes_sim"
    solution_text="The baseline characteristics are very similar, which indicates successful randomization."
%}

---

### Section 2: Outcomes and Follow-up (Table 4)

<table class="table table-bordered">
  <caption>Table 4 - Comparison of primary and secondary outcomes at six and 12 month follow-up assessment</caption>
  <thead>
    <tr>
      <th scope="col">Outcome by follow-up</th>
      <th scope="col">Intervention Adj. Mean (SE)</th>
      <th scope="col">Intervention (No)</th>
      <th scope="col">Control Adj. Mean (SE)</th>
      <th scope="col">Control (No)</th>
      <th scope="col">Difference in adj. means (95% CI)</th>
      <th scope="col">P value</th>
    </tr>
  </thead>
  <tbody>
    <tr><th scope="row" colspan="7" style="background-color: #f2f2f2;">Barthel index‡</th></tr>
    <tr>
      <th scope="row">6 months</th>
      <td aria-label="Intervention, 6 months Barthel: 4.78, Standard Error: 0.20">4.78 (0.20)</td>
      <td>525</td>
      <td aria-label="Control, 6 months Barthel: 4.78, Standard Error: 0.22">4.78 (0.22)</td>
      <td>448</td>
      <td aria-label="Difference: 0.004, CI: -0.52 to 0.53">0.004 (−0.52 to 0.53)</td>
      <td>0.99</td>
    </tr>
    <tr>
      <th scope="row">12 months</th>
      <td aria-label="Intervention, 12 months Barthel: 3.93, Standard Error: 0.21">3.93 (0.21)</td>
      <td>512</td>
      <td aria-label="Control, 12 months Barthel: 3.77, Standard Error: 0.22">3.77 (0.22)</td>
      <td>430</td>
      <td aria-label="Difference: 0.16, CI: -0.40 to 0.72">0.16 (−0.40 to 0.72)</td>
      <td>0.58</td>
    </tr>
    <tr><th scope="row" colspan="7" style="background-color: #f2f2f2;">Rivermead mobility index</th></tr>
    <tr>
      <th scope="row">6 months</th>
      <td aria-label="Intervention, 6 months Rivermead: 2.64, SE: 0.11">2.64 (0.11)</td>
      <td>421</td>
      <td aria-label="Control, 6 months Rivermead: 2.67, SE: 0.12">2.67 (0.12)</td>
      <td>346</td>
      <td>−0.03 (−0.33 to 0.27)</td>
      <td>0.84</td>
    </tr>
    <tr>
      <th scope="row">12 months</th>
      <td aria-label="Intervention, 12 months Rivermead: 2.19, SE: 0.13">2.19 (0.13)</td>
      <td>354</td>
      <td aria-label="Control, 12 months Rivermead: 2.46, SE: 0.14">2.46 (0.14)</td>
      <td>271</td>
      <td>−0.26 (−0.62 to 0.09)</td>
      <td>0.15</td>
    </tr>
    <tr><th scope="row" colspan="7" style="background-color: #f2f2f2;">Geriatric depression scale-15</th></tr>
    <tr>
      <th scope="row">6 months</th>
      <td aria-label="Intervention, 6 months Depression: 6.20, SE: 0.21">6.20 (0.21)</td>
      <td>338</td>
      <td aria-label="Control, 6 months Depression: 6.68, SE: 0.22">6.68 (0.22)</td>
      <td>284</td>
      <td>−0.48 (−1.04 to 0.09)</td>
      <td>0.10</td>
    </tr>
    <tr>
      <th scope="row">12 months</th>
      <td aria-label="Intervention, 12 months Depression: 6.22, SE: 0.22">6.22 (0.22)</td>
      <td>297</td>
      <td aria-label="Control, 12 months Depression: 6.40, SE: 0.25">6.40 (0.25)</td>
      <td>219</td>
      <td>−0.18 (−0.80 to 0.43)</td>
      <td>0.56</td>
    </tr>
    <tr><th scope="row" colspan="7" style="background-color: #f2f2f2;">EQ-5D-3L§</th></tr>
    <tr>
      <th scope="row">6 months</th>
      <td aria-label="Intervention, 6 months EQ5D: 0.22, SE: 0.02">0.22 (0.02)</td>
      <td>363</td>
      <td aria-label="Control, 6 months EQ5D: 0.23, SE: 0.02">0.23 (0.02)</td>
      <td>315</td>
      <td>−0.01 (−0.05 to 0.04)</td>
      <td>0.72</td>
    </tr>
    <tr>
      <th scope="row">12 months</th>
      <td aria-label="Intervention, 12 months EQ5D: 0.20, SE: 0.02">0.20 (0.02)</td>
      <td>316</td>
      <td aria-label="Control, 12 months EQ5D: 0.18, SE: 0.02">0.18 (0.02)</td>
      <td>244</td>
      <td>0.02 (−0.03 to 0.07)</td>
      <td>0.48</td>
    </tr>
  </tbody>
</table>

<p style="font-size: 0.9em; margin-top: -10px;">
*Adjusted by care home as a random effect, and baseline score, type of care home and centre as fixed effects.<br>
†Tukey-Kramer adjusted confidence intervals and P values.<br>
‡Participants who died before follow-up are given a Barthel score of zero.<br>
§EuroQol group 5-dimension self report questionnaire (three levels).
</p>

Considering the results for the **Barthel Index**

{% include question_multiple_choice.html
    id="s_q7"
    title="7"
    question_text="For the Barthel index after 6 months, what is the **adjusted mean** for the control group and intervention group?"
    options="both_478::They are both 4.78.||int_393::Intervention: 3.93, Control: 3.77.||int_478::Intervention: 4.78, Control: 4.22."
    correct_answer="both_478"
    solution_text="At 6 months, both groups have an adjusted mean of 4.78."
%}

{% include question_multiple_choice.html
    id="s_q8"
    title="8"
    question_text="In Table 4, what does the number in the bracket after the mean represent?"
    options="sd::Standard Deviation (SD)||se::Standard Error (SE)||perc::Percentage (%)"
    correct_answer="se"
    solution_text="The column headers in Table 4 label this as 'Adjusted mean (SE)'."
%}

{% include question_numerical.html
    id="s_q9"
    title="9"
    question_text="What was the **difference in adjusted means** between the intervention and control groups at 6 months?"
    correct_answer="0.004"
    tolerance="0"
    solution_text="The 'Difference in adjusted means' column for 6 months shows 0.004."
%}

{% include question_multiple_choice.html
    id="s_q10"
    title="10"
    question_text="What was the **95% confidence interval** for the difference in adjusted means at 6 months?"
    options="ci_6::−0.52 to 0.53||ci_12::−0.40 to 0.72||ci_se::0.20 to 0.22"
    correct_answer="ci_6"
    solution_text="The value in brackets next to 0.004 is (−0.52 to 0.53)."
%}

{% include question_multiple_choice.html
    id="s_q11"
    title="11"
    question_text="Was the value of ‘0’ (representing no difference) within the 95% confidence interval for the difference in adjusted means?"
    options="no_out::No; the interval is entirely above zero.||yes_in::Yes; the interval ranges from -0.52 to 0.53.||yes_only::Yes; but only for the intervention group."
    correct_answer="yes_in"
    solution_text="Because the range goes from a negative number to a positive number, it must pass through zero."
%}

{% include question_multiple_choice.html
    id="s_q12"
    title="12"
    question_text="Is there any evidence of a difference in the Barthel index between the control and intervention groups at 6 months?"
    options="yes_ev::Yes; the p-value is 0.05.||no_ev::No; the p-value is 0.99, which is much larger than 0.05.||no_ci::No; because the Mean Difference is exactly zero."
    correct_answer="no_ev"
    solution_text="A p-value of 0.99 indicates no statistically significant difference."
%}

{% include question_multiple_choice.html
    id="s_q13"
    title="13"
    question_text="Do any of the 6-month or 12-month comparisons (Barthel, Mobility, Depression, EQ-5D) show evidence of a difference?"
    options="none_sig::No; every p-value in Table 4 is greater than 0.05.||some_sig::Yes; the Mobility index at 12 months is significant.||all_sig::Yes; all results are significant at 12 months."
    correct_answer="none_sig"
    solution_text="Scanning the 'P value' column, all values (0.99, 0.58, 0.84, 0.15, 0.10, 0.56, 0.72, 0.48) are above 0.05."
%}


{% include question_multiple_choice.html
    id="s_q14"
    title="14"
    question_text="Look at footnote ‡ for Table 4. Why did the researchers give participants who died a Barthel score of zero?"
    options="opt1::To ensure that the 'worst' outcome (death) is reflected in the functional score.||opt2::To make the average scores look higher than they actually were.||opt3::Because a score of zero is required by the Tukey-Kramer adjustment."
    correct_answer="opt1"
    solution_text="In stroke trials, giving a '0' for death prevents the results from looking better just because the frailest people died and were removed from the average."
%}

{% include question_multiple_choice.html
    id="s_q15"
    title="15"
    question_text="In Table 4, the difference for the Rivermead mobility index at 12 months is **-0.26**. Based on how these differences are usually calculated (Intervention minus Control), what does the negative sign indicate?"
    options="opt1::The intervention group had a slightly higher mean score.||opt2::The control group had a slightly higher mean score.||opt3::The result is statistically significant."
    correct_answer="opt2"
    solution_text="A negative difference means the Control group's mean was higher than the Intervention group's mean."
%}

{% include question_multiple_choice.html
    id="s_q16"
    title="16"
    question_text="The Barthel index is a 20-point scale. If a study found a difference between groups that was statistically significant ($p < 0.05$) but only 0.004 points, how should a clinician react?"
    options="opt1::Adopt the intervention immediately based on the p-value.||opt2::Recognize that while statistically significant, the effect size is likely too small to be clinically meaningful to a patient.||opt3::Ignore the result because p-values are invalid when the mean difference is small."
    correct_answer="opt2"
    solution_text="This highlights the difference between statistical significance and clinical significance (the 'size' of the effect)."
%}
