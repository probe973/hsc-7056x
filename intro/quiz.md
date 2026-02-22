---
layout: default
title: Introduction Quiz
---

<div class="instructions" markdown="1">
  
# Statistics Matching Exercise

The exercise below will give you a set of statistical words, each with a numerical value.  Your job is to look at the definitions in the table and type in the number that best matches the definition.

</div>

### Statistical Terms

1. Confidence interval
2. Frequency
3. Inference
4. Mean
5. Median
6. Odds ratio
7. p-value
8. Power
9. Standard deviation
10. Standard error

{% capture introquiz %}
<table class="table table-bordered">
  <thead>
    <tr>
    <th scope="col">Definition</th>
    <th scope="col">Matching term number</th>
    </tr>
  </thead>
  <tbody>
       <tr>
            <td>The number of times a particular value or category appears in a dataset</td>
            <td><input type="number" step="any" aria-label="Mean of the data set"></td>
       </tr>
       <tr>
            <td>The middle value in an ordered list of numbers. If there are two middle values, it is the average of those two</td>
            <td><input type="number" step="any" aria-label="Median of the data set"></td>
       </tr>
       <tr>
            <td>A range of plausible values for an unknown population quantity, constructed so that it would contain the true value a specified proportion of the time if the study were repeated</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
      <tr>
            <td>The average value found by adding all observations and dividing by the number of observations</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
    <tr>
            <td>The probability of observing results this extreme (or more so) if there were actually no real effect</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
    <tr>
            <td>The process of using data from a sample to make conclusions about a larger population</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
    <tr>
            <td>A comparison of the likelihood of an outcome occurring in one group relative to another group</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
    <tr>
            <td>The probability that a study will correctly detect a real effect when one truly exists</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
    <tr>
            <td>A measure describing how spread out values are around the average; larger values indicate greater variability</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
    <tr>
            <td>An estimate of how much a calculated sample result would vary if the study were repeated many times</td>
            <td><input type="number" step="any" aria-label="Range of the data set"></td>
       </tr>
  </tbody>
</table>
{% endcapture %}

{% include table_fill.html 
   id="introq" 
   title="Match"
   question_text="Type in the numerical value that best matches the definition, from the list given."
   table_content=introquiz
   answers="2 || 5 || 1 || 4 || 7 || 3 || 6 || 8 || 9 || 10"
   tolerance="0" 
   solution_text="Answers are only shown as correct or incorrect for this quiz"
%}

<div style="text-align: center; margin-top: 3em;">
    <a href="{{ "/intro" | relative_url }}">← Back</a>
</div>
