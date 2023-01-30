# Ted-talks
Text analytics of the TED talks by Stefan Sagmeister and Steven Pinker(sentiment analysis)
Description of the report
The goal of the report was to present and compare word frequencies and sentiment analyses for the transcripts of TWO TED speakers that were randomly assigned. You can take them randomly. Mine were Stefan Sagmeister and Steven It’s highly recommended that you go to the TED website, search and watch their talks to get an overview of what topics, ideas and contexts you will analyse and compare.

Relevant tips
think about what types of things can you determine from the text data. Think about what you would explore in terms of similarities/dissimilarities between the speakers’ words and sentiments. 






How to load the data sets of your allocated TED talks
You should load the dsEssex and tidyverse packages into your report. Then load the ted_talks data using the following code.
# load the required packages
library(dsEssex)
library(tidyverse)

# load the 'ted_talks' data
data(ted_talks)
Find out who are the two speakers your going to work with.
Use filter() with your own speaker names (that you got from the step 2 above) to filter data of the talks given by these speakers (Note: a speaker might has given more than one talk, and you should consider all the talks given by your speakers in the data). For example, to filter data of the talks given by Ken Robinson and Hans Rosling (Note that these names should be replaced with the actual two names which were assigned to you):


# Filter the two talk data for your analyses
## the IDs 3 and 6 here are for illustration only and MUST be replaced with your own IDs
MyData <- ted_talks %>%
  filter(speaker %in% c("Ken Robinson", "Hans Rosling"))
start using the filtered data for your project.