---
title: "Working with files"
teaching: 15
exercises: 20
questions:
- "How should a project folder be organized?"
- "What are naming conventions?"
- "How should I name my files?"
- "How does project organisation help to make data FAIR?"
objectives:
- "Learn different file naming strategies"
- "Engage in project organization"
- "Be able to explain how it helps in being FAIR"
keypoints:
- "You have to plan ahead your project layout"
- "You have to decide on naming conventions and stick to them"
- "Project organization helps you save time in the long run"
- "Project organization helps to make your data Findable"
- "Project organization can also help to make your data Interoperable"
---

## Project organization: planning file names and folders structure

Before you even start collecting or working with data, you should decide how you will structure and name files and folders. This will:
* allow for standardized data collecting and analysis by many team members.
* make it easier for the researcher to determine where files should be saved.
* avoid file duplication.
* help to make retrieval and archiving more efficient.


![Intro to folder structure](../fig/07-intro_folder_structure.png)
*Figure credits: Andrés Romanowski*

Consistent naming and organizing files in folders has two main goals:
* quick finding needed files
* being able to tell the file content without opening it

## Naming your files (and folders)
One important and often overlooked aspect of organizing, sharing, and keeping track of data
files is standardising naming.
It is important to develop naming conventions
which permits encoding experimental factors which are important to the project.

File (folder) names should be consistent, meaningful to you and your collaborators,
allow you to easily find what you are looking for,
give you a sense of the content without opening the file,
and identify if something is missing.

> > 2020-07-14_s12_phyB_on_SD_t04.raw.xlsx
> > 2020-07-14_s1_phyA_on_LD_t05.raw.xlsx
> > 2020-07-14_s2_phyB_on_SD_t11.raw.xlsx
> > 2020-08-12_s03_phyA_on_LD_t03.raw.xlsx
> {: .source}

> 2020-07-14_s12_phyB_on_SD_t04.raw.xlsx
> 2020-07-14_s1_phyA_on_LD_t05.raw.xlsx
> 2020-07-14_s2_phyB_on_SD_t11.raw.xlsx
> 2020-08-12_s03_phyA_on_LD_t03.raw.xlsx
{: .source}


> ## Naming and sorting (5 minutes)
> Have a look at the example files from a project, similar
> to the one from metadata episode.
>
> All the files have been sorted by name and
> demonstrate consequences of different naming strategies.
>
> For your information, to encode experimental details, following conventions were taken:
> * phyB/phyA are sample genotype,
> * sXX is sample number
> * LD/SD are different light conditions
> * on/off are different media
> * measurement date
> * other details are timepoint and raw or normalized data
>
> > 2020-07-14_s12_phyB_on_SD_t04.raw.xlsx
> > 2020-07-14_s1_phyA_on_LD_t05.raw.xlsx
> > 2020-07-14_s2_phyB_on_SD_t11.raw.xlsx
> > 2020-08-12_s03_phyA_on_LD_t03.raw.xlsx
> > 2020-08-12_s12_phyB_on_LD_t01.raw.xlsx
> > 2020-08-13_s01_phyB_on_SD_t02.raw.xlsx
> > 2020-7-12_s2_phyB_on_SD_t01.raw.xlsx
> > AUG-13_phyB_on_LD_s1_t11.raw.xlsx
> > JUL-31_phyB_on_LD_s1_t03.raw.xlsx
> > LD_phyA_off_t04_2020-08-12.norm.xlsx
> > LD_phyA_on_t04_2020-07-14.norm.xlsx
> > LD_phyB_off_t04_2020-08-12.norm.xlsx
> > LD_phyB_on_t04_2020-07-14.norm.xlsx
> > SD_phyB_off_t04_2020-08-13.norm.xlsx
> > SD_phyB_on_t04_2020-07-12.norm.xlsx
> > SD_phya_off_t04_2020-08-13.norm.xlsx
> > SD_phya_ons_t04_2020-07-12.norm.xlsx
> > ld_phyA_ons_t04_2020-08-12.norm.xlsx
> {: .source}
>
> How do you think the naming conventions will affect sorting of these files? Discuss in pairs.
> > ## Solution
> > There a series of issues with the way the files were named. Let's see if you found the same ones we spotted:
> > * Using dates up front makes it difficult to find a particular file by genotype/conditions (though dates in front may have value when content has multiple variables).
> > * Look at how 's12' would appear before s1 and s2 because a leading 0 is not used when naming the files.
> > * You need dates to be numeric or the other will not be logical (example: Aug would appear before Jul, if using letters).
> > * There is lack of consistency with the numerical date at the start: 2020-7 appears after 2020-08-13 (there is a missing leading zero that c).
> > * Further lack of consistency as the files on top, middle, and bottom use different conventions.
> > * There are some issues with cases, 'ld' is after 'SD', also 'phya' is after 'phyB'.
> >
> > There are some good points too:
> > * Normalised data has a consistent way to help you find the data: 'LD' vs 'SD' conditions, followed by genotype.
> > * Keeping the same length of each section of the name makes it easier to read: 'ons' and 'off' (on succrose, off succrose) nicely ordered in the last three files.
> {: .solution}
{: .challenge}

## Naming your files (and folders)
One important and often overlooked aspect of organizing, sharing, and keeping track of data files is standardising naming. It is important to develop naming conventions including elements that are important to the project. Your file (and folder) names should be consistent, meaningful to you and your collaborators, allow you to easily find what you are looking for, give you a sense of the content without opening the file, and identify if something is missing.
Some things to take into account to decide on your naming convention are:

- Does your convention make your files easy to sort?
	- date: consider using 'YYYYMMDD' or 'YYYY-MM-DD' as part of your name
	- file version: consider including versioning as part of your system. Using leading zeroes will help keep a certain length in this element (i.e.: v005 instead of v5).
	- other parameters that will help you sort your files: consider including a project acronym, researcher name, sample, experiment as part of your file name.
- Is your file name as descriptive as possible?
	- include any parameter that helps the name being as descriptive as possible (i.e.: project, experiment, researcher, sample, organism, date (range), data type, method)
- Have you defined a standard vocabulary for file names?
	- decide which elements go in which order. This will help everyone use a common language.
- Have you defined a maximum name length? (is the name to long or too short?)
	- aim for filenames no longer than ~30 characters. If you need to abbreviate your parameters to fit this criteria, remember to document it on your metadata.
- Have you defined which punctuations to use?
	- decide on conventions on when to use symbols, capitals, hyphens and spaces.
- Are you using special symbols?
	- Don't! Some software cannot recognise the symbols and this may bring problems in the long run.


> ## Challenge (2.5 minutes)
> Now imagine a case where you would have to rename thousands of files instead of 5-10.
> Using the previous example, can you imagine a solution involving folder structure that could help if you had hundreds or thousands of files?
>
> > ## Solution
> > One way to solve this would be to transform the elements of your file naming conventions into a folder structure:
> > For example:
> > .
> > |-- LD
> > |-- | arabidopsis
> > |-- |-- | genotype
> > |-- |-- |-- | media
> > |-- |-- |-- |-- | sample ID
> >
> > > ## Must do
> > > Regardless of whether you are using long filenames or incorporating some of the variables within the folder structure, document it!
> > > Always include a ReadMe file describing your file naming and folder organisation conventions.
> > {: .callout}
> {: .solution}
{: .challenge}


## Strategies to set up a clear folder structure
Establishing a system that allows you to access your files, avoid duplication and ensure that your data can be easily found needs planning. You can start by developing a logical folder structure. To do so, you need to take into account the following suggestions:

- Use folders: grouping related files within a single folder will make it easy to locate them.
- Name folders appropriately: use descriptive names after the areas of work to which they relate. It is not recommended to use individual researchers or students as the folder name as this can lead to confusion in shared workspaces.
- Be consistent: agree on a naming convention from the outset of your research project.
- Structure folders hierarchically: use broader topics for your main folders and increase in specificity as you go down the hierarchy.

> ## Before you begin
> Always check if your group already has set up standard operating procedures for structuring research data folders. Don't reinvent the wheel, unless it is absolutely necessary.
>
{: .callout}

> ## Tip
> Sometimes it is better to make separate folders for ongoing and completed work. In some cases it is a good idea to start thinking about separating your older documents from those you are currently working on. See if this fits with your project.
{: .callout}

> ## Challenge (5 minutes)
> Take a look at the folder structure recommended by the [Good enough practices in scientific computing](https://doi.org/10.1371/journal.pcbi.1005510) paper.
> >
> > .
> > |-- CITATION
> > |-- README
> > |-- LICENSE
> > |-- requirements.txt
> > |
> > |-- data
> > |   |-- birds_count_table.csv
> > |
> > |-- doc
> > |   |-- notebook.md
> > |   |-- manuscript.md
> > |   |-- changelog.txt
> > |
> > |-- results
> > |   |-- summarized_results.csv
> > |
> > |-- src
> > |   |-- sightings_analysis.py
> > |   |-- runall.py
> > |
> >
> > Note: This project doesn't have a bin directory because it does not rely on any compiled software.
> {: .source}
> > ## Solution
> > The structure is a concrete example of how a simple scientific computing project might be organized.
> > * The root directory contains a README file that provides an overview of the project as a whole, a CITATION file that explains how to reference it, and a LICENSE file that states the licensing.
> > * The data directory contains a single CSV file with tabular data on bird counts (machine-readable metadata could also be included here).
> > * The src directory contains sightings_analysis.py, a Python file containing functions to summarize the tabular data, and a controller script runall.py that loads the data table, applies functions imported from sightings_analysis.py, and saves a table of summarized results in the results directory.
> {: .solution}
{: .challenge}

## Good enough practices for scientific computing recommendations
The [Good enough practices in scientific computing](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510#sec009) paper makes the following simple recommendations:
* Put each project in its own directory, which is named after the project
* Put text documents associated with the project in the 'doc' directory
* Put raw data and metadata in a 'data' directory
* Put files generated during cleanup and analysis in a 'results' directory
* Put project source code in the 'src' directory
* Put compiled programs in the 'bin' directory
* Name all files to reflect their content or function:
	- Use names such as 'bird_count_table.csv', 'notebook.md', or 'summarized_results.csv'.
	- Do not use sequential numbers (e.g., result1.csv, result2.csv) or a location in a final manuscript (e.g., fig_3_a.png), since those numbers will almost certainly change as the project evolves.

> ## After you have a plan
> Your naming conventions might need some adjustments as the project progresses. Don't despair, just document it!
{: .callout}

## Backup your project files and folders
Always backup your data in 3 places, at least one off-site (cloud-storage). Don't just use a failure-prone option (i.e.: USB drive)
Warning! You may not be able to put everything in a public cloud (check your institutional guidelines).

> ## Challenge (2.5 minutes)
> How can you achieve this?
> > ## Solution:
> > - Check your institutional services regarding data backup
> > - Determine the 3 places where you will backup your data
> > - You need to set up automatic software to backup
> {: .solution}
{: .challenge}


## Project organization and FAIR guidelines
Did you realise that the suggestions we made above mean that you are including valuable metadata as part of your folder and file names? As we mentioned in the [Introduction to Metadata episode](../04-intro-to-metadata), metadata provides valuable information for us and others to be able to interpret your research data.

> ## Challenge - discussion (5 minutes)
> In groups, discuss:
> * how can planning project folder organisation and defining naming conventions help the process of FAIRification?
{: .challenge}


> ## Attribution
> Content of this episode was created using the following references as inspiration:
> - [Good enough practices in scientific computing (Wilson et al., 2017)](https://doi.org/10.1371/journal.pcbi.1005510)
> - [Organising your data](https://www.data.cam.ac.uk/data-management-guide/organising-your-data)
> - [Organising files and folders](https://www.wur.nl/en/Value-Creation-Cooperation/Collaborating-with-WUR-1/Organising-files-and-folders.htm)
> - [File naming](https://libguides.princeton.edu/c.php?g=102546&p=930626)
>
{: .callout}


{% include links.md %}
