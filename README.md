**Twitter AutoBot**

Twitter AutoBot is a demo project that demonstrates how to create a simple Twitter bot using the Twitter4J library in Java. This bot automatically tweets a set of predefined messages from a text file at specified intervals.

Getting Started

_To run the Twitter AutoBot, follow these steps:_

**Step 1: Create a Twitter Application**
Go to the Twitter Developer Portal and log in to your account.
Create a new Twitter application.
Take note of the Consumer Key, Consumer Secret, Access Token, and Access Token Secret provided for your application.
<br/><br/>
**Step 2: Set up the Project**
Download and install IntelliJ Community Edition (or use your preferred Java IDE).
Clone or download the TwitterAutoBot project from the repository.
Open the project in IntelliJ or your preferred IDE.
<br/><br/>
**Step 3: Configure Twitter4J**
In the project, locate the twitter4j.properties file in the src/main/resources directory.
Open the twitter4j.properties file and replace the following properties with your Twitter application credentials:
oauth.consumerKey
oauth.consumerSecret
oauth.accessToken
oauth.accessTokenSecret
<br/><br/>
**Step 4: Prepare Tweets**
In the project, create a text file named tweets.txt in the src/main/resources directory.
Add the tweets you want the bot to post, with each tweet on a separate line. Make sure each tweet is within Twitter's character limit (280 characters).
<br/><br/>
**Step 5: Run the Bot**
In your IDE, locate the TwitterAutoBot class in the src/main/java directory.
Run the main method in the TwitterAutoBot class.
The bot will start tweeting the messages from the tweets.txt file at the specified intervals.
Customization
<br/><br/>
We can customize the behavior of the Twitter AutoBot by modifying the following:
<br/><br/>
Tweet Interval: In the tweetLines method of the TwitterAutoBot class, we can adjust the Thread.sleep duration to set the time interval between tweets.<br/>
Tweet File: If we want to use a different file for tweets, update the file path in the FileInputStream constructor in the tweetLines method.<br/>
Please note that the project currently uses a limited subset of Twitter API endpoints. If we require access to additional endpoints, we may need to upgrade our developer account or request access from Twitter.
