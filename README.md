# How is evolving the interest about ecology through Amazon ?

# Abstract

The dataset we have choosen is the Amazon reviews which contains product reviews and metadata from Amazon, including 142.8 million reviews spanning May 1996 - July 2014. This year’s theme is “data science for social good”, we though about how we could improve society through data analysis.

What we want to do : Study and try to tell a story about the evolution of people interest concerning climate change, renewables energies, pollution and bio food. Indeed there are many categories of products to work on : [Books, Kindle Store, TV-Movies, Home and Kitchen, Health - Personal Care, Tools and Home Improvement, Grocery and Gourmet Food]. We will then do some visualization to show the evolution about the concerned products with the Number of Reviews, the Sale Ranking of the product and the number of products linked with our subject.

We would like then to use our Machine Learning knowledge to use the extracted data in order to train some models which could give some predictions about the coming years. This could give some ideas and trends about the products linked to the subject, by showing maybe a growing (or not) market, and an evolution of the interest by the users.

Actually, aside Ada course, our group is following another course Data Visualization in which our project is to do some data visualization about different climates changes scenario over the year 2050. The data is provided by Stanford University and what we would like to do is to compare Amazon and Standford data over two differents project but focused on the same topic.


# Research questions
- How the interest and concern in the climate change evolved over the years ?
- How Amazon proposals evolved on this theme ? Did they follow the trend on this subject
- What are people's favorite support ? (e-book, book, reports, ..)
- Who are the main and different different publishers ? Indeed information sources are very important in this domain
- Is the climate change theme linked with some others (dependent, correlated , ..) ?
- What did people also buy ?
- What are the most growing sectors focusing on Ecology ?
- Which categories to focus on ?
- How to best visualize  the relevant information ?
- How is evolving the price of these products ? (The bio was for example known to be expensive).
- How could evolve the Sale Ranking of this kind of products ? (Prediction)
- How could evolve the Nb of reviews (users interest) ? (Prediction)
- How could evolve the Nb of products concerned ? (Prediction)

# Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

The total amount of data represents 142.8 million reviews spanning from May 1996 to July 2014. It is in total around 20Gb. This dataset includes reviews (ratings, text, helpfulness votes), product metadata (descriptions, category information, price, brand, and image features), and links (also viewed/also bought graphs).

Here is the link of Amazon dataset overview : http://jmcauley.ucsd.edu/data/amazon/

As our theme is mostly climate change, we might focus on some categories such as :  Books, Kindle Store, TV-Movies, Health - Personal Care, Tools and Home Improvement, App for android, Amazon Instant Video. Indeed some ohters such as sport and outdoor or clothes might not be a big study part unless people interests can be linked. it will then depend on the results.

The data is split into K-core and Ratings only subsets and group by categories.
K-cores (i.e., dense subsets): These data have been reduced to extract the k-core, such that each of the remaining users and items have k reviews each.
Ratings only: These datasets include no metadata or reviews, but only (user,item,rating,timestamp) tuples. Thus they are suitable for use with mymedialite (or similar) packages.

We will also use the metadata dataset which is complementary to the reviews and will give information about the product itself : Sale ranking, price etc...

The data can by read with python, as a python dictionnary object, which is fine for us because we will use python. It also can be written in json file to use another langage. On the dataset overview, they provide a way to read the data into a pandas data frame.
Regarding the size of the data and the subsete, the question we have to answer is if we need the use of apache spark or not ? As the data is split in subset, it will mainly depend on the size of subsets or on what we want to do and how. Also amazon splits the data into file which can be subset as wee saw above, soem file with or without duplicates reviews, with or without the ratings. We might focus on categories subsets which interest us.

For our side, the dataset is stored on the EPFL cluster.

# A list of internal milestones up until project milestone 2

Milestone 2 : 25th November

First of all we will properly define the relevant categories by observing the data and the numbers.
Then we will work on the data extraction of the chosen categories and for each category we will select the products respecting the criterias of our subject (Bio, Ecology, Renewable etc..).
For this we will have to set a list of key words to focus on, in order to filter the data.
There will be of course a big part of data cleaning in order to gather all the relevant informations.
Additionally, as the dataset is on the cluster, we will do some observation extraction of data in order to understand and use the frameworks through the cluster.

We will then work following these milestones :

11th November :
Analysis of the Amazon dataset. Understanding of the cluster process.
Data analysis - extraction : Choice of categories
List of key words to do the fliter search of products.

18th November :
Analysis of the 2 datasets : Amazon Reviews and Metadata, in order to merge/combine these 2. We will then have the information about the products (categories, sales etc..) and the associated reviews.
Data extraction, data wrangling on the interesting parts.
This will then allow us to work for the next milestone and get all the concerned data.

25th November :
Create a final notebook with the explanations about the data collection and cleaning.
Merged dataset with Dataset Reviews and Metadata.
Different cases of data following the categories of products. Each will have a data cleaning.

Then the dataset will be well processed and ready for the Milestone 3.
Indeed, once the data is well gathered and cleaned, we will then be able to work on it using Machine Learning models to do some prediction and to do visualization on it. With the splitted data we will then compare the different categories.

# Questions for TAa
Add here some questions you have for us, in general or project-specific.

If our theme enough big to work with ? Is it not to contraint ?
We also though about another theme : Robotic and IA. If climate change is not enought, we can compare the evolution of those two themes.
The data is stored on the cluster, but is it possible to extract the relevant information concerning our subject and then work on it or to work entirely on the cluster ?
Do you think we should use spark ? During the project presentation the professor explained that the Amazon dataset was on the limit for the usability of spark (20Gb).
The dataset website explain that there is a 20Gb dataset and an other 18Gb removing the duplicates. Which one is in the cluster and can we use the cleaned one ?
What could be the direction to extract the data in the cluster ?
Is the Metadata dataset also available on the cluster ? (about prices, sale ranking of products)
