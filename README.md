# AI-BASED-RECOMMENDATION-SYSTEM

**COMPANY**: COTECH IT SOLUTIONS

**NAME**: Mahagaonkar Chaitanya Chandrakant

**INTERN ID** : CTIS3602

**DOMAIN**: JAVA PROGRAMMING

**BATCH DURATION** 4 WEEK

**MENTOR NAME**: NEELA SANTOSH

# ENTER DESCRIPTION OF TASK PERFORMED NOT LESS THAN 500 WORDS


As part of Internship Task-4, I developed an AI-Based Recommendation System using Java. The objective of this task was to design and implement a working recommendation engine capable of suggesting products or content to users based on their preferences. The system uses collaborative filtering techniques and cosine similarity to analyze user behavior and generate personalized recommendations.

The recommendation system was built using core Java concepts such as collections (HashMap, List, Set), object-oriented programming principles, and stream processing. Although advanced libraries like Apache Mahout can be used for large-scale machine learning applications, this implementation focuses on building the logic from scratch to understand the fundamental working principles of recommendation systems.

### 1. Objective of the System

The main objective of the system is to recommend items to a target user based on similarities between users’ preferences. The system analyzes historical rating data and predicts which items the user is most likely to prefer but has not yet rated.

The recommendation engine follows a **User-Based Collaborative Filtering** approach. This means:

* It compares users with similar tastes.
* It finds users who have rated similar items similarly.
* It recommends items liked by similar users that the target user has not yet interacted with.

### 2. Sample Data Creation

To simulate a real-world scenario, I created sample user data inside the program using HashMaps. Each user is associated with a map of items and ratings.

For example:

* User1 rated Item1, Item2, and Item3.
* User2 rated Item1, Item2, Item3, and Item4.
* User3 rated Item1, Item4, and Item5.
* User4 rated Item2, Item3, Item4, and Item5.

This data structure allows easy retrieval and comparison of user ratings.

### 3. Cosine Similarity Implementation

To measure similarity between two users, I implemented the Cosine Similarity algorithm. Cosine similarity calculates the cosine of the angle between two vectors (in this case, rating vectors). The value ranges from 0 to 1:

* 1 means users are highly similar.
* 0 means no similarity.

Steps followed in cosine similarity calculation:

1. Identify common items rated by both users.
2. Compute the dot product of their ratings.
3. Compute the magnitude (norm) of each rating vector.
4. Divide the dot product by the product of magnitudes.

This mathematical approach ensures accurate similarity measurement even when users have rated different numbers of items.

### 4. Generating Recommendations

After calculating similarity scores between the target user and all other users, the system:

* Ignores the target user.
* Multiplies similarity score with other users' ratings.
* Computes weighted scores for items the target user has not rated.
* Sorts items in descending order of weighted score.
* Returns the top N recommended items.

This ensures personalized and relevant suggestions.

### 5. User Interaction

The system allows the user to enter a username (User1, User2, User3, or User4). Based on the entered user, the program dynamically generates and displays top recommendations.

Example Output:
If User1 is entered, the system may recommend Item4 and Item5 based on similarity with other users.

### 6. Technical Concepts Used

* Java Collections Framework (HashMap, ArrayList, HashSet)
* Stream API for sorting and filtering
* Mathematical computation (cosine similarity formula)
* Object-oriented programming
* Data structure manipulation

### 7. Learning Outcomes

Through this task, I gained a strong understanding of:

* How recommendation systems work in real-world platforms like Netflix and Amazon.
* The difference between content-based filtering and collaborative filtering.
* How similarity metrics impact recommendation quality.
* Practical implementation of mathematical models in Java.

I also improved my knowledge of Java streams, data handling, and algorithm optimization.

### 8. Conclusion

The AI-Based Recommendation System successfully demonstrates how personalized suggestions can be generated using collaborative filtering techniques. The system is scalable and can be enhanced further by:

* Integrating Apache Mahout for large datasets.
* Connecting to a database instead of static sample data.
* Adding item-based collaborative filtering.
* Implementing a graphical user interface (GUI).

Overall, this task helped me understand the core logic behind intelligent recommendation engines and provided hands-on experience in implementing AI concepts using Java.

---

