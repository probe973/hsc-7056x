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

**Risk** is the same as probability. it is the number of people who experience an event divided by the total number of people in that group.

$$\text{Risk} = \frac{\text{Number of events}}{\text{Total number in group}}$$

**Relative Risk (RR)** is used to compare the risk in two different groups (usually an "exposed" or "intervention" group vs. a "control" group).

$$\text{Relative Risk} = \frac{\text{Risk in intervention group}}{\text{Risk in control group}}$$

*   **RR = 1**: The risk is the same in both groups.
*   **RR > 1**: The risk is higher in the intervention group.
*   **RR < 1**: The risk is lower in the intervention group (the treatment may be protective).
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
      <td><input type="number" step="any" aria-label="New Sweaty"></td>
      <td><input type="number" step="any" aria-label="New Non-Sweaty"></td>
      <td><input type="number" step="any" aria-label="New Total"></td>
    </tr>
    <tr>
      <td>Standard Treatment</td>
      <td><input type="number" step="any" aria-label="Old Sweaty"></td>
      <td><input type="number" step="any" aria-label="Old Non-Sweaty"></td>
      <td><input type="number" step="any" aria-label="Old Total"></td>
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

{% include question_numerical.html
    id="odds_q1"
    title="2a"
    question_text="Calculate the **odds** of exposure for the Ruptured group."
    correct_answer="0.25"
    tolerance="0"
    solution_text="$\text{Odds} = 64 / 256 = 0.25$."
%}

{% include question_numerical.html
    id="odds_q2"
    title="2b"
    question_text="Calculate the **Odds Ratio (OR)** for exposure in the Ruptured group compared to the No Rupture group."
    correct_answer="2.0"
    tolerance="0"
    solution_text="$\text{Control Odds} = 40 / 320 = 0.125$. <br> $\text{OR} = 0.25 / 0.125 = 2.0$."
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

The following table shows factors associated with **delayed discharge** in geriatric wards.

| Factor | OR | P-value | 95% CI |
| :--- | :--- | :--- | :--- |
| **Discharge EMS $\ge$ 14** | 0.72 | 0.075 | 0.50 – 1.03 |
| **Lives Alone** | 1.98 | <0.001 | 1.40 – 2.81 |

{% include question_multiple_choice.html
    id="reg_q1"
    title="3a"
    question_text="Is the 'EMS $\ge$ 14' factor a statistically significant predictor of delayed discharge at the 5% level?"
    options="no::No, because p > 0.05 and the CI includes 1.0||yes::Yes, because the OR is less than 1.0"
    correct_answer="no"
    solution_text="The p-value is 0.075 (greater than 0.05) and the Confidence Interval includes 1.0, so it is not significant."
%}

{% include question_dropdown.html
    id="reg_q2"
    title="3b"
    question_text="Interpret the Odds Ratio for 'Lives Alone'."
    solution_text="The OR is 1.98, which is approximately 2. This means patients who live alone have nearly double (2x) the odds of a delayed discharge compared to those who do not live alone. This result is highly significant (p < 0.001)."
%}
