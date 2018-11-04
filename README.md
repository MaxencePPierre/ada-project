# Title

# Abstract
A 150 word description of the project idea, goals, dataset used. What story you would like to tell and why? What's the motivation behind your project?

The dataset we have choosen is the Amazon reviews which contains product reviews and metadata from Amazon, including 142.8 million reviews spanning May 1996 - July 2014. This year’s theme is “data science for social good”, we though about how we could improve society through data analysis
What we want to do : Study and try to tell a story about the evolution of people interest concerning climate change, renewables energies, pollution and bio food. Actually, aside Ada course, our group is following another course Data Visulation is which our project is to do some data visualiaztion about different climates changes scenario over the year 2050. The data is provided by standford and what would like to do is that we found interested to compare Amazon and Standford data over two differents project but focused on the same topic.


# Research questions
A list of research questions you would like to address during the project.
- How the interest and concern in the climate change evolved over the years ?
- How Amazon proposals evolved on this theme ? Did they follow the trend on this subject
- What are people's favorite support ? (e-book, book, reports, ..)
- Who are the main and different different publishers ? Indeed information sources are very important in this domain
- Is the climate change theme linked with some others (dependent, correlated , ..) ? 
- What did people also buy ?
- Which categories to focus on ?
- How to visualize the best the relevant information ? 

# Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

The total amount of data represents 142.8 million reviews spanning from May 1996 to July 2014. It is in total around 20Gb. This dataset includes reviews (ratings, text, helpfulness votes), product metadata (descriptions, category information, price, brand, and image features), and links (also viewed/also bought graphs).

Here is the link of Amazon dataset overview : http://jmcauley.ucsd.edu/data/amazon/
As our theme is mostly climate change, we might focused on some categories such as :  Books, Kindle Store, TV-Movies, Health - Personal Care, Tools and Home Improvement, App for android, Amazon Instant Video. Indeed sport and outdoor or clothes might not be a big study part unless people interests can be linked. 

The data is split into K-core and Ratings only subsets and group by categories. 
K-cores (i.e., dense subsets): These data have been reduced to extract the k-core, such that each of the remaining users and items have k reviews each.
Ratings only: These datasets include no metadata or reviews, but only (user,item,rating,timestamp) tuples. Thus they are suitable for use with mymedialite (or similar) packages.

The data can by read with python, as a python dictionnary object, which is fine for use because we will use python. It also can be written in json file to use another langage. On the dataset overview, they provide a way to read the data into a pandas data frame.
Regarding the size of the data and the subsete, the question we have to answer is if we need the use of apache spark or not ? As the data is split in subset, it will mainly depend on the size of subsets or on what we want to do and how.
 

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

# Questions for TAa
Add here some questions you have for us, in general or project-specific.

If our theme enough big to work with ? Is it not to contraint ?
We also though about another theme : Robotic and IA. If climate change is not enought, we can compare the evolution of those two themes.
