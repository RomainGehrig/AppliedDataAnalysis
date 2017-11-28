# Twitter Vote

# Abstract
Voting participation is declining and is particularly low for young people, but people express their opinions more and more on social medias.
Does opinions expressed on Twitter reflect the opinion of all the population?

We want to understand how the opinion of the Swiss population evolve before and after a Federal votation using the tweets referring it.
Knowing the results, we can put in perspective the tweets and compare the opinion of people region by region.

# Research questions
  * Are the sentiments towards a votation different from the results?
  * Do they change after knowing the results?
  * Would it be possible to predict the results?
  * How the sentiment evolve through time? Is there turning points? And what caused them?

# Dataset
The Swiss tweets dataset will be our primary source, with it's sentiment score used to evaluate the feeling of Swiss people about a votation.
We will also use the votation results to draw a parallel with Twitter.

## Exploration
We downloaded the Spinn3r dataset to be able to work on our own computers, but the resulting 36GB of data are too big to fit in memory.
Since we wanted to work on tweets containing tags, we started by filtering out untagged tweets and thus reduced our dataset to 7GB.

To find out which votations have been discussed on Twitter, we looked at the hashtags often tweeted in pair with #chvote. And we found the following votations to have been discussed the most:
  1. #abst16 (Reduce dependency on atomic energy)
  2. #avsplus (Change the AVS)
  3. #lrens (Give more power to Swiss intelligenc agency)
  4. #rbi (Provide an universal income)

The hashtag #abst16 is the more frequent tag, so we will use this votation to do our analysis. People don't always refer to that votation with the same hashtag, so we will need to find the other tag linked to it (for instance #sortiedunucleaire).

We wanted to base our analysis on the `sentiment` computed by Spinn3r, but unfortunately tweets have been mostly categorized as `NEUTRAL`. We will need to build our own classifier (reusing for instance our work on the last homework) to extract more meaningful infomations.

# A list of internal milestones up until project milestone 2
We will explore the Swiss Twitter dataset to understand which votations have been discussed on the platform and select a set of them.
We can then select a votation and start extracting informations from the tweets.
We will produce a map of Switzerland where we can display the results of the votations and our analysis with different resolutions (by region, city, etc.)

# Milestone 3
For the next part we will compute our own sentiment score. We still hesitate in reusing our work in the previous homework to build the classifier or to rely on an existing on like IBM Watson. Depending on the results, we should be able produce interesting predictions and analysis, like finding a correlation between Twitter's opinion and the votation result.

We also need to produce visualisation on those data, for instance plotting the tweets on a map (that may reveal some bias in the data) and plotting the sentiment of regions.

# Questions for TAs
Not for now, but we won't hesitate to ask on Mattermost if needed!
