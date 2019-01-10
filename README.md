# write-a-blog-post
Udacity project - using a real-world dataset, clean the data and investigate three business-domain questions 


### Table of Contents

1. [Libraries and Installation](#installation)
2. [Project Description](#motivation)
3. [Files](#files)
4. [Findings](#results)

## Libraries and Installation <a name="installation"></a>

Libraries used:
### Folium

The Folium library is used to plot maps and locations.

MIT Licensed by Rob Story

To install:
$ conda install -c conda-forge folium

### TextBlob

The TextBlob library was used to perform sentiment analysis of English free text.  Built on top of the NLTK.

MIT Licensed by Steven Loria

See: https://textblob.readthedocs.io/en/dev/

To install:
$ pip install -U textblob
$ python -m textblob.download_corpora


### LangDetect

The LangDetect library is used to detect languages used to write the user reviews.

It is licensed under the Apache License License: Apache Software License (Copyright 2014-2015 Michal "Mimino" Danilak) by Michal Mimino Danilak.

See: https://pypi.org/project/langdetect/

To install:
$ pip install langdetect

## Project Description<a name="motivation"></a>

This project uses the AirBNB Boston dataset to explore the effects of large entertainment events on AirBNB Business.

Specifically, I am looking for a quantifiable trend in terms of:

1. Number of customers
2. Price charged by operator
3. Customer experience

These values are investigated relative to distance to the event and a seasonally-adjusted baseline.


## Files <a name="files"></a>

The analysis and summary explanation can be foind in the Jupyter Notebook "write-a-blog-post.ipynb".  Exploratory code is contained in the other two notebooks, which are not critical to the project. 

The relevant datasets are "calendar4.csv", "listings2.csv", and "reviews2.csv", and were obtained from the archival dataset at http://insideairbnb.com/get-the-data.html.

The data files indicated above capture the data relevant to the 2018 timeframe.

## Findings<a name="results"></a>

Briefly, the analysis shows:

1. A distinct up-trend in business is expected for AirBNB operators around the time of a major entertainment or sporitng event.
The threshold for significant business increase occurres around the 40000-atendee mark. For the Boston market at least, this trend is
consistent across the local AirBNB market; there is no evidence to support a localized phenomenon near the event venue.  As a result, 
creating a linear model to predict localized increases in business is not relevant.

2. AirBNB operators near the event venue are observed to be offering their services at an increased price.  This trend does not 
continue into more remote AirBNB service operations.

3. The satisfaction of AirBNB customers is inferred to be less when staying with an operator close (within approximately 5 km) to the venue.  This inference is made using NLP of review sentiment.

A summary of the findings is published here:
<#TBD>.





