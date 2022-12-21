# From Social Science to Data Science

This repository contains the complete code for the book **From Social Science to Data Science** by Bernie Hogan. 

<img>

This book is designed to cover core data science skills from a social science perspective. It is written as an introductory textbook to Social Data Science. 

# Prerequisites
It is meant for students, practicioners, and learners with introductory-level Python skills, like one would cover in Van Der Plas' [Whirlwind Tour of Python]() or my own [Introducing Python](). 

It assumes you can run the Jupyter notebooks. You can do this either from your local machine using Jupyter Lab (downloadable from www.anaconda.com/individual) or by clicking on the links in each notebook for "open in Google Colab" or "open in Binder". 

# Organising the repo
This repository contains several subfolders for the book:
- [chapters](https://github.com/berniehogan/fsstds/tree/main/chapters) contains Jupyter notebooks for all of the headers and code in the book. It should correspond precisely to the code in the book, but where it does not, it is typically that the GitHub code has been updated for clarity, security, or functionality 
- [exercises]() contains Jupyter notebooks of exercises that I have given over the years which correspond to different chapters of the book. Many of these are mentioned specifically in the book, but others are there simply because I think they can help you learn and practice. You can also find multiple choice quizzes on Sage's online resource page. 
- [data](/tree/main/data) contains almost all of the data you will need for this book. The one exception is Stack Exchange. In the later chapters we use an export of a Stack Exchange archive. You should get this data yourself [from the Internet Archive](). If you are having issues creating a pickle file from this data (as per the code in Chapter 10) then you can use [this notebook]() to directly download and process the Stack Exchange. I recommend walking through Chapter 10 regardless. The rest of the data is either fair use, creative commons, or provided with permission (GADM shape files).  
- [img]() are images that I want to include in the GitHub repo, as well as reference copies of all the images in the book for reference (though you should be able to produce these yourself using the Jupyter notebooks). 
- [output]() should not have much in there. But you might want to store your own output there.
- [supplemental_notebooks]() contains notebooks that either did not make the final cut for the book or were never meant for the book itself. These include short notebooks on [how to use virtual environments](), [how to download and clean Stack Exchange data]() in one step, and [how to get GeoPandas]() set up. This is also where I keep a running list of errata and important changes.


# Summary
We begin Part 1 by [introducing what data is]() (and isn't), then consider how programming can help us collect some kinds of data. While the book is generally about programming, it is important to motivate such work by considering how data represents the world, but also thus represents many of its inequalities and assumptions. 

The next few chapters focus on the main ways to store and represent distributions of data in Python: [the Series] and [the DataFrame]. 

In Part 2 I discuss how to get data into a DataFrame. We start by considering how different sites, such as Reddit, Wikipedia, and Stack Exchange tend to use consistent [file formats, like `json` and `XML`](). We show how to move from XML and JSON to a DataFrame. We see how to [merge data from multiple tables](), what that logic represents, and then how to get data from the web. 

When [accessing data from the World Wide Web], I first focus on how we construct URL strings to ask for data. Then I show how we may need to [authenticate our requests]() with things such as keys or bearer tokens depending on the circumstance. In these chapters we reflect on how data minimisation can be applied as one of several ethical principles to consider in our work.  

In Part 3 we explore how to ask questions about this data. The first of these chapters is non-technical and discusses more the importance of considering questions as inductive or deductive, predictive or explanatory. I discuss how we can shift our thinking from being descriptive to being scientific by emphasising prior expectations. In the second chapter on this part, we revisit this, but with code. We look at how statistics as well as visualisations can help us see an expectation, pattern, trend, or outlier. This careful dance between what we expect and what we observe gets ever more complicated alongside our models. 

Part 4 of the book looks at some analysis approaches in practice. We start by cleaning Stack Exchange data. In this chapter the cleaning is done with a focus on the social structural features of the data. That is, we might be interested in trends or patterns by time, by geography, by identity, etc. These give us both a motivation for looking at the data but also a way to focus our cleaning efforts.  