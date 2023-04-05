# Twitter Topic Modeling

This is a Python script for scraping tweets from a specified user's timeline, performing topic modeling on the tweets using Latent Dirichlet Allocation (LDA), and visualizing the most frequent words in the topics using word clouds. 

## Installation

To run the script, you will need to install the following libraries:

- `snscrape`
- `pandas`
- `nltk`
- `gensim`
- `wordcloud`

You can install these libraries using `pip` by running the following command:

`pip install snscrape pandas nltk gensim wordcloud`


## Usage

To run the script, you will need to provide the following inputs:

- `username`: the Twitter username of the user whose tweets you want to scrape
- `num_tweets`: the number of tweets to scrape from the user's timeline
- `num_topics`: the number of topics to generate using LDA
- `passes`: the number of times to run the LDA algorithm

You can run the script by running the `topic_model_from_user()` function with the required inputs:

`topic_model_from_user(username, num_tweets, num_topics, passes)`


The script will scrape the specified number of tweets from the user's timeline, preprocess the tweets, generate the LDA model, calculate the coherence score, and visualize the most frequent words in the topics using word clouds.

## Limitations

The main limitation of this script is that it relies on the `snscrape` library, which is not an officially supported Twitter API and may not always work as expected. Additionally, the accuracy of the topic modeling and word clouds may be affected by the quality of the scraped tweets and the parameters used for the LDA model.

## Reference

```
E. S. Negara, D. Triadi and R. Andryani, "Topic Modelling Twitter Data with Latent Dirichlet Allocation Method," 2019 International Conference on Electrical Engineering and Computer Science (ICECOS), Batam, Indonesia, 2019, pp. 386-390, doi: 10.1109/ICECOS47637.2019.8984523.
```

## License

This script is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
