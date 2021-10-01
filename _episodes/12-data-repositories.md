---
title: "Public repositories"
teaching: 10
exercises: 20
questions:
- "Where can I deposit datasets?"
- "What are general data repositories?"
- "How to find a repository?"
objectives:
- "See the benefits of using research data repositories."
- "Differentiate between general and specific repositories."
- "Find a suitable repository."
keypoints:
- "Repositories are the main means for sharing research data."
- "You should use data-type specific repository whenever possible."
- "Repositories are the key players in data reuse."
---

## What are research data repositories?
Research data repositories are online repositories that enable the preservation, curation and publication of research 'products'. These repositories are mainly used to deposit research 'data'. However, the scope of the repositories is broader as we can also deposit/publish 'code' or 'protocols' (as we saw with protocols.io). 

There are general "data agnostic" repositories, for example:
* [Dryad](http://datadryad.org),
* [Zenodo](http://zenodo.org),
* [FigShare](http://figshare.com),
* [Dataverse](http://thedata.org).

Or domain specific, for example:
* [UniProt](https://www.uniprot.org/) protein data,
* [GenBank](https://www.ncbi.nlm.nih.gov/genbank/) sequence data,
* [MetaboLights](https://www.ebi.ac.uk/metabolights/) metabolomics data
* [GitHub](https://github.com/) for code.
 
Research outputs should be submitted to discipline/domain-specific repositories whenever it is possible. When such a resource does not exist, data should be submitted to a 'general' repository.
Research data repositories are a key resource to help in data FAIRification as they
assure Findability and Accessibility.

> ## Challenge 1. The general repository (5 minutes).
> Have a look at the following record for data set in Zenodo repository:
> [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5045374.svg)](https://doi.org/10.5281/zenodo.5045374)  
> What elements make it FAIR?    
>   
> > ## Solution  
> > The elements that make this deposit FAIR are:  
> >   
> > Findable:  
> > - F1. (Meta)data are assigned a globally unique and persistent identifier - YES  
> > - F2. Data are described with rich metadata (defined by R1 below)- YES  
> > - F3. Metadata clearly and explicitly include the identifier of the data they describe - YES  
> > - F4. (Meta)data are registered or indexed in a searchable resource - YES  
> >   
> > Accessible:  
> > - A1. (Meta)data are retrievable by their identifier using a standardised communications protocol - YES  
> > - A2.  Metadata are accessible, even when the data are no longer available - YES  
> >   
> > Interoperable:  
> > - I1. (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation. - YES  
> > - I2. (Meta)data use vocabularies that follow FAIR principles - PARTIALLY  
> > - I3. (Meta)data include qualified references to other (meta)data - YES  
> >   
> > Reusable:  
> > - R1. (Meta)data are richly described with a plurality of accurate and relevant attributes - YES  
> > 	- R1.1. (Meta)data are released with a clear and accessible data usage license - YES  
> > 	- R1.2. (Meta)data are associated with detailed provenance - YES  
> > 	- R1.3. (Meta)data meet domain-relevant community standards - YES/PARTIALLY  
> >    
> {: .solution}
{: .challenge}

> ## Challenge 2. Datasets discovery (4 minutes).  
>  
> Can you easily find similar data sets in Zenodo? Try to find an interesting dataset for you  
>   
> Hint 1: Verify the completeness/richness of the associated metadata. Is it complete? Are some bits missing?   
> Hint 2: Does the dataset include a ReadMe.txt file?   
>  
> > ## Solution
> > Zenodo is a good place to keep your data separate from paper. It gives access to all files, allowing you to cite the data as well (or instead of) the paper.  
> > However, it is not good for disovery, and does not enforce most metadata!  
> >   
> {: .solution}
{: .challenge}

> ## Minimal data set   
> Minimal data set to consist of the data required to replicate all study findings reported 
> in the article, as well as related metadata and methods.
>
> * The values behind the means, standard deviations and other measures reported;
> * The values used to build graphs;
> * The points extracted from images for analysis.
>
> (no need for raw data if the standard in the field is to share data that have been processed)
>
> [PLOS](https://journals.plos.org/plosbiology/s/data-availability)  
>  
{: .callout}

> ## Challenge 3. Domain specific repositories (4 minutes).  
>  
> Select one of the following repositories based on your expertise/interests:  
>  
> - Have a look at mRNAseq accession 'E-MTAB-7933' in [ArrayExpress](https://www.ebi.ac.uk/arrayexpress/experiments/E-MTAB-7933/)  
> - Have a look at microscopy 'project-1101' in [IDR](https://idr.openmicroscopy.org/webclient/?show=project-1101)  
> - Have a look at the synthethic part record 'SubtilinReceiver_spaRK_separated' within the 'bsu' collection in [SynBioHub](https://synbiohub.org/public/bsu/SubtilinReceiver_spaRK_separated/1)  
> - Have a look at the proteomics record 'PXD013039' in [PRIDE](https://www.ebi.ac.uk/pride/archive/projects/PXD013039)  
> - Have a look at the metabolomics record 'MTBLS2289' in [Metabolights](https://www.ebi.ac.uk/metabolights/MTBLS2289/descriptors)  
> - Have a look at the scripts deposit 'RNA-Seq-validation' in [GitHub](https://github.com/PauloFlores/RNA-Seq-validation)  
>  
> Report to the group, what advantages can you see in using a specific repository over a generalist repository like Zenodo.
> 
>> ## Solution
>> Some advantages are:
>> *   The repository is more relevant to your discipline than a generalist one.
>> *   Higher exposure (people looking for those specific types of data will usually first look at the specific repository).
>> *   Higher number of citations (see above).
> {: .solution}
{: .challenge}

## How do we choose a research data repository?
As a general rule, your research needs to be deposited in discipline/data specific repository. If no specific repository can be found, then you can use a generalist repository. Having said this, there are tons of data repositories to choose from. Choosing one can be time consuming and challenging as well.
So how do you go about finding a repository:
- Check the publisher's / funder' recommended list of repositories, some of which can be found below:
	- [BioMed Central / Springer Nature](https://www.springernature.com/gp/authors/research-data-policy/recommended-repositories)
	- [eLife](https://submit.elifesciences.org/html/elife_author_instructions.html#policies)
	- [Elsevier](https://www.elsevier.com/about/policies/research-data)
	- [EMBO Press](https://www.embopress.org/page/journal/14602075/authorguide#datadeposition)
	- [F1000 Research](https://f1000research.com/for-authors/data-guidelines)
	- [GIGAscience - OUP](https://academic.oup.com/gigascience/pages/instructions_to_authors)
	- [PLoS](https://journals.plos.org/plosbiology/s/recommended-repositories)
	- [Scientific Data - Nature](https://www.nature.com/sdata/policies/repositories)
	- [Taylor and Francis](https://authorservices.taylorandfrancis.com/data-sharing-policies/repositories/)
	- [BBSRC](https://bbsrc.ukri.org/research/resources/)
	- [NERC](https://nerc.ukri.org/research/sites/environmental-data-service-eds/policy/)
	- [Royal Society](https://royalsociety.org/journals/ethics-policies/data-sharing-mining/)
	- [Wellcome Open Research](https://wellcomeopenresearch.org/for-authors/data-guidelines)  
   
- Check [Fairsharing recommendations](https://fairsharing.org/recommendations/?q=)
	- alternatively, check the [Registry of research data repositories - re3data](https://www.re3data.org/)

> ## Challenge 4. Finding a repository (4 minutes).
>
> a) Find a repo for genomics data.  
> b) Find a repo for microscopy data.  
> Note to instructor: Fairsharing gives few options, people may give different answer follow up why they selected particular ones.
>
>> ## Solution  
>>  
>> a) GEO/SRA and ENA/ArrayExpress are good examples. Interestingly these repositories do not issue a DOI.  
>> b) IDR and UoE Public Omero are good examples. Once again, these repositories do not issue a DOI.  
> {: .solution}  
{: .challenge}  

A list of UoE BioRDM's recommended data repositories can be found [here](https://www.wiki.ed.ac.uk/display/RDMS/Suggested+data+repositories).

> ## What comes first? the repository or the metadata?
> Finding a repository first may help in deciding what metadata to collect and how!  
>   
{: .callout}  
  
> ## Extra features
> It is also worth considering that some repositories offer extra features, such as running simulations or providing visualisation. For example, [FAIRDOMhub](https://fairdomhub.org/) can run model simulations and has project structures. Do not forget to take this into account when choosing your repository. Extra features might come in handy.  
>  
{: .callout}  
  
> ## Can GitHub be cited?  
> To make your code repositories easier to reference in academic literature, you can create persistent identifiers for them. Particularly, you can use the data archiving tool in Zenodo to archive a GitHub repository and issue a DOI for it.  
>  
{: .callout}  

## Evaluating a research data repository
You can evaluate the repositories by following this criteria:
- who is behind it, what is its funding
- quality of interaction: is the interaction for purposes of data deposit or reuse efficient, effective and satisfactory for you?
- take-up and impact: what can I put in it? Is anyone else using it? Will others be able to find stuff deposited in it? Is the repository linked to other data repositories so I don't have to search tehre as well? Can anyone reuse the data? Can others cite the data, and will depositing boost citations to related papers?  
- policy and process: does it help you meet community standards of good practice and comply with policies stipulating data deposit? 

An interesting take can be found at Peter Murray-Rust's blog post [Criteria for succesful repositories](https://blogs.ch.cam.ac.uk/pmr/2011/08/19/criteria-for-successful-repositories/).
    
    
> ## Challenge 5, Wrap up discussion (3 minutes).
> Discuss the following questions:
> - Why is choosing a domain specific repositories over zenodo more FAIR?
> - How can selecting a repository for your data as soon as you do an experiment (or even before!) can benefit you research and help your data become FAIR?
> - What's your favourite research data repository? Why?
>
{: .challenge}


> ## Attribution
> Content of this episode was adapted or inspired by:.
> - [FAIR principles](https://www.go-fair.org/fair-principles/)
> - [BioRDM suggested data repositories](https://www.wiki.ed.ac.uk/display/RDMS/Suggested+data+repositories)
> - [DCC - How can we evaluate data repositories?](https://www.dcc.ac.uk/news/how-can-we-evaluate-data-repositories-pointers-dryaduk)
> - [Criteria for succesful repositories](https://blogs.ch.cam.ac.uk/pmr/2011/08/19/criteria-for-successful-repositories/)
{: .callout}


{% include links.md %}
