Project 3 NLP classification of subreddits posts

Business Problem
If you are new to reddit and have never used it before, you might be initimated by the number of subreddits that are present in this online community.

Furthermore, if you have a question as a system administrator or a network administrator, which subreddit do you pose your question in? https://www.reddit.com/r/sysadmin/ or https://www.reddit.com/r/networking/? With IT teams using these two role names interchangeably and with organizations increasingly expecting their staff to wear multiple hats, there is not a clear demarcation to what constitutes a network or system issue. The issue might even be multi-faceted that requires domain knowledge of both areas of expertise.

This projects aims to create an NLP machine learning model to be able to review posts and show which subreddit it would belong to and thus increase your probability of getting a helpful response to your issue.

Table of Contents
Data Cleaning
Merging the two subreddits
Exploratory Data Analysis
Train/Test Split
Stopwords
Preprocessing
CountVectorizer
Naive Bayes
Testing other models
Conclusion and Recommendations

*webscaping function is stored in separate jupyter notebook

Challenges: The struggle is real with acronyms with these two IT centric subreddits, it may look like they are stop words - worthy but on further research found to represent specialised technologies that are understood within that subreddit community.

Findings: The models that used TfidVectorizer returned features that were more meaningful words and we could see how they would be important in classifying which subreddits they would more likely belong to. Even if the Naive Bayes WordVectorizer model scored the best on unseen data, the most important features were not really actionable or insightful. Out of the three models, the feature importance extracted from Logistic Regression proved most useful in answering our business problem.

Recommendations: While we did build a good prediction model that can take processed posts from reddit and classify them according to the most appropriate subreddit, we would attach a few qualifiers to the use of this NLP machine learning model. It is a short term project that webscaped as many posts as reddit would allow and so for popular subreddits that have an active community, we were only scaping the 'flavour' of the month. For more definitive recommendations and revealing the truly important features to improve our model, it would be ideal to be able to run our model for an extended period of time just to account for seasonal topics, changing IT topics, etc for the model to stay relevant.

Areas for further research: To better answer which subreddit we would recommend if we had a brief summary of the issue or topic a user was raising, we would look to consider training our model on top rated/glided/upvoted/linked posts that the community has identified as quality contributions. That way we can ensure that our recommendations of which subreddit to post in would be in line with the reddit community's recommendations as well.
