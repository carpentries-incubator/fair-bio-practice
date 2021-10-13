---
title: "Jupyter notebooks for data analysis"
teaching: 0
exercises: 0
questions:
- "How is live coding with instant output beneficial for FAIR?"
- ""
- ""
objectives:
- "Benefits of notebooks for analysis"
- "Use a notebook and modify it"
- "How notebooks help in FAIR"
keypoints:
- "Tools such as Jupyter Notebooks are great to share analysis with non-programmers"
- ""
- ""
---

## Jupyter Notebook for FAIR practices
[Jupyter](www.jupyter.org) Notebooks are interactive web applications which allow you to type and edit lines of code in Python or R, and view the output (e.g. graphs or calculations) immediately. The huge benefit of such notebooks is that source code is mixed with documentation, thus explaining experimental setup, analysis, results of tables and plots throughout.

What is left for us to do is write the code through which we want to analyse our data, and explain the narrative behind the experiment and interpretation of the results. Notebooks can be exported as .pdf and .html file which allows for easy sharing of notebooks.

> ## Exercise
>
> Discuss how Jupyter Notebooks can help in being FAIR:
>
>> ## Solution
>>
>> *  Findable? - We should mention that you can share them on Git and then they are finadable no?
>> *  Sharing of code in form of a Jupyter Notebook makes data and analysis more accessible
>> *  The format of Jupyter Notebooks is highly interoperable since files can be exported as .pdf, .html or as original jupyter notebook files (.ipynb) which allows opening/viewing of these files with standard browsers
>> *  Sharing of code in form of a Jupyter Notebook makes analysis reproducible
> {: .solution}
{: .challenge}

## Working with Jupyter Notebooks

To show you how easy it is to work with Jupyter Notebooks, we have created an exercise for you where we will work on "real-life" data from an experiment looking at circadian influence on plants following short-day and long-day light exposure. We will create some graphs and test whether there are differences between our genotypes of arabidopsis using R.

> ## Exercise - basics of Jupyter notebooks
> Open this [Jupyter notebook](http://mango.bio.ed.ac.uk:8888/tree), we will first show you how to duplicate a notebook and save it and how to run the code:
> 1. Select the notebook titled 'student_notebook_light_conditions.ipynb' as depicted below and click 'Duplicate'. Confirm with Duplicate when you are asked if you are certain that you want to duplicate the notebook.
> ![Figure 1. Duplicate a Jupyter notebook](../fig/10-01-duplicate_notebook.png)
> 1. A copy of the notebook has appeared with the suffix '-Copy' and a number (Figure 2a), select this notebook. Have a look around the notebook and explore its anatomy (Figure 2), you should see experimental details, an image, and code. If you click on separate parts of the notebook you can see that it is divided into individual cells (Figure 2 e-g) which are of varying type (Code, R in this case, or Markdown - Figure 2d). Hashtags are comments within the code and shall help you to interpret what individual bits of code do.
> ![Figure 2. Anatomy of a Jupyter notebook: (a) depicts the name of the notebook, (b, c) are toolbars, (c) contains the most commonly used tools, (d) shows of what type - Markdown, Code etc... - the currently selected cell is, and (e-g) are examples of cells, where (e) shows the currently selected cell. ](../fig/10-02-jupyter_anatomy.png)
> 1. Change the title of the notebook (a) to your initials e.g. "student_notebook_light_conditions_IB"
> 1. To Save the notebook click on the disk symbol in the toolbar (c).
> 1. To run the code select the top cell of the notebook (e) - this is likely pre-selected already - and click "Run" in the tool bar (c). The selected cell jumps one cell down (f).
> 1. To avoid having to press Run repeatedly until we are at the end of the code (try clicking Run two more times and see what happens), we will show you how to run all the code. In the top tool bar (b) click "Cell" and select "Run All". ("Cell > Run All".)
> 1. If you have another look at the notebook you can see that a table, graph and outputs of statistical testing have been generated.
>> ## Solution
>> If you followed all steps correctly you should have reproduced the table, a graph and statistical testing. Apart from the pre-filled markdown text the rendered values of the code should look like this:
>> ![Figure 3. Rendering of data frame](../fig/10-03-jupyter_dataframe.png)
>> ![Figure 4. Rendering of plot](../fig/10-04-jupyter_plot.png)
> {: .solution}
{: .challenge}

> ## Exercise - how to add and remove content
> In your previously saved notebook, we will now show you how to add text and remove cells within your notebook. Additionally we will show you how to change code:
> 1. We want to change the author name to your name: Double click on the cell containing the author name. You can see how the layout of the cell changes into Markdown, and you can simply change the name.
> 2. Press the Run button in the toolbar and the Markdown of the cell will be rendered again and you can see the text shows as previously.
> 3. We now want to add some details about the "light_results.txt" file which is being loaded. To add a cell above the code, click the cell currently above the first lines of code and click the "+" in the toolbar. This creates a cell below selected cell.
> 4. Now add a note about the file which is being loaded and the purpose of the subsequent analysis: e.g. Loading of results following short- and long-day light exposure on arabidopsis, followed by visualisation of differences in chlorophyll/biomas etc... content between genotypes on short-days and long-days. To show the cell as Markdown and not code, make sure "Markdown" is selected in the toolbar.
> 5. To remove a cell, select it and click on the scissors icon in the toolbar.
> 6. To change the output of your graph click on the cell containing the code below the "Visualise data" title. We want you to change the colours of the box-plots. You can do this where the comment "# change colour of groups" is written. Either you can use three different HEX codes (a 6-symbol code representing colours from white to black), or colours simply by their name - e.g. dark blue, orange...
{: .challenge}

> ## Exercise - add another analysis step
> We have shown you how to manipulate text and code in Jupyter notebooks, now we want you to add data visualisation (a graph) and stats for long-day light condition:
> 1. Add additional cells including
> * titles
> * edited code to depict graph from long-days and not short-days
> * Figure legend
> * statistical testing of difference between genotypes on long-days
> *interpretation of results of statistical testing.
>
>> ## Solution
>> The following code will result in your new graph:
>> ~~~
>> ggplot(subset(df, light_condition %in% "LD"), 
>> # subset only SD from >>light condition column for plotting
>>       mapping = aes(x = genotype, y = biomas, fill = genotype)) + 
>> # x-axis shows genotype, y-axis shows biomas
>>    geom_boxplot(alpha=0.3) +
>>    labs(title = "Biomas per Genotype on long days",
>>        x = "Genotype", # Title of x-axis
>>        y = "Biomas (g)") + # Title of y-axis
>>    # change colour of groups
>>    scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9")) +
>>    theme_bw() +
>>    theme(legend.position="none")
>> ~~~
>> {: .source}
>>
>> The following code will result in testing of biomas between genotypes in long-days - we assign a new variable to separate both analysis.
>> ~~~
>> res.aov.LD <- aov(biomas ~ genotype, data = subset(df, light_condition %in% "LD"))
# Summary of the analysis
summary(res.aov.LD)
>> ~~~
>> {: .source}
>> 
>> The following code will result in Tukey multiple pairwise-comparison testing.
>> ~~~
>> # conduct Tukey multiple pairwise-comparison
TukeyHSD(res.aov.LD)
>> ~~~
>> {: .source}
> {: .solution}
{: .challenge}

Show a notebook (with nice descriptions cells) which:
- (if possible to get a sensible library/program) 
calls a code from command line to do some simple file processing
(maybe one step from workflows workshop) 
that should show that it can replace commands lines while showing how exactly the programs/library well called
- reads in the results or excell files (in python)
- plots something from the results
- saves the figure to a file

- ask to run it
- ask to add some description (non coding cell)
- ask to change input file to another one and re-analysed it


## I am a section

With a text.

![Figure 1. I am some figure](../fig/figure_file.jpg)

*After [Figure source](https://www.figure.link/)*


> ## I am a yellow info
>
> And my text.
{: .callout}


~~~
I am code
~~~
{: .source}


> ## I am a problem
>
> Defined here.
>
>> ## Solution
>>
>> *   I am an answer.
>> *   So am I.
> {: .solution}
{: .challenge}


> ## Attribution
> Content of this episode was adopted from
> [Reproducible analysis and Research Transparency](https://reproducible-analysis-workshop.readthedocs.io/en/latest/4.Jupyter-Notebook.html).
{: .callout}


{% include links.md %}
