---
layout: default
title: Risk and Odds Workshop
---

<div class="explanation" markdown="1">
# Workshop: Risk and Odds

This workshop focuses on understanding how to quantify the likelihood of an event occurring using two different measures: **Risk** and **Odds**. We will also look at how to compare these measures between groups using **Ratios**.
</div>

---

<div class="explanation" markdown="1">
## Risk and Relative Risk (RR)

**Risk** is the number of people who experience an event divided by the total number of people in that group.

$$\text{Risk} = \frac{\text{Number of events}}{\text{Total number in group}}$$

**Relative Risk (RR)** is used to compare the risk in two different groups (usually an "exposed" or "intervention" group vs. a "control" group).

$$\text{Relative Risk} = \frac{\text{Risk in intervention group}}{\text{Risk in control group}}$$

*   **RR = 1**: The risk is the same in both groups.
*   **RR > 1**: The risk is higher in the intervention group.
*   **RR < 1**: The risk is lower in the intervention group.
</div>

### Question 1: Clinical Trial Data

400 people were recruited into a study regarding "sweaty palms." 160 people were given a **New Treatment**, and 240 people continued with the **Standard Treatment**. 

*   In the New Treatment group, 50 had an attack of sweaty palms.
*   In the Standard Treatment group, 120 had an attack of sweaty palms.

{% capture risk_table %}
<table class="table table-bordered">
  <thead>
    <tr>
      <th scope="col">Group</th>
      <th scope="col">Sweaty Palms</th>
      <th scope="col">No Sweaty Palms</th>
      <th scope="col">Total</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>New Treatment</td>
      <td><input type="number" step="any" aria-label="New treatment sweaty palms count"></td>
      <td><input type="number" step="any" aria-label="New treatment non-sweaty palms count"></td>
      <td><input type="number" step="any" aria-label="New treatment total count"></td>
    </tr>
    <tr>
      <td>Standard Treatment</td>
      <td><input type="number" step="any" aria-label="Standard treatment sweaty palms count"></td>
      <td><input type="number" step="any" aria-label="Standard treatment non-sweaty palms count"></td>
      <td><input type="number" step="any" aria-label="Standard treatment total count"></td>
    </tr>
  </tbody>
</table>
{% endcapture %}

{% include table_fill.html 
   id="risk_q1" 
   title="1a"
   question_text="Complete the table based on the information provided above:"
   table_content=risk_table
   answers="50 || 110 || 160 || 120 || 120 || 240"
   tolerance="0" 
   solution_text="New Treatment: 50 sweaty / 160 total = 110 non-sweaty. Standard Treatment: 120 sweaty / 240 total = 120 non-sweaty."
%}

{% include question_numerical.html
    id="risk_calc_1"
    title="1b: Calculate Risk"
    question_text="Calculate the **risk** of sweaty palms for the New Treatment group (as a decimal)."
    correct_answer="0.3125"
    tolerance="0.005"
    solution_text="$\text{Risk} = 50 / 160 = 0.3125$"
%}

{% include question_numerical.html
    id="risk_calc_2"
    title="1c: Calculate Relative Risk"
    question_text="Calculate the **Relative Risk (RR)** of the New Treatment compared to the Standard Treatment."
    correct_answer="0.625"
    tolerance="0.005"
    solution_text="$\text{Standard Risk} = 120 / 240 = 0.5$. <br> $\text{RR} = 0.3125 / 0.5 = 0.625$."
%}

{% include question_multiple_choice.html
    id="risk_calc_1d"
    title="1d Interpret"
    question_text="How would you interpret the risk of sweaty palms in the new treatment compared to the standard treatment?"
    options="w1::There is no difference in risk||w2::There is an increased risk in the new treatment group ||c::There is a decreased risk in the new treatment group"
    correct_answer="c"
    solution_text="RR<1, so reduced risk"
%}

---

<div class="explanation" markdown="1">
## Odds and Odds Ratio (OR)

While Risk compares the number of events to the *total* group, **Odds** compare the number of events to the number of *non-events*.

$$\text{Odds} = \frac{\text{Number of events}}{\text{Number of non-events}}$$

In a **retrospective case-control study**, we start with people who already have a condition (cases) and look back. In these studies, we often don't know the total population at risk, so we cannot calculate Risk. Instead, we use the **Odds Ratio (OR)**.

$$\text{Odds Ratio} = \frac{\text{Odds of exposure in cases}}{\text{Odds of exposure in controls}}$$

</div>

### Question 2: Retrospective Study (Bungee Jumping)

320 people with **ruptured nodules** (cases) were investigated; 64 had been exposed to a cold bungee rope. 360 people **without** nodules (controls) were investigated; 40 had been exposed.

| | Ruptured (Cases) | No Rupture (Controls) |
| :--- | :--- | :--- |
| **Exposed** | 64 | 40 |
| **Not Exposed** | 256 | 320 |

{% include question_dropdown.html
    id="odds_q2a"
    title="2a: Show your work"
    question_text="The odds of exposure in the ruptured group is 0.25. Which calculation correctly shows how this value is reached?"
    solution_text="Odds is Events (64) divided by Non-events (256). $64 / 256 = 0.25$."
%}

{% include question_numerical.html
    id="odds_q2b"
    title="2b: Calculate control odds"
    question_text="Calculate the **odds** of exposure in the group where ruptured nodules **did not** occur (the controls)."
    correct_answer="0.125"
    tolerance="0"
    solution_text="For the controls: $40 / 320 = 0.125$."
%}

{% include question_numerical.html
    id="odds_q2c"
    title="2c: Calculate the Odds Ratio"
    question_text="Calculate the **Odds Ratio (OR)** for exposure in the Ruptured group compared to the No Rupture group."
    correct_answer="2.0"
    tolerance="0"
    solution_text="$\text{OR} = 0.25 / 0.125 = 2.0$."
%}

{% include question_dropdown.html
    id="odds_q2d"
    title="2d: Interpretation"
    question_text="How would you interpret this odds ratio?"
    solution_text="The odds of having been exposed to a cold bungee are 2 times higher for those with ruptured nodules compared to those without."
%}

---

<div class="explanation" markdown="1">
## Odds Ratios in Regression

In medical research papers, you will often see Odds Ratios reported from "Multivariate Regression Models." These models tell us the odds of an outcome occurring based on several different factors at once.

*   **OR > 1**: The factor increases the odds of the outcome.
*   **OR < 1**: The factor decreases the odds of the outcome.
*   **P-value < 0.05**: The result is considered statistically significant.
*   **95% Confidence Interval (CI)**: If the range **includes 1.0**, the result is usually **not** significant.
</div>

### Question 3: Interpreting Regression Results

The following table includes all factors from a study on **delayed discharge**.

<table class="table table-bordered">
  <thead>
    <tr>
      <th scope="col">Factor</th>
      <th scope="col">P</th>
      <th scope="col">OR</th>
      <th scope="col">95% CI for OR</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Discharge EMS &ge; 14</td><td>0.075</td><td>0.72</td><td>0.50 – 1.03</td></tr>
    <tr><td>CFS &ge; 5</td><td>0.009</td><td>1.74</td><td>1.15 – 2.63</td></tr>
    <tr><td>Delirium</td><td>0.008</td><td>1.79</td><td>1.17 – 2.74</td></tr>
    <tr><td>Lives Alone</td><td>&lt;0.001</td><td>1.98</td><td>1.40 – 2.81</td></tr>
    <tr><td>New Institutionalization</td><td>&lt;0.001</td><td>2.78</td><td>1.67 – 4.62</td></tr>
    <tr><td>New Package of Care</td><td>&lt;0.001</td><td>4.05</td><td>2.68 – 6.10</td></tr>
  </tbody>
</table>

{% include question_dropdown.html
    id="reg_q3a"
    title="3a"
    question_text="Based on the table, are there higher or lower odds of a delayed discharge if the patient has a discharge EMS of 14 or greater? Is this significant at the 5% level?"
    solution_text="The OR is 0.72 (lower odds), and the p-value is 0.075 (not significant at the 5% level)."
%}

{% include question_dropdown.html
    id="reg_q3b"
    title="3b"
    question_text="Does the 95% Confidence Interval for the EMS variable concur with the significance result found in Question 3a?"
    solution_text="Yes. The interval 0.50 to 1.03 includes 1.0, meaning the result is not statistically significant."
%}

{% include question_numerical.html
    id="reg_q3c"
    title="3c"
    question_text="Approximately how many times **higher** are the odds of being delayed in discharge if the patient lives alone?"
    correct_answer="1.98"
    tolerance="0.02"
    solution_text="The OR for 'Lives Alone' is 1.98, which is nearly double the odds."
%}
