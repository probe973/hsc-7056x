---
layout: default
title: Understanding Effect Sizes
---

<div class="explanation" markdown="1">

# Understanding Effect Sizes

This workshop focuses on the crucial concept of **effect sizes**, exploring what they represent, how they complement or differ from p-values, and why they are particularly important when dealing with studies that involve very large sample sizes.

## What is an Effect Size?

An **effect size** is a quantitative measure of the magnitude of a phenomenon. In simpler terms, it tells you *how much* of an effect there is. While a p-value helps determine if an effect exists (statistical significance), an effect size tells you about the *strength* or *practical importance* of that effect. It's a standardized way to quantify the difference between groups or the strength of a relationship between variables, making it understandable and comparable across different studies.

## Effect Sizes vs. P-values: What's the Difference?

*   **P-value:** The p-value indicates the probability of observing results as extreme as, or more extreme than, the observed results, assuming the null hypothesis (i.e., no effect or no difference) is true. A small p-value (e.g., typically less than 0.05) leads us to reject the null hypothesis, suggesting that the observed effect is statistically significant and likely not due to random chance. **Crucially, a p-value does NOT tell you about the size or importance of that effect.**

*   **Effect Size:** An effect size, on the other hand, quantifies the *magnitude* of the observed effect. It provides a measure that is independent of sample size and can be directly interpreted in terms of practical significance. For example, a "small" effect size might mean a subtle difference or relationship, while a "large" effect size indicates a prominent and impactful difference or relationship.

Think of it this way: A p-value answers the question, "Is there an effect?" An effect size answers, "How big is the effect?" Both pieces of information are vital for drawing complete and meaningful conclusions from research.

## The Pitfall of P-values with Large Sample Sizes

One of the most significant reasons why effect sizes are indispensable is the behavior of p-values in studies with very large sample sizes. As the sample size increases, the statistical power to detect even tiny, practically meaningless effects also increases.

*   **The Problem:** With a sufficiently large sample, even a minuscule difference or relationship, which has no real-world importance, can yield a statistically significant p-value (e.g., p < 0.001). This can lead researchers to mistakenly interpret a statistically significant finding as practically important.
*   **The Solution:** Effect sizes provide the necessary context. If a study with a massive sample size reports a very small p-value but also an extremely small effect size, it indicates that while an effect *statistically exists*, it is too trivial to be practically meaningful. Conversely, a large effect size, even with a moderately significant p-value, suggests a finding that is both detectable and important.

Therefore, always consider both the p-value and the effect size to fully understand the implications of research findings.

## Common Effect Size Measures and Their Interpretation

Different statistical tests use different effect size measures. Here are some commonly encountered ones and their general interpretation guidelines:

### 1. Cohen's d (for comparing two means)

**What it measures:** Cohen's d is a standardized measure of the difference between two means, expressed in standard deviation units. It's commonly used with t-tests.
**Interpretation Guidelines:**
*   **Small effect:** d = 0.2
*   **Medium effect:** d = 0.5
*   **Large effect:** d = 0.8
*   **Note:** These are general conventions, and what constitutes a "small," "medium," or "large" effect can vary by research field and specific context.

### 2. Partial Eta-squared (η²p) (for ANOVA)

**What it measures:** Partial Eta-squared represents the proportion of variance in the dependent variable that is explained by a specific independent variable, after accounting for other factors in the model. It's commonly used in ANOVA.
**Interpretation Guidelines:**
*   **Small effect:** η²p = 0.01 (1% of variance explained)
*   **Medium effect:** η²p = 0.06 (6% of variance explained)
*   **Large effect:** η²p = 0.14 (14% of variance explained)
*   **Note:** Like Cohen's d, these are general guidelines, and context is important.

### 3. Cramer's V (for Chi-square tests)

**What it measures:** Cramer's V is a measure of the strength of association between two nominal (categorical) variables. It ranges from 0 (no association) to 1 (perfect association). It's commonly used with chi-square tests of independence.
**Interpretation Guidelines:** The interpretation of Cramer's V depends on the degrees of freedom (df), which is determined by the number of rows and columns in the contingency table (df = min(number of rows - 1, number of columns - 1)).
*   **For df = 1 (e.g., a 2x2 table):**
    *   **Small effect:** V = 0.10
    *   **Medium effect:** V = 0.30
    *   **Large effect:** V = 0.50
*   **For df = 2 (e.g., a 2x3 or 3x3 table):**
    *   **Small effect:** V = 0.07
    *   **Medium effect:** V = 0.21
    *   **Large effect:** V = 0.35
*   **Note:** As the degrees of freedom increase, the thresholds for small, medium, and large effects tend to decrease. Always refer to the appropriate guidelines for your specific table dimensions.

</div>

---

### Memory Boost

A new memory training program has been developed, and researchers want to assess its effectiveness. They recruit a group of participants and measure their memory recall scores before the program and after completing a 6-week program. Higher scores indicate better memory recall.

A **paired-samples t-test** is performed, and **Cohen's d** is calculated as a measure of effect size.

| | N | Mean | SD | Mean Difference (After – Before) | 95% CI for Mean Difference | t | p | Cohen's d |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| Before Program | 80 | 25.4 | 4.8 | 2.1 | (1.1, 3.1) | 4.15 | < 0.001 | 0.46 |
| After Program | 80 | 27.5 | 5.1 | | | | | |

{% include question_multiple_choice.html
    id="effectsize1a_new"
    title="Study Design"
    question_text="Is this an example of a between-groups analysis or a within-groups analysis?"
    options="bg::Between-groups||wg::Within-groups"
    correct_answer="wg"
    solution_text="The same individuals are measured on two different occasions (before and after the program), making this a **within-groups** analysis."
%}

{% include question_dropdown.html
    id="effectsize1b_new"
    title="P-value Interpretation"
    question_text="Interpret the p-value given in the table."
    solution_text="The p-value of < 0.001 is very small (much less than 0.05). This indicates that the observed increase in memory recall scores is statistically significant, suggesting it is highly unlikely to have occurred by chance if the program had no effect."
%}

{% include question_dropdown.html
    id="effectsize1c_new"
    title="Cohen's d Interpretation"
    question_text="Interpret Cohen's d (0.46) for this study using the guidelines provided. What does it tell us about the program's effect?"
    solution_text="Cohen's d is a standardized measure of the mean difference. According to the guidelines, a Cohen's d of 0.2 is small, 0.5 is medium, and 0.8 is large. Our value of 0.46 falls between small and medium, indicating a **medium effect size**. This means the memory training program has a noticeable, moderate practical impact on improving memory recall."
%}

{% include question_dropdown.html
    id="effectsize1d_new"
    title="Overall Conclusion"
    question_text="Combining the p-value and Cohen's d, what can you conclude about the effectiveness of the memory training program?"
    solution_text="The p-value (< 0.001) confirms statistical significance, meaning the program likely has an effect. Cohen's d (0.46) indicates a medium effect size, suggesting this effect is also practically meaningful. Therefore, there is strong evidence that the memory training program is effective, and its impact on memory recall is of moderate importance."
%}

---

### Stress Reduction Therapy

A clinical trial is conducted to compare the effectiveness of three different stress reduction therapies (Therapy X, Therapy Y, and a control group receiving standard care). Participants are randomly assigned to one of the three groups, and their stress levels are measured after 8 weeks. Lower scores indicate lower stress.

An **Analysis of Variance (ANOVA)** is performed, and **Partial Eta-squared (η²p)** is calculated as a measure of effect size.

$$F(2, 147) = 3.89, p = 0.022, \eta^2_p = 0.05$$

{% include question_multiple_choice.html
    id="effectsize2a_new"
    title="Study Design"
    question_text="Is this an example of a between-groups analysis or a within-groups analysis?"
    options="bg::Between-groups||wg::Within-groups"
    correct_answer="bg"
    solution_text="Participants are divided into three distinct groups, with each participant only belonging to one group. This is a **between-groups** analysis."
%}

{% include question_dropdown.html
    id="effectsize2b_new"
    title="P-value Interpretation"
    question_text="Interpret the p-value given for the ANOVA."
    solution_text="The p-value of 0.022 is less than the standard significance level of 0.05. This indicates that there is a statistically significant difference in stress levels among the three therapy groups, suggesting at least one therapy differs from the others."
%}

{% include question_dropdown.html
    id="effectsize2c_new"
    title="Partial Eta-squared Interpretation"
    question_text="Interpret the Partial Eta-squared (η²p) value (0.05) using the guidelines provided. What does it tell us about the therapy effect?"
    solution_text="Partial Eta-squared (η²p) represents the proportion of variance in stress levels explained by the type of therapy. According to the guidelines, η²p = 0.01 is a small effect, 0.06 is a medium effect, and 0.14 is a large effect. Our η²p = 0.05 indicates a **small effect size**. This means that the therapy type accounts for about 5% of the variability in stress levels."
%}

{% include question_dropdown.html
    id="effectsize2d_new"
    title="Combined Conclusion"
    question_text="Considering both the p-value and Partial Eta-squared, what is your overall conclusion regarding the effectiveness of the therapies?"
    solution_text="The p-value (0.022) suggests a statistically significant difference between the groups. However, the Partial Eta-squared (0.05) indicates that the therapy type explains only a small proportion of the variance in stress levels. While there's a detectable difference, the practical impact of therapy type on individual stress levels might be considered modest."
%}

---

### Customer Loyalty Survey

A large retail company wants to investigate if there is an association between a customer's preferred communication method (email, phone, in-store) and their reported loyalty status (loyal, regular, new). They conduct a survey with 5000 customers.

| | Loyal | Regular | New | TOTAL |
| :---- | :---- | :---- | :---- | :---- |
| Email | 1500 | 800 | 200 | 2500 |
| Phone | 500 | 300 | 100 | 900 |
| In-store | 900 | 600 | 100 | 1600 |
| TOTAL | 2900 | 1700 | 400 | 5000 |

A **chi-square test of independence** is performed to examine the association, and **Cramer's V** is calculated as an effect size. The contingency table has 3 rows (Email, Phone, In-store) and 3 columns (Loyal, Regular, New). The degrees of freedom for Cramer's V are min(3-1, 3-1) = min(2,2) = 2.

$$ \chi^2(4, N=5000) = 28.5, p < 0.001, \text{Cramer's V} = 0.075 $$

{% include question_numerical.html
    id="effectsize3a_new"
    title="Loyalty via Email"
    question_text="What percentage (correct to 1 decimal place) of customers who prefer email are 'Loyal'?"
    correct_answer="60.0"
    tolerance="0.05"
    solution_text="$\frac{1500}{2500} \times 100 = 60.0\%$"
%}

{% include question_numerical.html
    id="effectsize3b_new"
    title="Loyalty via Phone"
    question_text="What percentage (correct to 1 decimal place) of customers who prefer phone are 'Loyal'?"
    correct_answer="55.6"
    tolerance="0.05"
    solution_text="$\frac{500}{900} \times 100 = 55.55... = 55.6\%$ (1 d.p.)"
%}

{% include question_dropdown.html
    id="effectsize3c_new"
    title="P-value Interpretation"
    question_text="Interpret the p-value from the chi-square test."
    solution_text="The p-value of < 0.001 is extremely small, well below the 0.05 threshold. This indicates a statistically significant association between preferred communication method and loyalty status, meaning the relationship is unlikely due to random chance."
%}

{% include question_dropdown.html
    id="effectsize3d_new"
    title="Cramer's V Interpretation"
    question_text="Interpret Cramer's V (0.075) for this study, considering the degrees of freedom (df=2) and the guidelines provided. What does it tell us about the association?"
    solution_text="Cramer's V is a measure of association for nominal variables. For df=2, the guidelines are: 0.07 (small effect), 0.21 (medium effect), 0.35 (large effect). Our Cramer's V = 0.075 falls into the **small effect size** category (just above the threshold for small). This means that while there's a statistically significant association, the strength of the relationship between communication preference and loyalty status is quite weak in practical terms."
%}

{% include question_dropdown.html
    id="effectsize3e_new"
    title="Overall Conclusion & Large Sample Size"
    question_text="Given the very small p-value but also a very small Cramer's V, what is your overall conclusion? What does this illustrate about large sample sizes?"
    solution_text="This scenario highlights the importance of effect sizes. The p-value (< 0.001) indicates a statistically significant association. However, the Cramer's V (0.075) reveals that this association is very weak. With such a large sample size (N=5000), even a negligible relationship can become statistically significant. Our conclusion is that while an association technically exists, its practical importance is minimal. This demonstrates that a small p-value does not automatically imply a practically important effect, especially with large samples."
%}
