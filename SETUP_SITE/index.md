# Bio3d

## Overview  

<img src="http://thegrantlab.org/bio3d_v2/images/geostas_nma-v6-small.png" align="right" alt="" width="220"/>  

Bio3D is an [R package]() containing utilities for the analysis of protein structure, sequence and trajectory data.   

It is currently distributed as platform independent source code under the [GPL version 3 license](). Major features include:  

- The ability to read, write and process biomolecular structure, sequence and dynamics trajectory data. [>> more](reference/index.html#section-input-output)  
- Perform atom selection, alignment and superposition, rigid core identification, dynamic domain analysis, conformational clustering, correlation network analysis, torsion analysis, distance matrix analysis and principal component analysis of structure data. [>> more](reference/index.html#section-structure-analysis)   
- Perform ensemble normal mode analysis on large structure sets to explore evolutionary dynamics and structure dependent protein flexibility. [>> more](reference/index.html#section-normal-mode-analysis)   
- Perform conservation analysis of sequence and structural data. [>> more](reference/index.html#section-sequence-analysis)   
- Integration of major protein structure and sequence databases and associated search tools. [>> more](reference/index.html#section-utilities)  
- In addition, various utility functions are provided to enable the statistical and graphical power of the R environment to work with biological sequence and structural data. [>> more](reference/index.html#section-graphics)  

## Quick Install

On all platforms (Mac, Linux, and PC) open R (version 3.1.0 or higher) and use the function `install.packages("bio3d")` at the R command prompt to install the package from your local CRAN site:

```
install.packages("bio3d", dependencies=TRUE)
```

For more detailed installation and setup instructions please see the [Installing Bio3D](articles/online/install_vignette/Bio3D_install.html) page. 


## Getting Started

First time users may find our [getting started guide](articles/online/intro_vignette/Bio3D_introduction.html) helpful.

We also distribute a number of extended [**Bio3D vignettes**](articles/index.html) that provide worked examples of using Bio3D to perform a particular type of analysis. There is also a <a href="https://cran.r-project.org/web/packages/bio3d/bio3d.pdf">package manual</a> (in PDF format) that is a concatenation of each [functions documentation](reference/index.html). 


## Development

For information on current and future development of Bio3D, see the [Bio3D project on BitBucket](https://bitbucket.org/Grantlab/bio3d/). Details of recent package changes and [reported issues](https://bitbucket.org/Grantlab/bio3d/issues?status=new&status=all) can also be found on BitBucket.  


## Citing Bio3D

Bio3D: An R package for the comparative analysis of protein structures.  
Grant, Rodrigues, ElSawy, McCammon, Caves, (2006) *Bioinformatics* 22, 2695-2696   
( [Abstract](http://bioinformatics.oxfordjournals.org/cgi/content/abstract/22/21/2695) | [PubMed](http://www.ncbi.nlm.nih.gov/entrez/query.fcgi?cmd=retrieve&db=pubmed&list_uids=16940322&dopt=Abstract) | [PDF](http://bioinformatics.oxfordjournals.org/content/22/21/2695.full.pdf) | [BibTeX](authors.html) )  

Integrating protein structural dynamics and evolutionary analysis with Bio3D.
Skjærven, Yao, Scarabelli, Grant, (2014) *BMC Bioinformatics* 15, 399  
( [Abstract](http://www.biomedcentral.com/1471-2105/15/399/abstract) | [PubMed](http://www.ncbi.nlm.nih.gov/pubmed/25491031) | [PDF](http://www.biomedcentral.com/content/pdf/s12859-014-0399-6.pdf) )  

Online interactive analysis of protein structure ensembles with Bio3D-web.
Skjærven, Jariwala, Yao, Grant, (2016) *Bioinformatics* 32, 3510-3512  
( [Abstract](http://bioinformatics.oxfordjournals.org/content/early/2016/07/14/bioinformatics.btw482.abstract) | [PubMed](http://www.ncbi.nlm.nih.gov/pubmed/27423893) | [PDF](http://bioinformatics.oxfordjournals.org/content/early/2016/07/14/bioinformatics.btw482.full.pdf) )  

The Bio3D packages for structural bioinformatics.  
Grant, Skjærven, Yao (2020) *Protein Science*, In press.  
( [Abstract](https://onlinelibrary.wiley.com/doi/abs/10.1002/pro.3923) | [PubMed](https://pubmed.ncbi.nlm.nih.gov/32734663/) | [PDF](https://onlinelibrary.wiley.com/doi/epdf/10.1002/pro.3923) )  



