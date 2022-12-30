                                                                           Person-rank
A large part of what Google uses to rank websites is something called PageRank. 
Effectively each page gets a value based upon how many other pages link to it. 
The value that those pages have influences the value of the page that is linked to as well.
A link from a highly ranked page could be worth more than several links from lower ranked pages for example.
Let's do similar for Tweets and create a PersonRank. Say we have a file and in it are a series of Tweets.
Each line begins with the handle of the person making the tweet, followed by a tab, then the actual tweet, 
followed by a tab again, and finally the number of likes that tweet got.
Every time a person is mentioned in a tweet, we can consider a vote for that person. 
See if you can write a program to read in the tweets from the file and then calculate each person’s PersonRank. 
Print out the results in order of the PersonRank.

Criteria to use: You may use the number of mentions, and the number of likes. Weightage can be such that each like on tweet mentioning the user has a score of 5 and each mention has a score of 50. Each like on the tweet by the user has a score of 10.

Explaination of Problem :-
    ~basically we need to extract the users name and then score them according to criteria.
    ~According to Criteria their are three ways to score the users.
      - we need to score 10 to the user for each like on the tweet.
      - we need to give score 50 to each mentioned user.
      - we need to give score 5 to each mentioned user for each like.


