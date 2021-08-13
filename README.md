# Tweet Takedowns in India 
This repository contains data and analysis for my master's project at Columbia Journalism School on the rise of social media censorship and content removals by the Indian government, particularly after the BJP's victory in 2014. It includes notebooks with original code as well as the completed datasets. This project was completed on August 12, 2021.

## Data 

In `Removal Requests and Twitter API.ipynb`, I first compile data from Twitter's [transparency reports](https://transparency.twitter.com/en/reports/countries/in.html) about the number of tweets and accounts flagged for removal by the Indian government. I then scrape the [Lumen Database](https://lumendatabase.org/) for the original legal demands, available as downloadable PDFs. I extracted all the Twitter URLs specified in the removal orders with regular expressions, and using Twitter's API I collected data on the tweets' texts, engagement metrics, user bios and followers. Since tweets appear differently in and outside India, I included two separate columns to compare what they look like.

In `Indian Kanoon court cases scraping.ipynb` and `Extracting text from PDFs.ipynb` I scraped, extracted and cleaned data on sedition and UAPA court cases in India from 1950 to today. While I didn't use most of this data for my story, it helped provide a framework with which to understand freedom of online speech in India.

## Files 

- `tweet_removals_india.csv` is the full, cleaned dataset for all the tweets the Indian government legally demanded Twitter to take down. The URLs are obtained from Lumen, which Twitter provides voluntarily, and as such, may not be _all_ the tweets flagged for removal by India. The file also contains the tweet's text as it appears in India and the US, as well as other metrics about the user.
- `twitter_transparency_data_india.csv` contains cleaned data obtained from Twitter's transparency reports since 2012. 
- `categorized_available_tweets.csv` is a pared down version of the full dataset – only containing tweets whose text was available. One of 8 categories is then ascribed to the tweet, giving a sense of the kinds of content flagged by the government. Variations of this file were made to map this data.
- `sedition_cases_all.csv` contains all the data scraped and cleaned from [Indian Kanoon](https://indiankanoon.org/).
- `behindbars_data.csv` is a database of journalists arrested and/or detained, pulled from Free Speech Collective's [Behind Bars report](https://freespeechcollectivedotin.files.wordpress.com/2020/12/behind-bars-arrests-of-journalists-in-india-2010-20.pdf).

## Contact
If you have questions about this data or analysis, please contact Paroma Soni at paroma.soni@columbia.edu.
