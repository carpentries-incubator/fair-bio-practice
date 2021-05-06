---
title: "Working with files"
teaching: 15
exercises: 15
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

## Project files and folder structure organization
Before you even start collecting or working with data, you should decide how you will structure and name files and folders. This will:
* allow for standardized data collecting and analysis by many team members.
* make it easier for the researcher to determine where files should be saved.
* avoid file duplication.
* help to make retrieval and archiving more efficient.  
  
Established file plans demonstrate consistency and continuity in recordkeeping.

## Strategies to set up a clear folder structure
Establishing a system that allows you to access your files, avoid duplication and ensure that your data can be easily found needs planning. You can start by developing a logical folder structure. To do so, you need to take into account the following suggestions:

- Use folders: grouping related files within a single folder will make it easy to locate them.
- Name folders appropriately: use descriptive names after the areas of work to which they relate. It is not recommended to use individual researchers or students as the folder name as this can lead to confusion in shared workspaces.
- Be consistent: agree on a naming convention from the outset of your research project.
- Structure folders hierarchically: use broader topics for your main folders and increase in specificity as you go down the hierarchy.

![Intro to folder structure](../fig/07-intro_folder_structure.png)
*Figure credits: Andrés Romanowski*  

> ## Before you begin
> Always check if your group already has set up standard operating procedures for structuring research data folders. Don't reinvent the wheel, unless it is absolutely necessary.  
> 
{: .callout}

> ## Tip
> Sometimes it is better to make separate folders for ongoing and completed work. In some cases it is a good idea to start thinking about separating your older documents from those you are currently working on. See if this fits with your project.
{: .callout}

> ## Challenge (5 minutes)
> Look at this two different folder structures used to organise the same data. Which one do you think is the better option? 
> 
> <ADD MISSING FIG>
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
	- aim for filenames no longer than ~30-60 characters. If you need to abbreviate your parameters to fit this criteria, remember to document it on your metadata.
- Have you defined which punctuations to use?
	- decide on conventions on when to use symbols, capitals, hyphens and spaces.
- Are you using special symbols?
	- Don't! Some software cannot recognise the symbols and this may bring problems in the long run. 

> ## Challenge (5 minutes)
> You have to decide on a naming convention for the microscopy figures of the dataset we looked at in the [Introduction to Metadata episode](../04-intro-to-metadata):
> <p style="text-align:center;"> <img src="../fig/04-microscopy_with_metadata.png" alt="nematode_confocal_microscopy_image" width="300"/>
> Figure credits: María Eugenia Goya </p>
> 
> Can you come up with a descriptive, easy to sort, filename that fulfills the criteria descrribed above? Discuss in pairs.
> > ## Possible solution
> > One possible naming convention would be:  
> > 'YYYYMMDD-FS-TC-day_10-Ec_OP50_to_Ec_OP50-NL5901'
> > , where:  
> > * FS = Food Switching  
> > * TC = Time Course  
> > * Ec = *Escherichia coli*  
> >   
> > We have included the date of the sample, the type of experiment, experimental sampling date, the strain of the bacteria where the nematodes were grown and the bacteria to which they were switched to, and the nematode strain (We ommited *C. elegans* from the name because no other nematodes are used for the project). Total name length = 49 characters (well within our intended size!).
> {: .solution}
{: .challenge}

> ## After you have a plan
> Once you have set up your naming criteria, stick to it!  
{: .callout}

> ## Backup your project files and folders
> It is good data management practice to ensure that your files are regularly backed up.
{: .callout}

## Project organization and FAIR guidelines
Did you realise that the suggestions we made above mean that you are including valuable metadata as part of your folder and file names? As we mentioned in the [Introduction to Metadata episode](../04-intro-to-metadata), metadata provides valuable information for us and others to be able to interpret your research data. 
	
> ## Challenge - discussion (5 minutes)
> In groups, discuss:
> * how can planning project folder organisation and defining naming conventions help the process of FAIRification?
> * do you think including extra metadata to understand your conventions will be useful/necessary?
{: .challenge}


> ## Attribution
> Content of this episode was created using the following references as inspiration:  
> - [Organising your data](https://www.data.cam.ac.uk/data-management-guide/organising-your-data)  
> - [Organising files and folders](https://www.wur.nl/en/Value-Creation-Cooperation/Collaborating-with-WUR-1/Organising-files-and-folders.htm)  
> - [File naming](https://libguides.princeton.edu/c.php?g=102546&p=930626)  
> 
{: .callout}


{% include links.md %}
