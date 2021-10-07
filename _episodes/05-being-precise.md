---
title: "Being precise"
teaching: 10
exercises: 20
questions:
- "How to make my metadata interoperable?"
- "How to avoid disambiguation?"
objectives:
- "Using public identifiers"
- "Understand difference between close vocabulary and ontology"
- "Finding ontology terms"
keypoints:
- "Public identifiers and ontologies are key to knowledge discovery"
- "Automatic data aggregations needs standarised metadata formats and values"
---


## Being precise

If the metadata purpose is to help understand the data, it has
to be done in a precise and "understandable" way i.e. it has to be
interoperable. To be interoperable metadata should use
a ***formal, accessible, shared, and broadly applicable terms/language***
for knowledge representation.

One of the easiest examples is the problem of author disambiguation.

![Why we need ORCID](../fig/04-names-example.jpg)

*After [Libarary Carpentry FAIR Data](https://librarycarpentry.org/lc-fair-research/)*


> ## Open Researcher and Contributor ID (ORCID)
>
> Have you ever searched yourself in pubmed and found that you have a
> *doppelganger*? So how can you uniquely associate something you created
> to just yourself and no other researcher with the same name?
>
> [ORCID](https://orcid.org/) is a free, unique, persistent identifier that you own and control—forever.
> It distinguishes you from every other researcher across disciplines,
> borders, and time.
>
> ORCIDs of authors of this episode are:
> * [0000-0002-0194-5706](https://orcid.org/0000-0002-0194-5706)
> * [0000-0003-0737-2408](https://orcid.org/0000-0003-0737-2408)
>
> You can connect your iD with your professional information—affiliations,
> grants, publications, peer review, and more.
> You can use your iD to share your information with other systems,
> ensuring you get recognition for all your contributions,
> saving you time and hassle, and reducing the risk of errors.
>
> If you do not have an [ORCID](https://orcid.org/),
> you should register to get one!
>
{: .callout}

ORCID provides the registry of researchers, so they can be precisely identified.
Similarly, there are other registries that can be used to identify many
of biological concepts and entities:
* species e.g. [NCBI taxonomy](https://www.ncbi.nlm.nih.gov/Taxonomy)
* chemicals e.g. [ChEBI](https://www.ebi.ac.uk/chebi)
* proteins e.g. [UniProt](https://www.uniprot.org/)
* genes e.g. [GenBank](https://www.ncbi.nlm.nih.gov/genbank/)
* metabolic reactions, enzymes e.g [KEGG](https://www.genome.jp/kegg/)

[BioPortal](https://bioportal.bioontology.org/) or
[NCBI](https://www.ncbi.nlm.nih.gov/)  
are good places to start searching for a registry or a term.


> ## Public ID in action (3)
>
> Wellcome Open Research journal uses ORCID to identify authors.
> * Open one of our papers [doi.org/10.12688/wellcomeopenres.15341.2](https://doi.org/10.12688/wellcomeopenres.15341.2)
> and check how public IDs as ORCID can be used to interlink information.
>
> * If you have not done it yet, register yourself at ORCID*

>
> * The second metadata example (the Excel table):
> contains two other types of public IDs.  
> ![Metadata in data table example](../fig/04-metadatafull_spreadsheet.png)
> *Figure credits: Tomasz Zielinski and Andrés Romanowski*
>   
> 	- Can you find the public IDs?
> 	- Can you find the meaning behind those Ids?
>
>
> > ## Solution
> > ORCID is used to link to authors profiles which list their other
> > publications.
> >
> > The metadata example contains genes IDs from The Arabidopsis Information Resource
> > [TAIR](https://www.arabidopsis.org) and metabolites IDs from
> > [KEGG](https://www.genome.jp/kegg/compound/)
> >
> {: .solution}
{: .challenge}



> ## Attribution
>
> Content of this episode was adapted from:
{: .callout}

{% include links.md %}
