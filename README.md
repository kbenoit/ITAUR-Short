## Quantitative Text Analysis Using R


#### GESIS Computational Social Science Winter Symposium, Köln (Cologne), 1 December 2015

[Kenneth Benoit](kbenoit@lse.ac.uk), Department of Methodology, LSE  
[Paul Nulty](p.nulty@lse.ac.uk), Department of Methodology, LSE  

**Version:** 30 November 2015

This repository contains the workshop materials for the short workshop [Quantitative to Text Analysis Using R](http://www.gesis.org/css-wintersymposium/program/workshops-tutorials/quantitative-text-analysis-using-r/) taught on December 1, 2015 by Kenneth Benoit and Paul Nulty.  This workshop is part of the pre-conference training sessions of the GESIS Computational Social Science Winter Symposium, 1-3 December 2015.  Ken Benoit and Paul Nulty's involvement is supported through European Research Council grant ERC-2011-StG 283794-QUANTESS.

### Instructions for using this resource ###

You have three options for downloading the course material found on this page:  

1.  You can download the materials by clicking on each link.  

2.  You can "clone" repository, using the buttons found to the right side of your browser window as you view this repository.  This is the button labelled "Clone in Desktop".  If you do not have a git client installed on your system, you will need to [get one here](https://git-scm.com/download/gui) and also to make sure that [git is installed](https://git-scm.com/downloads).  This is preferred, since you can refresh your clone as new content gets pushed to the course repository.  (And new material will get actively pushed to the course repository at least once per day as this course takes place.)

3.  Statically, you can choose the button on the right marked "Download zip" which will download the entire repository as a zip file.

You can also subscribe to the repository if you have [a GitHub account](https://github.com), which will send you updates each time new changes are pushed to the repository.

### Objectives

This workshop covers how to perform common text analysis and natural language processing tasks using R.  When used properly, R is a fast and powerful tool for managing even very large text analysis tasks.  

The course consists of instructor presentations in three sets, followed by exercises that students are meant to do in class.  Computers should be available, but we suggest you bring your own.

We will cover how to format and input source texts, how to structure their metadata, and how to prepare them for analysis.  This includes common tasks such as tokenisation, including constructing ngrams and "skip-grams", removing stopwords, stemming words, and other forms of feature selection.  We show how to: get summary statistics from text, search for and analyse keywords and phrases, analyse text for lexical diversity and readability,  detect collocations, apply dictionaries, and measure term and document associations using distance measures.  Our analysis covers basic text-related data processing in the R base language, but most relies on the “quanteda” (https://github.com/kbenoit/quanteda) package for the quantitative analysis of textual data.  We also cover how to pass the structured objects from quanteda into other text analytic packages for doing topic modelling, latent semantic analysis, regression models, and other forms of machine learning.


### Prerequisites

While it is designed for those who have used R in some form previously, expertise in R is not required, and even those with no previous knowledge of R are welcome.


### Part 1: Getting Started and Basic Text Analysis

*  [CRAN](https://cran.r-project.org) for downloading and installing R
*  [GitHub page for the **quanteda** package](https://github.com/kbenoit/quanteda)
*  Additional packages to install:  STM, topicmodels, glmnet
*  [Getting started, text import, and basic analysis](http://htmlpreview.github.com/?https://github.com/kbenoit/ITAUR-Short/1_getting_started/1_getting_started.html)
*  **Exercise:** Step through execution of the [.Rmd file](1_getting_started/1_getting_started.Rmd).
*  Sample data files: [SOTU_metadata.csv](https://github.com/kbenoit/ITAUR/blob/master/data/SOTU_metadata.csv), [inaugTexts.csv](https://github.com/kbenoit/ITAUR/blob/master/data/inaugTexts.csv), [tweetSample.RData](https://github.com/kbenoit/ITAUR/blob/master/data/tweetSample.RData)

*  **Exercises:**  
    1. Try running this RMarkdown file: [test_setup.Rmd](http://htmlpreview.github.com/?https://github.com/kbenoit/ITAUR-Short/0_demo_and_setup/test_setup.Rmd).  If it builds without error and looks like [this](http://htmlpreview.github.com/?https://github.com/kbenoit/ITAUR/blob/master/0_setup/test_setup.html), then you have successfully configured your system.  

### Part 2: Descriptive text analysis using R

*  [Descriptive analysis of texts](http://htmlpreview.github.com/?https://github.com/kbenoit/ITAUR-Short/2_descriptive/2_descriptive.html)
*  **Exercise:** Step through execution of the [.Rmd file](2_descriptive/2_descriptive.Rmd).

### Part 3: Advanced analysis and working with other text packages

*  [Advanced analysis and working with other packages](http://htmlpreview.github.com/?https://github.com/kbenoit/ITAUR-Short/3_advanced/advanced.html)
*  **Exercise:** Step through execution of the [.Rmd file](3_advanced/advanced.Rmd)
*  **Twitter analysis example**, and the instructions for setting up your own Twitter app, in [Twitter.Rmd](3_advanced/Twitter.Rmd). 

### Additional Resources

Designed to be done before the course or after, to augment what is presented during the course.  These are just suggestions -- no reading for the course is required.

*  [Sanchez, G. (2013) Handling and Processing Strings in R Trowchez Editions. Berkeley, 2013.](http://www.gastonsanchez.com/Handling and Processing Strings in R.pdf)  
*  [**stringi** package page](http://www.rexamine.com/resources/stringi/), which also includes a good discussion of the [ICU library](http://site.icu-project.org)  
*  Some guides to regular expressions: (Zytrax.com's User Guide)[http://www.zytrax.com/tech/web/regex.htm]
 or the comprehensive resources from http://www.regular-expressions.info  
*  See the [`quanteda` tag on Stack Overflow](http://stackoverflow.com/questions/tagged/quanteda), where you can pose questions and see some brilliant answers by our development team.
