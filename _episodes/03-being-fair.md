---
title: "Being FAIR"
teaching: 0
exercises: 0
questions:
- "How to get more value from own data?"
- "What are the FAIR guidelines?"
- "Why being FAIR matters?"
objectives:
- "Recognize typical issues that prevents data re-use"
- "Understand FAIR principles"
- "Know steps for achieving FAIR data"
keypoints:
- "FAIR stands for Findable Accessible Interoperable Reusable"
- "FAIR assures easy access to data underlying scientific findings"
---

TODO some intro, maybe like:
Thanks to UK (?and EU?) funders polices there is a wide adoption of Open Access
and as the results easy access to the recent biomedical publications.
Unfortunately, the same cannot be said about data and software code
that underlines those publications.

> ## What is data
>
> Although scientific data is a very broad term we still encounter
> groups who (wrongly) believe they do not have data!
> -- maybe give the centre example unless we will use it somewhere else --
> Data are not only the Excel files recording measurements from a machine,
> date are also:
> * images, not only from microscopy
> * information about biological materials, like strain details
> * recipes, laboratory and measurement protocols
> * ?ARE THERE ANOTHER EXAMPLES?
> * scripts, analysis procedures, custom software can also be considered as data,
> although there are often specific recommendations how to deal with code.
>
{: .callout}

Let's have a look how difficult it is to find data from
published biological papers.

TODO:

> ## Impossible protocol 
>
> Imagine you have discovered a protein of interest during a RNA-seq or
> proteomics experiment and are wanting to validate your data via a
> western blot of your samples. That protein is Titin, the largest
> protein in the body with a molecular weight of 3,800 kDa, and you are
> now looking for protocols on how to best separate and transfer this
> large protein. You found an antibody that has been validated in
> western blots and immunofluorescence, have ordered it and are now
> looking through those publications which have successfully used it.
> Sigma Aldrich lists [this paper](https://doi.org/10.1002/acn3.50831)
> which uses their antibody.
> Can you find a complete protocol in their Methods under Western blot
> analysis (p. 1312), where their reference (ref 17) leads you to another
> publication?
>
>> ## Solution 
>>
>>  * Ref 17 will lead you to [this
>>     paper](https://doi.org/10.1002/ana.24102), which first of all is
>>     not open access
>>  * Access the paper through your institutions (if you can) and find
>>     the 'Western Blotting' protocol on page 232 which will show the
>>     following (Screenshot from the methods section from [Evilä et al 2014](https://doi.org/10.1002/ana.24102)):
>>  * ![Figure 1. Impossible Protocol](../fig/impossible_protocol.png) 
>>  * "Western blotting were performed according to standard methods." -
>>     with no further reference to these standard methods, describing
>>     these methods, or supplementary material detailing these methods
>>  * This methodology is unfortunately a true dead end and we thus
>>      can't easily continue our experiments!
>>
> {: .solution}
{: .challenge}

> ## Impossible numbers
>
> Defined here.
>
{: .challenge}

> ## Impossible resource/link
>
> Defined here.
>
{: .challenge}

> ## Impossible format
>
> Defined here.
>
{: .challenge}

TODO: As we saw the typical problems are: ....
To avoid such problems FAIR principles were designed.

![Figure 2. FAIR principles](../fig/FAIR.png)
After [SangyaPundir](https://commons.wikimedia.org/wiki/File:FAIR_data_principles.jpg)

> ## FAIR Principles
>
> In 2016, the [FAIR Guiding Principles for scientific data management and stewardship](https://www.nature.com/articles/sdata201618)
> were published in Scientific Data.
> The original guideline focused on "machine-actionability" -
> ability of computer system to operate on data with
> a minimal human intervention. However, currently the focus shifts
> to making data accessible from human perspective not an automated one
> (mostly due to the lack of user friendly tooling that could help
> dealing with standards and structured metadata).
>
> **Findable**:  Easy to find the data and the metadata for
> both humans and computers.
> Automatic and reliable discovery of datasets and services depends
> on machine-readable persistent identifiers (PIDs) and metadata.
>
> **Accessible**: The (meta)data retrievable by their identifier using
> a standardized and open communications protocol (including authentication
> and authorisation). Metadata should be available even when the data
> are no longer available.
>
> **Interoperable**: The data should be able to be combined with and used
> with other data or tools. The format of the data should be open and
> interpretable for various tools. It applies both to the data and
> metadata, the (meta)data should use vocabularies that follow FAIR principles.
>
> **Re-usable**: FAIR aims at optimizing the reuse of data.
> Metadata and data should be well-described so that they can be replicated
> and/or combined in different settings. The reuse of the (meta)data
> should be stated with clear and accessible license(s)
>
{: .callout}


## FAIR in biological practice

#### Findable & Accessible

Deposit data to an external, reputable public repository.

Repositories provide persistent identifiers (PIDs), catalogue options,
advanced metadata searching, download stats.

Some repositories can host also private data or provide embargo period.

There are general "data agnostic" repositories, for example:
[Dryad](http://datadryad.org),
[Zenodo](http://zenodo.org),
[FigShare](http://figshare.com),
[Dataverse](http://thedata.org)

Or domain specific, for example:
[UniProt](https://www.uniprot.org/) protein data,
[GenBank](https://www.ncbi.nlm.nih.gov/genbank/) sequence data,
[MetaboLights](https://www.ebi.ac.uk/metabolights/) metabolomics data.

*We will cover repositories in more details in a later episode.*


> ## What are persistent identifiers (PIDs)
>
> A persistent identifier is a long-lasting reference to a digital resource.
> Typically it has two components:
> * a service that locates the resource over time even when its location in the changes
> * and a unique identifier (that distinguishes the resource or concept from others).
>
> Persistent identifiers aim to solve the problem of the persistence of accessing cited resource,
> particularly in the academic literature. All too often, web addresses (links) changes over time
> and fail to take you to the referenced resource you expect.
>
> There are several services and technologies (schemas) that provide PIDs
> for objects (whether digital, physical or abstract).
>
> One of the most popular is **Digital Object Identifier [(DOI)]()**,
> recognizable by the prefix doi.org in the web links.
>
> For example: [https://doi.org/10.1038/sdata.2016.18](https://doi.org/10.1038/sdata.2016.18)
> resolves to the location of the paper that describes FAIR principles.
>
> Public repositories often maintain web addresses of their content in a stable form
> which follows the convention http://repository.adress/identifier;
> these are often called permalinks.
> For well establish services, permalinks can be treated as PIDs.
>
> For example: [http://identifiers.org/SO:0000167](http://identifiers.org/SO:0000167) resolves to a page
> defining promoter role and can be used to annotate part of DNA sequence
> as performinig such role during transcription.
>
{: .callout}


#### Interoperable

* Use common files formats (can be domain specific)
* Always use .csv or .xls files for numerical data.
Never make data tables in word or pdf,
* Provide underlying numerical data for all plots and graphs
* Convert proprietary binary formats to the open ones, for example
 convert Snapgene to Genbank, microscopy multistack images to OME-TIFF

#### Reusable

1. Attach licence file.
Generally, without an explicit licence the data
cannot not be re-used.
Here, we recommend:
    * for data [Creative Commons Attribution (CC BY)](https://creativecommons.org/licenses/by/4.0/)
licence,
    * for code a permissive open source license such
as the [MIT](https://opensource.org/licenses/MIT),
[BSD](https://opensource.org/licenses/BSD-2-Clause),
or [Apache license](http://www.apache.org/licenses/).

2. Describe your data well / provide good metadata
    * write README file describing the data
    * user descriptive column headers for the data tables
    * tidy data tables, make them analysis friendly
    * describe your data in details (prepare good metadata)
    * use (meta)data formats (e.g. SBML, SBOL)
    * follow Minimum Information Standards

*Describing data well is the most challenging part of the data sharing proces.
We will cover it in more details later on*

> ## FAIR and You
>
> The FAIR acronym is sometimes accompanied with the following labels:
> * Findable - Citable
> * Accessible - Trackable and countable
> * Interoperable - Intelligible
> * Reusable - Reproducible
>
> Using those labels as hints discuss how FAIR principles directly
> benefit you as the data creators.
>
>> ## Solution
>>
>> * Findable data have their own identity, so they can be easily
>> cited and secure the credits to authors
>> * Data accessible over the Internet using standard protocols can be
>> easily monitored (for example using Goolge analytics) and give metrics
>> on the data popularity or even geo-locations of data users.
>> * TODO I dont know intelligible benefit!!!
>> * Well documented data should contain all the details necessary to
>> reproduce the experiments, helping the future you or someone taking over
>> you in the laboratory.
>>
> {: .solution}
{: .challenge}

> ## TODO example of FAIR data
>
> Idea. Look at the record of X in Uniprot (link).
> Identify how each of F.A.I.R principles has been met.
>
>> ## Solution
>>
>> Record has id which makes it Findable. It can downloaded in X formats
>> making it Accessible and Interoperable. TODO...
> {: .solution}
{: .challenge}


> ## FAIR Quiz
>
> Which of the following statement are true/false.
>
> * F in FAIR stands for Free F
>
> * Even if there is no license information you can combine the data
> with yours to produce a plot as long as you name the other authors F
>
> * Only figure presenting results of statistical analysis need
> numerical data that were used to create that figure F
>
> * Sharing numerical data as pdf in Zenodo is FAIR F
>
> * Sharing numerical data as Excel via Github is not FAIR F*
>
> * Metadata standards (for example MIAME MIQUE) assure IR in FAIR T
>
> * Group website is one the best place to share your data F
>
> * Data from failed experiments are not re-usable F
>
> * Data should always be converted to excel or cvs in order to be FAIR F
>
> * DOI of a dataset helps in getting credit T
>
> * FAIR data are peer reviewed F
>
> * FAIR data have to accompany a publication F
>
>> ## Solution
>> copied form above once the wording is corrected
>>
> {: .solution}
{: .challenge}


{% include links.md %}

