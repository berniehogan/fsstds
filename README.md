# From Social Science to Data Science

This repository contains the complete code for the book **From Social Science to Data Science** by Bernie Hogan. 

![Cover image](img/fsstds_book_cover_small.jpg)

This book is designed to cover core data science skills from a social science perspective. It is written as an introductory textbook to Social Data Science. 

# Who is this book for
FSSTDS is meant for students, practicioners, and learners with introductory-level Python skills who want to learn how to shape, clean, and analyse data, especially data from social media. A good place to brush up these intro skills might be my own [Introducing Python](https://github.com/berniehogan/IntroducingPython) or Van Der Plas' [Whirlwind Tour of Python](https://github.com/berniehogan/IntroducingPython). 

It assumes you can run the Jupyter notebooks. You can do this either from your local machine using Jupyter Lab (downloadable from https://www.anaconda.com/products/distribution) or by clicking on the links in each notebook for "open in Google Colab" or "open in Binder", like so: 

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/berniehogan/fsstds/master?filepath=chapters%2FCh.00.Prologue.ipynb)
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/berniehogan/fsstds/blob/master/chapters/Ch.00.Prologue.ipynb)


# Navigating this repository
This repository contains several subfolders for the book:

- [chapters](chapters) contains Jupyter notebooks for all of the headers and code in the book. It should correspond precisely to the code in the book, but where it does not, it is typically that the GitHub code has been updated for clarity, security, or functionality 
- [exercises](exercises) contains Jupyter notebooks of exercises that I have given over the years which correspond to different chapters of the book. Many of these are mentioned specifically in the book, but others are there simply because I think they can help you learn and practice. You can also find multiple choice quizzes on Sage's online resource page. 
- [data](data) contains almost all of the data you will need for this book. The one exception is Stack Exchange. In the later chapters we use an export of a Stack Exchange archive. You should get this data yourself [from the Internet Archive](https://archive.org/download/stackexchange). If you are having issues creating a pickle file from this data (as per the code in Chapter 10) then you can use [this notebook](supplemental_notebooks/Ch.supp.StackExchangeDownload.ipynb) to directly download and process the Stack Exchange. I recommend walking through Chapter 10 regardless. The rest of the data is either fair use, creative commons, or provided with permission (GADM shape files).  
- [img](img) are images that I want to include in the GitHub repo, as well as copies of all the images in the book for reference (though you should be able to produce these yourself using the Jupyter notebooks). 
- [output](output) should not have much in there. But you might want to store your own output there.
- [supplemental_notebooks](supplemental_notebooks) contains notebooks that either did not make the final cut for the book or were never meant for the book itself. These include short notebooks on [how to use virtual environments](), [how to download and clean Stack Exchange data]() in one step, and [how to get GeoPandas]() set up. This is also where I keep a running list of errata and important changes.


# FSSTDS at a Glance

We begin Part 1 by [introducing what data is](chapters/Ch.01.Introduction.ipynb) (and isn't), then consider how programming can help us collect some kinds of data. While the book is generally about programming, it is important to motivate such work by considering how data represents the world, but also thus represents many of its inequalities and assumptions. 

The next few chapters focus on the main ways to store and represent distributions of data in Python: [the Series](chapters/Ch.02.WranglingI_TheSeries.ipynb) and [the DataFrame](chapters/Ch.03.WranglingII_TheDataFrame.ipynb). 

In Part 2 I discuss how to get data into a DataFrame. We start by considering how different sites, such as Reddit, Wikipedia, and Stack Exchange tend to use consistent [file formats, like `json` and `XML`](chapters/Ch.04.FileTypes.ipynb). We show how to move from XML and JSON to a DataFrame. We see how to [merge data from multiple tables](chapters/Ch.05.MergingAndSQL.ipynb), what that logic represents, and then how to get data from the web. 

When [accessing data from the World Wide Web](chapters/Ch.06.Accessing.ipynb), I first focus on how we construct URL strings to ask for data. Then I show how we may need to [authenticate our requests](chapters/Ch.07.APIsRedditTwitter.ipynb) with things such as keys or bearer tokens depending on the circumstance. In these chapters we reflect on how data minimisation can be applied as one of several ethical principles to consider in our work.  

In Part 3 we explore how to ask questions about this data. The first of these chapters is non-technical and discusses more the importance of [considering research questions](chapters/Ch.08.ResearchQuestions.ipynb) as inductive or deductive, predictive or explanatory. I discuss how we can shift our thinking from being descriptive to being scientific by emphasising prior expectations. In the second chapter on this part, we revisit this, but with code. In the chapter ["Visualising Expectations"](chapters/Ch.09.VisualizingExpectations.ipynb), we look at how statistics as well as visualisations can help us see an expectation, pattern, trend, or outlier. This careful dance between what we expect and what we observe gets ever more complicated alongside our models. 

Part 4 of the book looks at some analysis approaches in practice. We start by [cleaning Stack Exchange data](Ch.10.Cleaning.ipynb). In this chapter the cleaning is done with a focus on the social structural features of the data. That is, we might be interested in trends or patterns by time, by geography, by identity, etc. These give us both a motivation for looking at the data but also a way to focus our cleaning efforts.  Then we have four "silo" chapters. Each one introduces some of the basic ingredients of different more sophisticated analytical techniques, each of which relate to a different aspect of the structuring of social life: [language](chapters/Ch.11.NLP.ipynb), [time](chapters/Ch.12.TimeSeries.ipynb), [relationships](chapters/Ch.13.NetworkAnalysis.ipynb), and [space](chapters/Ch.14.Geography.ipynb). 

Finally I [conclude](chapters/Ch.15.Conclusion.ipynb) by reflecting on some key conceptual and practical issues with data science as well as some directions for future learning, including tools and resources. 

# Additional resources

Many of the chapters have video walkthroughs available through YouTube. I'm keeping the links unlisted from search engines until they are all done. But you can check out the progress and enjoy draft versions of these videos through this link: https://www.youtube.com/playlist?list=PLXklL7hbg5bMEmBTE6kcAOSeT8CuRVkYH 


# Buying the book

This is meant to be a book and introductory course. While all the code is here, I feel like it makes the best sense (and looks the best) presented in book format. 

The book is available for purchase at many bookstores now. If you know me personally, feel free to get in contact as I have a few discount codes to give out.

To buy from Sage direct (or inquire about an inspection copy): https://us.sagepub.com/en-us/nam/from-social-science-to-data-science/book270152 

To buy from Amazon: https://amzn.to/3GEj6HT 