# Social Network Analysis: Twitter dataset

Analyze the dataset twitter.tsv contains over 450.000.000
tweets, crawled from June 2009 to December 2009. The file twitter-small.tsv contains a small
subset of these tweets that can be handled with Gephi, whereas twitter-large.tsv contains a bit
larger subset that can be analyzed using for example NetworkX. Each line of these files contains
one tweet, consisting of three tab-separated (`\t') fields denoting the timestamp, user who sent the
tweet and the content of the tweet. For example:

2009-07-05 14:07:18 aeneas Hi @achilles, how are you? #old

In the tweet content, a word starting with the @ symbol (such as @achilles) means that user
achilles is being mentioned by user aeneas, indicating that the tweet by aeneas was directed at
or specically about achilles. We refer to this as a mention. Mentions are the most direct sign of
public communication on Twitter. Tweets can also be directed at more than one user.

The mention graph is a Twitter network represented by a directed graph G = (V;E). In this
graph, the set of nodes V consists of users (anyone sending out a tweet or being mentioned by
someone else in a tweet). The set of links E consists of all user pairs (x; y) such that user x mentioned
user y at least once. Optionally, this network can be a weighted directed graph where the number of
times a user x mentions another user y is used for link weight. Also, the network could be analyzed
over time by assigning a timestamp to each link, indicating when x first mentioned y.
