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

    ~Basically we need to extract the users name and then score them according to criteria.
    ~According to Criteria their are three ways to score the users.
      - We need to score 10 to the user for each like on the tweet.
      - We need to give score 50 to each mentioned user.
      - We need to give score 5 to each mentioned user for each like.


Algorithm for Problem :-


  -First we need to read the tweet from file so create a read function.Then this read function return tweets in vector of string.
 
  -Now, we need to score user from vector of tweets.
  
  -We are using map for scoring all users, In which User name as key and score as value.
  
  -First, I extract all the user name and set the score of each user as 0 / zero.
  
  -Then extract username of the user who tweet , like and tweet separately in another vector.
  
  -Then performing calculation to get score of the user.
  
  -Print the map.
  
Our code:-


![code](https://user-images.githubusercontent.com/109334405/210048577-8d2c50d3-8b5d-4c81-851f-ef12124c7a05.jpeg)


Input:-

![input](https://user-images.githubusercontent.com/109334405/210048705-86061637-4598-4677-a1fc-5175994a91d1.jpeg)


Output :-

![output](https://user-images.githubusercontent.com/109334405/210048739-5c64ea9d-3b6f-4715-ae09-bf2b445caa8f.jpeg)

