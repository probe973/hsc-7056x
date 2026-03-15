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

**What it measures:** Partial Eta-squared represents the proportion of variance in the dependent variable that is explained by a specific independent variable (or factor in an ANOVA), after accounting for other factors in the model. It's commonly used in ANOVA.
**Interpretation Guidelines:**
*   **Small effect:** η²p = 0.01 (1% of variance explained)
*   **Medium effect:** η²p = 0.06 (6% of variance explained)
*   **Large effect:** η²p = 0.14 (14% of variance explained)
*   **Note:** Like Cohen's d, these are general guidelines, and context is important.

</div>

---

### New Pain Management Therapy

A clinical trial investigates the effectiveness of a new pain management therapy compared to a standard placebo treatment for chronic back pain. Two separate groups of patients are recruited: one receives the new therapy, and the other receives a placebo. Pain levels are measured using a validated scale (0-10, with higher scores indicating more pain) after 4 weeks of treatment.

An **independent-samples t-test** is performed to compare the mean pain levels between the two groups. **Cohen's d** is calculated as a measure of effect size.

| Group | N | Mean Pain Score | SD | t | p | Cohen's d |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| New Therapy | 40 | 3.2 | 2.5 | -4.85 | < 0.001 | 0.92 |
| Placebo | 40 | 5.5 | 2.5 | | | |

{% include question_multiple_choice.html
    id="effectsize1a_new"
    title="Study Design"
    question_text="Is this an example of a between-groups analysis or a within-groups analysis?"
    options="bg::Between-groups||wg::Within-groups"
    correct_answer="bg"
    solution_text="There are two distinct groups (New Therapy and Placebo), with each participant belonging to only one group. This is a **between-groups** analysis."
%}

{% include question_dropdown.html
    id="effectsize1b_new"
    title="P-value Interpretation"
    question_text="Interpret the p-value given in the table."
    solution_text="The p-value of < 0.001 is very small (much less than 0.05). This indicates that the observed difference in pain scores between the new therapy and placebo groups is statistically significant, suggesting it is highly unlikely to have occurred by chance."
%}

{% include question_multiple_choice.html
    id="effectsize1c_new"
    title="Cohen's d Interpretation"
    question_text="Based on the guidelines, what type of effect size does Cohen's d (0.92) represent?"
    options="small::Small effect||medium::Medium effect||large::Large effect"
    correct_answer="large"
    solution_text="Cohen's d is a standardized measure of the difference between two means. According to the guidelines (Small = 0.2, Medium = 0.5, Large = 0.8), our value of 0.92 is greater than the threshold for a large effect (0.8). Therefore, it indicates a **large effect size**. This means the new pain management therapy has a very substantial and practically important impact on reducing pain compared to the placebo."
%}

{% include question_dropdown.html
    id="effectsize1d_new"
    title="Overall Conclusion"
    question_text="Combining the p-value and Cohen's d, what can you conclude about the effectiveness of the new pain management therapy?"
    solution_text="The p-value (< 0.001) confirms statistical significance, meaning the new therapy is effective. Cohen's d (0.92) indicates a large effect size, suggesting this effect is also highly practically meaningful. Therefore, there is strong evidence that the new pain management therapy is significantly effective and has a substantial positive impact on reducing chronic back pain."
%}

---

### Sleep Quality Improvement Program

Researchers are testing a new sleep quality improvement program. A group of participants completes the 8-week program, and their sleep quality scores (higher scores = better sleep) are measured at three time points: Before the program, Mid-program (4 weeks), and After the program (8 weeks).

A **repeated-measures ANOVA** is performed to examine the change in sleep quality over time. **Partial Eta-squared (η²p)** is calculated for the 'Time' factor.

$$F(2, 58) = 4.10, p = 0.022, \eta^2_p = 0.04$$

{% include question_multiple_choice.html
    id="effectsize2a_new"
    title="Study Design"
    question_text="Is this an example of a between-groups analysis or a within-groups analysis?"
    options="bg::Between-groups||wg::Within-groups"
    correct_answer="wg"
    solution_text="The same individuals are measured at multiple time points (Before, Mid, After). This is a **within-groups** (or repeated-measures) analysis."
%}

{% include question_dropdown.html
    id="effectsize2b_new"
    title="P-value Interpretation"
    question_text="Interpret the p-value given for the repeated-measures ANOVA."
    solution_text="The p-value of 0.022 is less than the standard significance level of 0.05. This indicates that there is a statistically significant change in sleep quality scores over the three time points, suggesting the program had an effect."
%}

{% include question_multiple_choice.html
    id="effectsize2c_new"
    title="Partial Eta-squared Interpretation"
    question_text="Based on the guidelines, what type of effect size does Partial Eta-squared (η²p = 0.04) represent?"
    options="small::Small effect||medium::Medium effect||large::Large effect"
    correct_answer="small"
    solution_text="Partial Eta-squared (η²p) represents the proportion of variance in sleep quality scores explained by the 'Time' factor. According to the guidelines (Small = 0.01, Medium = 0.06, Large = 0.14), our η²p = 0.04 falls into the **small effect size** category, as it is greater than 0.01 but less than 0.06. This means that the progression through the program (time) accounts for about 4% of the variability in sleep quality scores."
%}

{% include question_dropdown.html
    id="effectsize2d_new"
    title="Combined Conclusion"
    question_text="Considering both the p-value and Partial Eta-squared, what is your overall conclusion regarding the effectiveness of the sleep quality improvement program?"
    solution_text="The p-value (0.022) indicates that the program led to a statistically significant change in sleep quality over time. However, the Partial Eta-squared (0.04) reveals that this effect is a small effect. While the program *does* have a detectable impact, the amount of variation in sleep quality scores explained by the program is modest. This suggests a statistically significant but practically small effect."
%}
