# Python

In this repository I will try to group all the different analysis that I have done in different courses at Copenhagen Business School and projects that I worked on in my spare time.

<h3> Data sets </h3>

<h4> Screening Tool </h4>
Since 2015, the Danish Agency for Labour Market and Recruitment (STAR) has used a profile clarification tool on job seekers in order to help the unemployed return to the labor market. The tool assesses the citizen’s risk of long-term unemployment. I present how STAR can remove potential discriminatory features by introducing a Random Forest model where origin does not have significant importance. The recommendation to STAR is based on an analysis of a range of models, all which can be found in the data set.

<h4> Generate fake trump tweets </h4>

By using the power of transformers, in this case a GPT-2 transformer, I show how to analyze trump tweets and generate [fake] tweets. The power of transformers is astonishing and the boundaries are being pushed every year. Especially now with the lunch of GPT-3 in 2020 which have shown remarkable results.

Data: the zip file is to be found above.

<h4> Analyzing amazon reviews with neural network </h4>

Amazon product reviews have been used for business analysis in multiple ways already; specifically when applying different machine learning methods from Natural Language Processing (NLP). Some research articles focus on applying supervised machine learning for Sentiment Analysis of the reviews (Haque et al. 2018, Jagdale et al. 2019). Another study built a generative model which created new text based on the existing review text (Dong et al. 2017). Existing studies focus on an amount of reviews ranging between 20.000 to 50.000 reviews in total. With our project, we wanted to focus on a larger data set and examine the most recent data available. During our research, we found out that there existed a large database of Amazon reviews. This database consisted of different versions, depending on the year they were released. For this project, we decided to use the 2018 Amazon review data, which is the newest version of the database that was published in the article of Ni et al. (2020). The amazon review data consists of reviews and metadata about products from multiple categories scraped from the website www.amazon.com. All reviews were created between 1996 and 2018. The total amount of reviews in this data set which could be analyzed (across all product categories) is roughly 233 million. The amount of reviews per category varies enormously, with some categories below 100k reviews (Magazine Subscriptions) and others in the double-digit millions (Sports and Outdoors, Electronics).

<h4> Topic modeling </h4>
I use the same amazon reviews that I mention above to do some topic modeling. I use LDA and wordcloud.

<h3> Data sets used in CS50 </h3>

<h3> Tournament </h3>
Assuming we have a CSV file with team names and ratings, the program will simulate a thousand tournaments between the teams and calculates the chance of winning for each team. Each teams and its rating is loaded into a list (list of dictionaries). Afterwards, we simulate a tournament and each time a team wins a count is upated. Based on the overall number of tournaments the probabilities are calculated.

<h3> DNA </h3>
A python script that can identify someone from a database, based on their DNA sequence. The script must be called with two additional command line arguments; a csv database containing the number of times that particular sequences of characters repeat in a list of people’s DNA sequences, and a DNA sequence .txt file that we will be analysing and assigning an owner to based on the database in the first argument.

Feel free to propose changes!
