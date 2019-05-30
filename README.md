## The quiz: Are you using the data science tool kit for open science?

**Evaluate your use of the data science tool kit. [Test](https://ca.research.net/r/6FG22QJ)**

### Explantion of how we marked the test

Have suggestions or thoughts? Send your comments through [issues](https://github.com/DougManuel/ds-presentation/issues)

#### 1) Open software

There are many data science software programs, each with its strength. Data scientists typically use multiple programs, but open software is the defacto way to share code with others. 

The two leading software packages for data science are R and Python. Julia is also open-source with rapid adoption. There are thousands and thousands of code packages that are publicly available in code repositories for R and Python. These code respositories have well-established guidelines for how to write and document code for sharing. A rich tool kit of supporting libraries are available to make it easy for you to adopt these best practices, including creating documentation, cleaning and linting your code, checking and testing for errors. 

A collection of several related presentations on data science. Each branch represents a presentation for a specific audience. 

#### 2) Coding style

Code is easier to read if it is written in a consistent style that includes naming variables, functions and how to using spaces. There are common style guides that are used for different languages or within institutions. For example, [Google](http://google.github.io/styleguide/) publishes their style guides for all major program languages. Try to the same style guide within your organization or collegues.

#### 3) Documenting your code

Documenting your analysis code is more than making comments within the program code explaining the steps or sections. See [blog post](https://www.divio.com/blog/documentation/) by Daniele Procida for a description of the four components of good documentation: tutorials, how-to guides, explanation and technical reference. 

> "It doesn’t matter how good your software is, because if the documentation is not good enough, people will not use it."

*Daniele Procida*. [What nobody tells you about documentation](https://www.divio.com/blog/documentation/)

#### 4) Code notebooks

Code notebooks like Juypter and rMarkdown are a great way to share code. You combine code snippets in a docment that is easy to read. The code snippets can be executed by your reader -- and modified by them if they wish to explore how the code works. The notebooks are easily shared on websites. 

We like rMarkdown because you can not only create notebooks but also [online books](https://bookdown.org/yihui/bookdown/), [blog](https://bookdown.org/yihui/blogdown/), (code package documentation)[https://pkgdown.r-lib.org/] and other documents.

#### 5) Check your code

Errors in code is (enivable)[https://www.mayerdan.com/ruby/2012/11/11/bugs-per-line-of-code-ratio]. The more code you write, the more eerors you'll have in your code. Remember, your data science projects are becoming increasingly complex, with more and larger data and more collaborations. 

Fortunately, there are tools to help you reduce the number of errors you write. In our teams, we check each others code if we plan to reuse it more than once or share it with others. We use linters, checkers and [tests](https://testthat.r-lib.org). As a back-up, we deploy program these tools using [continuous integration](https://travis-ci.org) before code is shared by others.

#### 6 to 8) Git and Git repositories

Git and Git repositories have the most points in our test. When we talk about Git terms like "linchpin" and "glue" come up. Many parts of the open science tool kit would look considerably less developed without Git. There are other version control systems but Git is really the only system that is used for new projects.

Git is difficult to learn, but everyone who learns it is glad they did. Using git will save you time and heartache -- any investment in your time will be returned to you many, many fold.

Git repositories like GitHub and Gitlab is how data scientist colloborate across the world. 

There are many [guides](http://kbroman.org/github_tutorial/) and [tips](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4945047/) for using git and git repositories. Keep your eyes open for the increasing number of resources for people like you (hint: many resources are for software developers in business). 

We have created some resources for health researchers. [Getting started with Git.](https://github.com/Big-Life-Lab/GettingStartedWithGit)

#### 9) Metadata

You may be suprized to see a question about metadata on the test. This is a rapidly developming area that data scientist are paying more attention. Data without context is meaningless -- metadata provide that context. Metadata tells you about your data: where it came from (data provance) and what it contains. 

Fortunately, many sources of data come with standarized metadata. For example, there are over ten thousand databases with 5 million variables available at [ICPSR](https://www.icpsr.umich.edu/icpsrweb/), all with metadata encoded using the Data Documentation Initiative((DDI)[https://www.ddialliance.org]). Aim to publish your results with metadata to allow machine-actionable uses of your research, in addition to ensure reliable reproduciblity and transparency. For example, we publish our algorihtms using Predictive Modelling Mark-up Language ((PMML)[http://dmg.org]). 

A challenge is a lack of well-developed tools to use metadata in your project (beyond variable and category lables). We've created an [R library](http://bllflow.projectbiglife.ca) that helps use and maintain metadata.

## Imperitives

### Internationally, a growing voice of concern about research reproducitibity

> “Academic institutions can and must do better. We should be taking multiple approaches to make science more reliable.”

*Jeffrey Flier*. Dean of Medicine, Harvard University. Nature 549, 133 (2017)

>“Put simply, this means that researchers should make their computational workflow and data available for others to view. 
> They should include the code used to generate published figures and omit only data that cannot be released for privacy or legal reasons.”

*Jeffrey M. Perkel*. A toolkit for data transparency takes shape. Nature 560, 513-515 (2018)

>"More than 70% of researchers have tried and failed to reproduce another scientist's experiments, and more than half have failed to reproduce their own experiments."

*Monya Baker*. 1,500 scientists lift the lid on reproducibility. Nature 533, 452-4 (2016)

## Our repository

*[bllflow](https://bllflow.projectbiglife.ca)* - an R package for efficient, transparent data prepartion and reporting.

## Panel presentation

The quiz was part of the data science panel at the [2019 CAHSPR meeting](https://www.cahspr.ca). The [presentation and further information](https://github.com/DougManuel/ds-presentation/tree/CASPHR2019-panel).

## References

### General

1) Donoho D, 50 years of Data Science. [Sept. 18, 2015](http://courses.csail.mit.edu/18.337/2015/docs/50YearsDataScience.pdf)

1) Stukel TA, Austin PC, Azimaee M, Bronskill SE, Guttmann A, Paterson JM, Schull MJ, Sutradhar R, Victor JC. _Envisioning a Data Science Strategy for ICES_. Toronto, ON: Institute for Clinical Evaluative Sciences; 2017. [ISBN: 978-1-926850-77-1](https://www.ices.on.ca/Publications/Atlases-and-Reports/2017/Data-science-strategy)

1) Rumsfeld JS, Joynt KE, Maddox TM. Big data analytics to improve cardiovascular care: promise and challenges. Nature reviews Cardiology. 2016;13(6):350-9.

1) Wilson G, Aruliah DA, Brown CT, Chue Hong NP, Davis M, Guy RT, et al. Best practices for scientific computing. [PLoS Biol](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745). 2014;12(1):e1001745. 

1) Hicks SC, Irizarry RA. A Guide to Teaching Data Science. The American Statistician. 2017;72(4):382-91.
[10.1080/00031305.2017.1356747](https://www.tandfonline.com/doi/full/10.1080/00031305.2017.1356747)

   
### Open Science

1) Flier, J. (2017). Faculty promotion must assess reproducibility. Nature, 549(7671), 133. [doi:10.1038/549133](https://www.nature.com/news/faculty-promotion-must-assess-reproducibility-1.22596)

1) Perkel, J. M. (2018). A toolkit for data transparency takes shape. [Nature, 560, 513-515](https://www.nature.com/articles/d41586-018-05990-5).

1) Baker, M. 1,500 scientists lift the lid on reproducibility. [Nature 533, 452-4 (2016)](https://www.nature.com/news/1-500-scientists-lift-the-lid-on-reproducibility-1.199700.

1) Woelfle, M.; Olliaro, P.; Todd, M. H. (2011). Open science is a research accelerator. Nature Chemistry. 3: 745–748. [doi:10.1038/nchem.1149](https://www.nature.com/articles/nchem.1149)

1) Stodden, V., McNutt, M., Bailey, D. H., Deelman, E., Gil, Y., Hanson, B., . . . Taufer, M. (2016). Enhancing reproducibility for computational methods. Science, 354(6317), 1240-1241. [doi:10.1126/science.aah6168](http://science.sciencemag.org/content/354/6317/1240.long)

1) Kopt D. This year’s Nobel Prize in economics was awarded to a Python convert. [qz.com](https://qz.com/1417145/economics-nobel-laureate-paul-romer-is-a-python-programming-convert/) Oct 2018.

1) Somers J. The Scientific Paper Is Obsolete: Here's what's next. [The Atlantic](https://www.theatlantic.com/science/archive/2018/04/the-scientific-paper-is-obsolete/556676/) Apr 2018.

1) Kitzes J, Turek D, Deniz F. _The practice of reproducible research: case studies and lessons from the data-intensive sciences_. [Univ of California Press](https://legacy.gitbook.com/book/bids/the-practice-of-reproducible-research/details); 2017.

1) Pioneering ‘live-code’ article allows scientists to play with each other’s results. [Nature](https://www.nature.com/articles/d41586-019-00724-7)


### Git and version control

1) Perez-Riverol Y, Gatto L, Wang R, Sachsenberg T, Uszkoreit J, Leprevost Fda V, et al. Ten Simple Rules for Taking Advantage of Git and GitHub. [PLoS Comput Biol](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4945047/). 2016;12(7):e1004947.

1) [Git/Github guide](http://kbroman.org/github_tutorial/)

1) [Version control with Git](https://swcarpentry.github.io/git-novice/)

1) [Git and GitHub learning resources](https://help.github.com/en/articles/git-and-github-learning-resources)

1) [Integration of GitHub with SAS](https://analytics.ncsu.edu/sesug/2013/PA-04.pdf)

1) [Gitkraken](https://www.gitkraken.com/git-client) (the Git client our team uses)

### Code documentation

1) What nobody tells you about documentation. Divio Blog. [Accessed Nov 2018](https://www.divio.com/blog/documentation)

1) [Jupyter Notebooks](https://jupyter.org/)

1) [Why Jupyter is data scientist’ computational notebook of choice](https://www.nature.com/articles/d41586-018-07196-1)

1) [Introduction to R Markdown](http://rmarkdown.rstudio.com/articles_intro.html) 

1) [R Markdown: The definitive guide](https://bookdown.org/yihui/rmarkdown/)

1) [R Markdown cheat sheet](https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf)

1) [Advantages to using R Markdown for data analysis over Jupyter Notebooks](https://minimaxir.com/2017/06/r-notebooks/)

### Programming

1) [Population Health Data Science with R. Tomas J Argon](https://bookdown.org/medepi/phds/)

1) [R for Data Science](http://r4ds.had.co.nz/index.html). G Grolemund and H Wickham

1)  [Efficient R programming]([https://csgillespie.github.io/efficientR/). C Gillespie, R Lovelace

1) [R for Data Science- Chapter 19: Functions](http://r4ds.had.co.nz/functions.html ). G Grolemund, H Wickham

### Metadata

1) IBM developerWorks. What is PMML? [Accessed 2018](https://www.ibm.com/developerworks/library/ba-ind-PMML1/).
