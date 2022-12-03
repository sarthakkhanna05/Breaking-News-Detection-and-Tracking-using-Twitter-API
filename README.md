# Breaking-News-Detection-and-Tracking-using-Twitter-API

## Abstract:
The current generation of adults prefer to consume their news in the form of small articles with the ability to track updates on that news. A large majority of these people just want to be notified about breaking news. With growing demand of such a majority, there arises a need for a fast and reliable news system with updates tracking. The existing popular news sources like Facebook and YouTube have tried combating the problem of delivering news in this format but have faced multiple challenges like real-time detection, fact checking, latency etc. To solve this problem, we propose a method to collect, predict and track breaking news using the Twitter API. We created an end to end application for the user to get their fact checked news, breaking news and related articles in one place without directly interacting with social media. The breaking news will be sent to the user as notification after regular intervals. We achieved this by combining multiple labeled data sources to detect breaking news. Pre-trained Transformer models are used for feature extraction and classification. Additionally, we created clusters of highly occurring words to identify breaking events. Furthermore, the news will be categorized into 5 categories. We also propose a similarity metric in order to compute similarity between news which will avoid repetition of news. Finally, we also rank the news to display the top trending breaking news.

# How to run the code ?

## web_app:
1. Please run npm install in both directories(Backend and Frontend) to install the dependencies.
2. Please use npm start in both directories to run the the backend and frontend code respectively
3. This will start the backend and frontend.
4. Go to localhost:3000 on your web browser. 

## ML_backend

Note: We have provided the API keys for the tweitter API. However, these will expire in a few days and you will have to create an account on twitter developer. Request for the academic development endpoint.

1. pip install -r requirements.txt
2. Download Jupyter Notebook if you want to do some visualizations
3. Run get_tweets_and_prediction.py or get_tweets_and_prediction.ipynb (if using Jupyter Notebook). 
* This will hit the twitter API every 30 mins.(You can change this in Part 7 of the code)
* It will fetch tweets from Twitter, make predictions on them, select the most informative tweet and compare similarity with previous 6 hours data for any similar news.
* After every 30 mins, the Node backend will receive tweets and corresponding information that will be processed, will be saved to the database. The data will then be used for API endpoints from where frontend can utilize different features.
4. The above command will also save upto 24 hours data which can be visualized in Graphs.py or Graphs.ipynb

## Android APP

NOTE: You need to npm install and npm start the backend in the web_app for this to work

1. Download Android studio
2. Install npm: npm install android
3. npm start (to start the application)
4. npm run android


