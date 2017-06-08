---
layout: post
title: "Weightlifting Data Analysis"
---

<p>I am currently in the process of analysing and exploring what factors affect the results of an Olympic weightlifter. Using data gathered from the <a href="http://www.iwf.net/" target="_blank">International Weightlifting Federation's</a> website, I generated a few graphs with Python's Matplotlib library comparing a number of variables affecting a weightlifter's results at the Olympics:</p>

{% include image.html url="https://github.com/LeNPaul/data-analysis-projects/tree/master/weightlifting" image="/blog/weightlifting-data-analysis/figure_4.png" text="View Code" %}

The above plot shows the relationship between a weightlifter's bodyweight, and their total weight lifted, plotted on a logarithmic scale. It's pretty clear that this relationship isn't linear, but more logarithmic (although it still deviates from a logarithm). This is interesting, because I believe the [Sinclair Coefficient](http://www.iwf.net/weightlifting_/sinclair-coefficient/), which offers a way of comparing lifters in different weight categories, also fundamentally is a logarithmic equation - this is most likely how it is derived, shown graphicaly.

{% include image.html url="https://github.com/LeNPaul/data-analysis-projects/tree/master/weightlifting" image="/blog/weightlifting-data-analysis/figure_7.png" text="View Code" %}

It's common knowledge that there is a strong linear relationship between a weightlifter's snatch, and clean & jerk lifts. The above plot just shows this more clearly. The line of best fit for this dataset is 81 +/- 3%, which fits nicely with anecdotal knowledge.

{% include image.html url="https://github.com/LeNPaul/data-analysis-projects/tree/master/weightlifting" image="/blog/weightlifting-data-analysis/hist_figure_2.png" text="View Code" %}

Finally, I wanted to see whether or not a weightlifter's results are influenced by the weight that they lifting, whether even numbered weights, such as 120kg or 125kg are more common than weights such as 121kg or 113kg. I did this initially by plotting a histogram of some weightlifting data, using 1kg bins. The presence of spikes in the histogram seems to demonstrate that even numbered weights are more common. More analysis is required.
