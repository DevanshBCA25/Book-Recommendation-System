# Book-Recommendation-System
Welcome to the Book Recommendation System! 📚✨ This project aims to help users discover new books based on their preferences and reading history using collaborative filtering and content-based recommendation techniques.

**Types of Recommendation System :
**

1 ) Content Based :
Content-based systems, which use characteristic information and takes item attriubutes into consideration .

Twitter , Youtube .

Which music you are listening , what singer are you watching . Form embeddings for the features .

User specific actions or similar items reccomendation .

It will create a vector of it .

These systems make recommendations using a user's item and profile features. They hypothesize that if a user was interested in an item in the past, they will once again be interested in it in the future

One issue that arises is making obvious recommendations because of excessive specialization (user A is only interested in categories B, C, and D, and the system is not able to recommend items outside those categories, even though they could be interesting to them).

2 ) Collaborative Based :
Collaborative filtering systems, which are based on user-item interactions.

Clusters of users with same ratings , similar users .

Book recommendation , so use cluster mechanism .

We take only one parameter , ratings or comments .

In short, collaborative filtering systems are based on the assumption that if a user likes item A and another user likes the same item A as well as another item, item B, the first user could also be interested in the second item .

Issues are :

User-Item nXn matrix , so computationally expensive .

Only famous items will get reccomended .

New items might not get reccomended at all .

3 ) Hybrid Based :
Hybrid systems, which combine both types of information with the aim of avoiding problems that are generated when working with just one kind.

Combination of both and used now a days .

Uses : word2vec , embedding .


**Technologies Used
**

Programming Language: Python

Libraries:

Pandas

NumPy

Scikit-learn

Matplotlib (for visualizations)

Data Storage: CSV files (can be extended to databases)


**Given Data
**

The Book-Crossing dataset comprises 3 files.

Users : Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL values.

Books : Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.

Ratings : Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.


**Contributing
**

Contributions are welcome! If you have suggestions for improvements or want to add features, feel free to open an issue or submit a pull request.
