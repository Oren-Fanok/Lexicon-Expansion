# Lexicon-Expansion


This Lexicon Expansion program is useful for defining relevant target data from large amounts of text using keywords. The file will build a dictionary of text based on whether or not the tweet contains the relevant keywords, as defined by the concetration functions (more information below). The final result is a lexicon built entirely out of text that is relevant to the business case.

# Process

To begin the we read in our source data we are looking to build a keyword dataset from. Once the file is read in we start experimenting with words that fit our criteria. Here we are looking for words that are a in tweets that involve vaping.

Once we have narrowed down three key words we split our dataset into two sets of tweets, tweets that contain the three keywords and tweets that do not. Next we will find words in our keyword tweet dataset that have a high concentration value and add them to our Lexicon dictionary.

For ease of use I built a function that takes care of all of the above steps. So we will repeat the process above three time using a new set of three keywords each time. Once we have 9 keywords in total we will use the functions built in the final function build section.

The get patterns function returns, total tokens, unique tokens, average token length, lexical diversity, and the top 10 tokens (most common). Our final comparison function breaks our vape tweet dataset into lists of tweets. Keyword tweets contain all tweets that contain our 9 keywords, while non keyword tweets does the opposite. It then compares both lists of tweets and returns a dictionary that compares word concentrations in each list of tweets.

