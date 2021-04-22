---
title: "Introduction to metadata"
teaching: 15
exercises: 15
questions:
- "What is metadata?"
- "What do we use metadata for?"
- "Is metadata important for data Reuse (the **R** in FAIR)?"
objectives:
- "Recognise what metadata is"
- "Distinguish different types of metadata"
- "Recognise how to provide metadata"
- "Recognise how FAIR guidelines apply to metadata"
keypoints:
- "Metadata provides contextual information so that other people understand our data."
- "Metadata is key for data reuse."
- "Metadata can be included as a standalone ReadMe.txt file or included as a header on a data file"
output: html_notebook
editor_options: 
  chunk_output_type: inline
---

## What is (or are) metadata?

Simply put, metadata is the data about the data. Does this sound
confusing? Let's clarify: metadata is the *description of your data*. It
allows others to gain deeper understanding about your data and provides
insight for its interpretation. Hence, you should consider your metadata
as important as your data. Further, metadata plays a very important role
in making your data FAIR. It has to be continuously added to your
research data (not just at the beginning or end of your project!).
Metadata can be produced in an automated way (e.g.: when you create a
microscopy image usually the accompanying software saves metadata on it)
or manually.

<ins>Let's take a look at an example:</ins>

This is a confocal microscopy image of a *C. elegans* nematode strain used
as a proteostasis model (Pretty! Isn't it?). The image is part of the raw data
associated to [Goya et al., 2020](https://doi.org/10.1016/j.celrep.2019.12.078),
which was deposited in a [Public Omero Server](https://publicomero.bio.ed.ac.uk/).

<img src="../fig/04-microscopy_with_metadata.png" alt="nematode_confocal_microscopy_image" width="600"/>

Let's see the associated metadata to the image and the dataset to which it belongs:
  
> ## Image metadata  
>  
> Name: OP50 D10Ad_06.czi  
> Image ID: 3485  
> Owner: Maria Eugenia Goya  
> ORCID: 0000-0002-5031-2470
>
> Acquisition Date: 2018-12-12 17:53:55  
> Import Date: 2020-04-30 22:38:59  
> Dimensions (XY): 1344 x 1024  
> Pixels Type: uint16  
> Pixels Size (XYZ) (µm): 0.16 x 0.16 x 1.00  
> Z-sections/Timepoints: 56 x 1  
> Channels: TL DIC, TagYFP  
> ROI Count: 0
>
> Tags: time course; day 10; adults; food switching; E. coli OP50;
> NL5901; C. elegans
>
> ## Dataset metadata
>  
> Name: Figure2_Figure2B  
> Dataset ID:	263  
> Owner: Maria Eugenia Goya  
> ORCID: 0000-0002-5031-2470
>  
>
> Description:  
> The datasets contains a time course of α-syn aggregation in NL5901 C.
> elegans worms after a food switch at the L4 stage:
>
> E. coli OP50 to OP50  
> Day 01 adults  
> Day 03 adults  
> Day 05 adults  
> Day 07 adults  
> Day 10 adults  
> Day 13 adults  
>
> E. coli OP50 to B. subtilis PXN21  
> Day 01 adults  
> Day 03 adults  
> Day 05 adults  
> Day 07 adults  
> Day 10 adults  
> Day 13 adults  
>
> Images were taken at 6 developmental timepoints (D1Ad, D3Ad, D5Ad,
> D7Ad, D10Ad, D13Ad)
>
> \* Some images contain more than one nematode.
>
> Each image contains   ~30 (or more) Z-sections, 1 µmeters apart. The
> TagYFP channel is used to follow the alpha-synuclein particles. The TL
> DIC channel is used to image the whole nematode head.
>
> These images were used to construct Figure 2B of the Cell Reports
> paper (<https://doi.org/10.1016/j.celrep.2019.12.078>).
>  
> Creation date: 2020-04-30 22:16:39
>  
> Tags: protein aggregation; time course; E. coli OP50 to B. subtilis PXN21; food switching; E. coli OP50;
> 10.1016/j.celrep.2019.12.078; NL5901; C. elegans
{: .callout}

This is a lot of information!

> ## Challenge
>
> -  Which information could you have guessed without the metadata?
> -  Discuss in pairs: 
> 	* how useful do you believe metadata is?
>	* should metadata be included with public datasets?
>
{: .challenge}

> ## Distinguishing data from metadata
>
> What is "data" and what is "metadata" is thereby a matter of
> perspective: Some researchers' metadata can be other researchers'
> data.
>
{: .callout}

## Types of metadata

According to [How to FAIR](https://howtofair.dk/) we can distinguish
between three main types of metadata:  
* **Administrative metadata:** are data about a project or resource
that are relevant for managing it; for example, project/ resource owner,
principal investigator, project collaborators, funder, project period,
etc. They are usually assigned to the data, before you collect or create
them.
* **Descriptive or citation metadata:** are data about a dataset or
resource that allow people to discover and identify it; for example,
authors, title, abstract, keywords, persistent identifier, related
publications, etc.
* **Structural metadata:** are data about how a dataset or resource
came about, but also how it is internally structured. Structural
metadata describe, for example, the unit of analysis, collection method,
sampling procedure, sample size, categories, variables, etc. Structural
metadata have to be gathered by the researchers according to best
practice in their research community and will be published together with
the data. Descriptive and structural metadata should be added
continuously throughout the project.


> ## Identifying metadata types
> Here we have an excel spreadsheet that contains project metadata for a made-up experiment
> ![metadata-full-spreadhseet](../fig/04-metadatafull_spreadsheet.png)
>
> In groups, identify different types of metadata used in this example.
> > ## Solution
> > * Administrative metadata appears in blue
> > * Descriptive metadata appears in orange
> > * Structural metadata appears in grey
> >![metadata-full-spreadhseet](../fig/04-metadatafull_spreadsheet_solution.png)
> {: .solution}
>  
> Optional: in groups, now repeat the excercise for the example of the previous section.
{: .challenge}

> ## Open Researcher and Contributor ID (ORCID)
> 
> Have you ever done a search in pubmed and found that you have
> *doppelganger*? So how can you uniquely associate something you created
> to just you and no other researcher that has the same name?
> Do not worry, there is a solution to that! It is called an ORCID. 
> An [ORCID](https://orcid.org/) is a unique identifier that links the resources 
> you produced with you.
>
> If you do not have an [ORCID](https://orcid.org/), you should consider getting one!
>
{: .callout}

## Metadata standards

Many fields have a set of defined ways in which to structure their
metadata (this ensures it is consistent among the researchers of the
field, and helps with machine readibility of metadata). A list of
metadata standards can be found at the [The Digital Curation
Center](http://www.dcc.ac.uk/resources/metadata-standards/list).

What can you do if there are no metadata standards defined for your
data / field of research? Think about the minimum information that
someone else (from your lab or from any other lab in the world) would
need to know about your dataset to be able to work with it without any
further inputs from you.

> ## Metadata and FAIR guidelines - discussion
> 
> In groups, discuss how metadata can help the process of FAIRification.
>  
{: .challenge}


> ## Attribution
>
> Content of this episode was adopted from: 
> - [Metadata - FAIR data for climate sciences](https://escience-academy.github.io/Lesson-FAIR-Data-Climate/metadata/index.html).
> - [Metadata - HOWTO FAIR](https://howtofair.dk/how-to-fair/metadata/)
> - [Data Tidiness](https://datacarpentry.org/organization-genomics/01-tidiness/index.html)
{: .callout}

{% include links.md %}
