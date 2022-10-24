


![Alt text](./Charts/headder.png?raw=true)


Project3 - Web Scraping & Classification


Problem Statement:
What characteristics of a post on Reddit are most predictive of the overall interaction on a
thread (as measured by number of comments)?


Who would be interested in this project:
Marketing and Social Media Agencies

What models will be created:
  - RandomForestClassifier
  - ExtraTreeClassifier
  - DecisionTreeClassifier
  - AdaBoostClassifier
  - LogisticRegression


What score indicates Success:
- I’m considering the median of number of comments as my baseline which is 9 comments.
- based on that baseline, my data is totally balanced, my baseline model will be predicting with about 50% accuracy:
		- Low engagement    0.503642
		- High engagement   0.496358


Metrics of Success:
  - Accuracy
  - Precision
  - Recall

Out of all models I have used I prefer to work with LogisticRegression since it’s easier for interpretation:

  - Overall accuracy: 81%  which is better than the baseline score 50% based on class majority

  - For low engagement we have a good precision 77% which is the true positive out of all positive observations, recall 87% which is the true positive of all observations.

  - F1 score:  82% which is the harmonic mean between precision and recall.


Modeling:

RandomForestClassifier:
  - X_train accuracy is: 0.9964848143982002
  - X_test accuracy is: 0.8838582677165354


ExtraTreeClassifier:
  - X_train accuracy is: 0.9967660292463442
  - X_test accuracy is: 0.8822178477690289


DecisionTreeClassifier:
  - X_train accuracy is: 0.9964848143982002
  - X_test accuracy is: 0.8894356955380578

AdaBoostClassifier:
  - X_train accuracy is: 0.9881889763779528
  - X_test accuracy is: 0.8562992125984252

LogisticRegression:
  - X_train accuracy is: 0.9420697412823397
  - X_test accuracy is: 0.800524934383202


My Recommendations:

Best Subreddits:
- r/memes
- r/dadjokes
- r/jokes
- r/theworldnews
- r/funny
- r/pics
- r/PokemonGoFriends
- r/me_irl


Best time to post:
- Between 3pm to 8pm

Best Words:
[Meme,Game,Like,Much,Still,One,Everyone,Anyone,Know,
Call,Men,Maybe,Last,Way,Get,Time,Every,Moment,Oc,Hospitality,Mirror,
Trump,Joe,Happened,Vetime,Head,Changed,Doing,Wcgw,Girl,Ichiel,lol]
