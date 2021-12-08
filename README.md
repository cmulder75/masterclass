# MA5851 Master Class
## Building a web crawler
Prototype NLP tasks by Coenraad F. Mulder

MA5851 Master Class building a web scraper and applying NLP tasks to it.

## Introduction
At the best of times, humanity is struggling to cope with the impact of social media on our world and environment. When a global pandemic such as the current Coronavirus (SARS-CoV-2, or COVID-19) is mixed into the equation, social media fuels the surge of numerous rumours, hoaxes and misinformation, thus amplifying the impact and severity of it exponentially (Tasnim et al., 2020).  The latest Coronavirus variant, Omicron (B.1.1.529), was discovered by a team of infectious disease specialists at the University of KwaZulu-Natal in Durban, South Africa, and first reported to the World Health Organization (WHO) on 24 November 2021. The release of the news statement by WHO on 26 November 2021 has caused a major knee-jerk reaction throughout the world (World Health Organization, 2021). Multiple countries have imposed immediate travel bans on international travellers from possible exposure sites, even though the actual severity or impact of Omicron has not been fully realised.

This assignment sets out to clarify how the hype around a new strain or variant of Coronavirus is fuelled by social media, more specifically, to identify some of the key issues social media commentators are Tweeting around the Omicron variant, and to determine the sentiment behind those Tweets (whether it is positive or negative). This is not a fact verification service; no attempt has been made to verify the validity or content of any of the Tweets. Rather, this Twitter web crawler scrapes Tweets for the specified time period and extracts the Tweeted text in its raw format. The Tweeted text is cleaned by removing hyperlinks and punctuation marks, removing stop words and lemmatisation of the text to create a cleaned corpus. This corpus is then fed into the first Natural Language Processing (NLP) task, using latent dirichlet alloction (LDA) to identify key topics from the corpus that social commentators are Tweeting about. The second NLP task, Sentiment Analysis, takes each of the corpus entries to determine the sentiment of the Tweet, whether positive, neutral or negative. These prototype NLP tasks can be used by any development team as basis to identify key topics in a corpus, and to measure the sentiment of entries within the corpus.

## Files included in this prototype
1. Task 1 - Overview.ipynb - a Python-based Jupyter Notebook containing markdown as introcuction and overview of the Web Crawler and NLP Tasks.
2. Task 2 - Webcrawler.ipynb - a Python based Jupyter Notebook containing the implementation of the Web Crawler
3. Task 3 - Prototype NLP Tasks.ipynb - a Python based Jupyter Notebook containing the implementation of the two NLP task prototypes, Latent Dirichlet Allocation (LDA) and Sentiment Analysis using VADER.
4. tweets.xlsx - the harvested tweets used for Task 3.

PLEASE NOTE: The __rendered__ directory contains the rendered versions of these files in PDF format.

## Usage 
These files can be used to augment Natural Language Processing tasks. It provides a basis for extracting Tweets from Twitter, using a predefined keyword.

To get started, open the __Task 1 - Overview.ipynb__ Notebook, and amend the Hyper-parameters for the Scraper section. Then execute each section in turn from top to bottom.

    #######################################################################
    # Hyper-parameters for the Scraper
    #######################################################################
    date_to = '2021-12-05'
    number_of_days = 14
    tweet_limit = 1000
    search_term = 'omicron'

## Programming reference
* Jupyter Notebooks
* Python 3.8.8 running through Anaconda 3.0

