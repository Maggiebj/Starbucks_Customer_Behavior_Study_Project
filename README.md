# Starbucks_Customer_Behavior_Study_Project

This project is a study of Starbucks customer behavior. we are about to answer the questions of which demographic users group response best to which type of offers. With the force of data science, we have develop some tools like classification prediction model and recommendation system to increase the users purchase. We approach the solutions by the following ways:

1 Found the demographic users difference in 4 groups and understood how demographic features associated with customer behaviors:

  Group1: Users completed the offer without viewed.

  Group2: Users viewed the offer and completed it.

  Group3: Users viewed the offer but not completed it.

  Group4: Users did not view nor complete the offers.

2 Built a classification model to predict whether a user who receive the offer(discount/bogo offers) would complete it.

3 Built a user-user based collaborative filtering recommendation system to recommend bogo/discount offers to new and old users.

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)


# Installation<a name="installation"></a>
The jupyter notebook file should be run with python 3.X . 

# Project Motivation<a name="motivation"></a>
Firstly we split users in 4 groups based on customer behavior on offers they received. And we have some analyze on how the users demographic associated with each the response behavior groups. We have observed that information offers do not have complete events. We have learned there are some differences between bogo/discount offers and information offers in response behavior and user demographic.

In the task 2 , we built a classification model to predict user who receive bogo/discount offers would complete it. That would help us to send offers to users more targetable and save money.

In the final task, User-user based collaborative recommendation can play well in this scenario. We recommend user with the offers which have cumulated maximun rewards from his similar user. And we remove the offer the user did not inflenced by. That's another way to increase purchase. The recommendation system works well for old user and new users. 

# File Descriptions<a name="files"></a>
There are 1 python files implement the product.

Starbucks_Capstone_notebook.ipyn--The implementation code for the 3 tasks


# Results<a name="results"></a>
We have successfully achieved the project goal by completed the 3 tasks. 
In task 1, we figured out demographic difference between the 4 user groups based on user’s behavior on offers. We concluded we have found in exploratory analysis:

	Elder users (age about 56-57) have more willing to buy.

	Users have higher income (income about 70000) are less impacted by offers and also more willing to pay.

	Users who have long period of membership (about 750days), they are more loyal and have more willing to pay.

We created a typical user profile who would view and completed offers: a female, about 58, she has income of 72000 and she has been a member for 754days. Or a male, he is 54, he has income of 64000, and he has been a member for 771 days.

We saw users who completed bogo and discount offers had longer membership period (above 750days) than users who did not completed offers (about 500days). Ages of users who completed bogo and discount offers (above 56) are higher than users did not (about 52). Users who completed bogo and discount offers have higher income (above 67000) than who did not (about 55000). 

For users who received information offers, we saw users who had transactions with or without viewed had longer membership days(above 760 days) and less income (income median 59000) than users who did not had transactions with or without viewed (membership about 450 days and income above 65000).

In task 2, we built a classification model with RandomForestClassifier to predict users would view and complete offer he receives. For bogo and discount offers, we have accuracy of 68.99% of predict correctly on whether a user would complete the offer. For a predict user who would complete the offer, we have 67.37% confident he would truly complete the offer. And for users who would actually complete the offers, there are 69.73% of the users he would be identified by the model.

In task 3, we built a user-user based collaborative filtering recommendation system. We recommend user offers which his similar users have got cumulated maximum rewards from these offers and we remove offers the user did not influenced by according to history(from offer_receive_view_complete dataset).


# Licensing, Authors, Acknowledgements<a name="licensing"></a>
Must give credit to Starbucks for the data.And [Udacity](http://www.udacity.com) for project design and instructions.
