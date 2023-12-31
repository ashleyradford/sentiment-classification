# Sentiment Classification

Joshua Bang, Ashley Radford, Emeric Szaboky, Lash Tan **(2018)**

This notebook compares two different binary sentiment classification methods. One approach uses a sparse Tf-idf matrix with a random forest classifier. Initially, text is normalized via cleaning, expanding contractions, case conversions, removing stopwords, stemming etc. The matrix is then constructed with a true-labeled column and random forest classification is applied.

The other approach relies on a parsimonious rule-based model for sentiment analysis - specifically, the VADER package. This particular model uses a constructed and validated gold-standard list of lexical features with their associated sentiment intensity measures. These features are combined with five general rules that embody grammatical and syntactical conventions, i.e. punctuation, capitalization, degree modifier, conjunction, and negation. Each text/review is scored with continuous polarity scores in range of [-1,1], where -1 represents extreme negative sentiment and 1 represents extreme positive sentiment.

## Requirements

You will need to have:
- Jupyter Notebook
- CJ Hutto's vaderSentiment repository [materials](https://github.com/cjhutto/vaderSentiment).
- `feature_extractors.py` from Dipanjan Sarkar's [chapter 4](https://github.com/dipanjanS/text-analytics-with-python/tree/master/Old_Edition_v1/notebooks/Ch04_Text_Classification).

## Data Download

Yelp business review and video game review text (from Steam) were used in this project. You may download the Yelp review dataset [here](https://www.yelp.com/dataset). The video game review data is not readily available, please refer to Reference in `nlp_text_mining.ipynb`.

## Running the Code

To run the code and analysis simply download `nlp_text_mining.ipynb` and run via Jupyter Notebook. A June presentation on this project is also provided as a `.key` file.
