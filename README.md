


# Political Wikipedia Edit trends: Indicators for important events
## CMPS 3160 Fall 2022 Project Website
Data Science: CMPS 6160, Fall 2022

[A link to the page can be found here](https://oliverorejolacmps3160.github.io.)

### Summary
[Wikipedia](https://www.wikipedia.org) is an open source online encyclopedia, with the english wikipedia host to more than 6.5 million articles. With it being open source, many users are at liberty to make edits, updates, and changes to articles pertaining to a plethora of topics ranging from science, pop culture, politics and many more. Those who make edits may have many reasons, but ofcourse when an event happens one expects that editors flock to article relevant to particular event and make edits as to capture or reflect the news. In this project we set out to study the relationship of wikipedia edits made and important events. Here and through out, we restrict our consideration to a handful of political figures in the United States.

The goal of this project is to investigate time series trends in wikipedia page edits for key US political figures. In particular, we are interested in answer the question if wikipedia edits are indicators for importnat events. We address correlation between types of wikipedia edits made (Major, Minor, and IPs) and their relationship with important events. Moreover, we test a unsupervised model for classifying important events.

Since important event is a rather subjective notion, we measure the importance of a date with respect to a particular person, with the number of times that date appears on their wikipedia page. Although, we can rank importance with this number, through out we consider a date importance to be a binary class. That is, a date is considered important with respect to an individual, if that date appears any where on their wikipedia page.

We use a classic unsupervised learning technique, Isolation Forrests, to classify dates as important. We demonstrate that these models preform with high precision, but with low recall as our definition of importance is ill posed and over counts.

#### Techniques Used
  * Web Scraping Using [Beautiful Soup](https://pypi.org/project/beautifulsoup4/#:~:text=Beautiful%20Soup%20is%20a%20library,and%20modifying%20the%20parse%20tree.)
  * Exploratory Data Analysis
    * Edit Trends
    * Important Dates
  * Unsupervised learning for Anomoly Detection
    *  [Isolation Forrests](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.IsolationForest.html)
