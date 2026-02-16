---
layout: default
title: Distributions Workshop
---

<div class="explanation" markdown="1">
# Distributions: Summary Statistics and Shape

This workshop focuses on understanding and calculating descriptive statistics—measures that summarize the characteristics of a dataset. We will focus on central tendency (mean and median), dispersion (range and standard deviation), and the shape of the distribution (skew).
</div>

---

### Question 1: Calculations

Consider the following dataset:  
     
   $34, 35, 35, 36, 40, 40, 40, 40, 41, 42, 44, 47$


{% capture stats1 %}
<table class="table table-bordered">
  <thead>
    <tr>
    <th scope="col">Statistic</th>
    <th scope="col">Value</th>
    </tr>
  </thead>
  <tbody>
       <tr>
            <td>Mean</td>
            <td><input type="number" step="any" aria-label="Mean of the data set"></td>
       </tr>
       <tr>
            <td>Median</td>
            <td><input type="number" step="any" aria-label="Median of the data set"></td>
       </tr>
       <tr>
            <td>Range</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
  </tbody>
</table>
{% endcapture %}

{% include table_fill.html 
   id="statsq1" 
   title="1"
   question_text="Calculate the mean, the median, and the range, rounding to 2 decimal places if necessary:"
   table_content=stats1
   answers="39.58 || 40 || 13"
   tolerance="0.005" 
   solution_text="The mean is calculated as the sum of all values divided by the number of values ($\frac{\sum x}{N}$).  $\frac{475}{12} = 39.58$. <br>
   Since there is an even number of values (12), the median is the average of the two middle values (the 6th and 7th values): $\frac{40 + 40}{2} = 40$.<br>
   The range is the largest value minus the smallest value: $47 - 34 = 13$."
%}

---

### Question 2: The Impact of Outliers

For the data in Question 1, we will change the final three data points ($42, 44, \text{ and } 47$) to $50, 65, \text{ and } 100$.

The new dataset is: $34, 35, 35, 36, 40, 40, 40, 40, 41, 50, 65, 100$.

{% include question_numerical.html
    id="q2_median"
    title="Question 2a: Recalculate the Median"
    question_text="Recalculate the **median** of the new dataset."
    correct_answer="40"
    tolerance="0"
    solution_text="The median is the average of the 6th and 7th values: $\frac{40 + 40}{2} = 40$. The median is not affected by these 3 extreme values."
%}

{% include question_numerical.html
    id="q2_mean"
    title="Question 2b: Recalculate the Mean"
    question_text="Recalculate the **mean** of the new dataset. (Round to two decimal places if necessary)"
    correct_answer="48.83"
    tolerance="0.01"
    solution_text="The new sum is $586$. The new mean is $\frac{586}{12} = 48.83$."
%}

{% include question_dropdown.html
    id="q2_contrast"
    title="Question 2c: Mean vs. Median"
    question_text="What do you notice about the values for the median and mean between Question 1 and Question 2?"
    solution_text="The **median** remained the same (40), but the **mean** increased significantly (from 39.58 to 48.83). This demonstrates that the mean is sensitive to extreme values (outliers), while the median is more resistant to them."
%}

{% include question_multiple_choice.html
    id="q2_skew"
    title="Question 2d: Type of Skew"
    question_text="What type of skew is shown in the data for Question 2?"
    options="neg::Negative (Skewed Left)||pos::Positive (Skewed Right)||sym::Symmetrical"
    correct_answer="pos"
    solution_text="The mean (48.83) is significantly higher than the median (40). This indicates that the extreme values (outliers) are pulling the mean toward the positive (right) end of the distribution, which is a **Positive Skew**."
%}

---

### Question 3: Comparing Datasets

Consider the following three sets of data:  
     
   Set A: 	$12, 13, 15, 15, 16, 16, 16, 17, 17, 19, 20, 20$  
   Set B:		$3, 5, 5, 9, 16, 21, 22, 30, 33$  
   Set C:		$21, 24, 25, 26, 26, 27, 27, 27, 27, 28, 29, 30$ 

{% capture stats2 %}
<table class="table table-bordered">
  <thead>
    <tr>
    <th scope="col">Statistic</th>
    <th scope="col">Set A</th>
     <th scope="col">Set B</th>
     <th scope="col">Set C</th>
    </tr>
  </thead>
  <tbody>
       <tr>
            <td>Mean</td>
            <td><input type="number" step="any" aria-label="Mean of the data set A"></td>
            <td><input type="number" step="any" aria-label="Mean of the data set B"></td>
            <td><input type="number" step="any" aria-label="Mean of the data set C"></td>
       </tr>
       <tr>
            <td>Median</td>
            <td><input type="number" step="any" aria-label="Median of the data set A"></td>
            <td><input type="number" step="any" aria-label="Median of the data set B"></td>
            <td><input type="number" step="any" aria-label="Median of the data set C"></td>
       </tr>
       <tr>
            <td>Range</td>
            <td><input type="number" step="any" aria-label="Range of the data set A"></td>
            <td><input type="number" step="any" aria-label="Range of the data set B"></td>
            <td><input type="number" step="any" aria-label="Range of the data set C"></td>
       </tr>
  </tbody>
</table>
{% endcapture %}

{% include table_fill.html 
   id="statsq3a" 
   title="3a"
   question_text="Calculate the mean, the median, and the range, rounding to 2 decimal places if necessary, of the three data sets:"
   table_content=stats2
   answers="16.33 || 16 || 26.42 || 16 || 16 || 27 || 8 || 30 || 9"
   tolerance="0.005" 
   solution_text="**Set A (N=12):** Mean = 16.33, Median = 16.0, Range = 8 <br>
   **Set B (N=9):** Mean = 16, Median = 16.0, Range = 30 <br>
   **Set C (N=12):** Mean = 26.42, Median = 27.0, Range = 9"
%}


{% include question_dropdown.html
    id="q3_contrast"
    title="Question 3b: Compare and Contrast"
    question_text="Compare and contrast the three datasets based on their summary statistics."
    solution_text="
*   **Central Tendency (Mean/Median):** Set A and Set B have similar median/mean values (around 16), while Set C has a much higher central tendency (around 26-27).
*   **Dispersion (Range):** Set B has the largest range (30), indicating the greatest spread of data. Set A has the smallest range (8), indicating the most homogeneous (least spread) data.
*   **Skew:** All datasets have very similar mean and median values, suggesting they are all relatively symmetrical."
%}

---

### Question 4: Interpreting Summary Statistics

Summary statistics are provided for three sets of data:  
     
   Set A:  
   Mean = 45.4,  Median = 33,  SD = 6.8,  Skew = 1.6  
     
   Set B:  
   Mean = 34.2,  Median = 33.5,  SD = 2.3,  Skew = 0.21  
     
   Set C:  
   Mean = 33,  Median = 33.6,  SD = 0.9, Skew = -0.12  

{% include question_multiple_choice.html
    id="q4_dispersion"
    title="Question 4a: Dispersion"
    question_text="Which dataset had the least dispersion (least spread of data)?"
    options="set_a::Set A||set_b::Set B||set_c::Set C"
    correct_answer="set_c"
    solution_text="Dispersion is measured by the Standard Deviation (SD). Set C has the smallest SD (0.9), meaning the data points are clustered most tightly around the mean."
%}

{% include question_multiple_choice.html
    id="q4_skew_dir"
    title="Question 4b: Skew"
    question_text="Which dataset had the most skew, and in what direction was the skew?"
    options="a_pos::Set A (Positive)||b_pos::Set B (Positive)||a_neg::Set A (Negative)"
    correct_answer="a_pos"
    solution_text="Set A had the largest absolute skew value (1.6), and since the value is positive, it shows a **Positive Skew**."
%}

{% include question_dropdown.html
    id="q4_contrast"
    title="Question 4c: Compare and Contrast"
    question_text="Compare and contrast the three datasets."
    solution_text="
*   Set A has a much higher mean value than the other two datasets, which have similar means.  The medians of all of the datasets are very similar. 
*   Set A is highly skewed to the right, whereas the other two datasets are more symmetrical.
*   Set C is the least spread of the three datasets, with the lowest standard deviation.
"
%}

---

### Question 5: Interpreting Histograms

Consider the following histograms and statistics:

![A 2 by 2 grid of histograms.  Top left has symettry and is centred around 30.  Top right has symettry, but less spread than others, and is centred around 50.  Bottom left has symettry and is centred around 50.  Bottom right has a tail to the left and is centred around 50.  In the same order the diagrams are labelled A, B, C, and D.]({{ "/assets/images/let/histogram_match.png" | relative_url }})


| Statistic | Set 1 | Set 2 | Set 3 | Set 4 |
|:----|:----|:----|:----|:----|
| Mean | 49.2 | 29.9 | 50 | 49.9 |
| Median | 50 | 30 | 50 | 50 |
| Standard Deviation | 10.5 | 11.4 | 5.7 | 11.4 |
| Skew | -0.64 | 0 | 0 | 0 |


{% capture distributions1 %}
<table class="table table-bordered">
  <thead>
    <tr>
    <th scope="col">Histogram</th>
    <th scope="col">Dataset number</th>
    </tr>
  </thead>
  <tbody>
       <tr>
            <td>A</td>
            <td><input type="number" step="any" aria-label="Histogram A set number"></td>
       </tr>
       <tr>
            <td>B</td>
            <td><input type="number" step="any" aria-label="Histogram B set number"></td>
       </tr>
       <tr>
            <td>C</td>
            <td><input type="number" step="any" aria-label="Histogram C set number"></td>
       </tr>
       <tr>
            <td>D</td>
            <td><input type="number" step="any" aria-label="Histogram D set number"></td>
       </tr>
  </tbody>
</table>
{% endcapture %}

{% include table_fill.html 
   id="distq5" 
   title="5"
   question_text="Match each of the histograms to one of the sets of statistics provided above."
   table_content=distributions1
   answers="2 || 3 || 4 || 1"
   tolerance="0.5" 
   solution_text="
   **Analysis and Matching:**
1.  **Look at Mean/Median/Skew:** One set of data has a Mean of 29.9 and a Median of 30. This is significantly lower than the other sets (which are near 50). This must be the histogram that is clustered more to to the **left** of the others on the horizontal axis, histogram A.
2.  **Look at Skew:** One set has a Skew of -0.64. This indicates a **Negative Skew (Skewed Left)**. This must be the histogram with the long tail extending to the left, histogram D.
3.  **Look at Standard Deviation (Dispersion):** Two remaining sets are symmetrical (Skew=0). One has a low SD (5.7) and one has a high SD (11.4). The low SD set must match the histogram that is the **least dispersed**. The high SD set must match the histogram that is the **most spread out**.

**Solution:**
*   **Histogram A** Matches Mean = 29.9, Median = 30, **Set 2**.
*   **Histogram B** Matches Mean = 50, SD = 5.7 **Set 3**.
*   **Histogram C:** Matches Mean = 49.4, SD = 11.4 **Set 4**
*   **Histogram D:** Matches SKew = -0.64 **Set 1**.
*   "
%}
