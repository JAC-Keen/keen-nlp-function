# keen-nlp-function
Keen Feedback Pipeline using Google's Natural Language Processesing API and GCPs Serverless Functions.

![flow chart](https://github.com/JAC-Keen/keen-nlp-function/blob/master/valentinefunction.png)


Tutorial: https://keen.io/blog/tutorial-keen-nlp-sentiment-analysis-made-easy/

Together we will walk through a project that focuses on building a feedback loop with Keen as our data store and query engine, and Google Cloud’s Natural Language for pre-processing. This application will ingest a feedback response, send it through a serverless function which will enrich feedback data with a score. This score will consist of a magnitude and sentiment analysis done by Google’s machine learning “Natural Language Processing” api. This can prove to be colossally useful in cases where a business is aiming to understand if customers are enjoying their experience. That experience could be the result of a cool new software application, maybe a healthcare app that enables patients to tell you about their latest office visit (the example we’ve built below). It’s possible to track a particular customer’s progress along some series of onboarding steps, or maybe you’re looking to onboard new hires and review the impact of training material...the possibilities are endless.

First we're creating a feedback form that turns a string of feedback to json to be processed by our cloud function.
Second, we're attaching a sentiment analysis and magnitude score to the the feedback.
Last that review_text event is stored in Keen which can be viewed in the "Streams" tab of your Keen dashboard.

Demo Site: https://jac-keen.github.io/keen-nlp-function/

Dashboard Site: https://dashboards.keen.io/?id=5ea1c04f1e421c0016e5bad7&projectId=5c2e3be8c9e77c0001ed971f&accessKey=62208E6C153F6B7E89D3C3982F4956443E51B3055922BF6AA1C57400C1E123A6#/
