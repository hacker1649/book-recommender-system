## Book Recommender System

### Introduction:

In today's digital age, where the abundance of choices can sometimes overwhelm users, recommender systems play a pivotal role in aiding decision-making processes. This project focuses on developing a sophisticated book recommender system which employs a hybrid approach by integrating two distinct recommendation techniques: content-based filtering and deep neural networks. The aim is to provide users with personalized recommendations based on their preferences and historical interactions with books. By combining these approaches, the recommender system aims to provide more accurate and diverse recommendations, enhancing the overall user experience, engagement, and retention, thereby benefiting both readers and book platforms alike.

### Dataset:

The dataset used in this project was sourced from Kaggle and is titled "Goodreads Best Books." This dataset provides comprehensive information about a wide range of books, including their titles, authors, ratings, genres, and descriptions. The dataset consists of the following key attributes:
1.	book_id: Unique identifier for each book.
2.	book_title: Title of the book.
3.	book_authors: Author(s) of the book.
4.	book_desc: Description of the book, providing insights into its content and theme.
5.	genres: Genres associated with the book, categorizing it into different literary categories.
6.	book_format: Format of the book (e.g., paperback, hardcover, ebook).
7.	book_rating: Average rating of the book on Goodreads.
8.	book_rating_count: Number of ratings the book has received on Goodreads.
9.	book_review_count: Number of reviews the book has received on Goodreads.
By utilizing this dataset, this project can analyze and suggest books based on factors like content similarity and popularity. This enables the system to offer personalized book recommendations aligned with users' preferences and interests, thereby enhancing their experience and engagement with the platform.

Source: [Goodreads Books Dataset | Kaggle](https://www.kaggle.com/competitions/goodreads-books-reviews-290312)

### Model Explanation:

The project utilizes a Content-based filtering approach and DNN (Deep Neural Network) approach, both widely-used techniques in recommendation systems. 

The content based approach suggests items similar to those the user has previously shown interest in. In the context of book recommendations, the system identifies books that are similar to those the user has read or interacted with before. This is achieved by analyzing textual attributes such as descriptions, genres, and authors.

### Results:

#### CNNS:

The calculate_precision function computes the precision score, which measures the proportion of relevant items recommended by the system among all items recommended. If no items are recommended, it returns 0 to avoid division by zero. Otherwise, it calculates precision by dividing the number of relevant items recommended by the total number of items recommended.

An example demonstrates its usage, where 4 out of 5 recommended items are deemed relevant by the user. This results in a precision score of 0.8.

![cnn](https://github.com/hacker1649/book-recommender-system/assets/88313681/df439d58-70df-4419-85e8-c5b08bc3a077)

#### DNN:

The plot shows how the validation error changes with each training epoch. As the model learns from more data, the validation error decreases, indicating improved performance in predicting user preferences for books. The minimum validation error achieved is 0.8378, suggesting that the deep neural network (DNN) model is effectively learning to recommend books to users.

![dnn](https://github.com/hacker1649/book-recommender-system/assets/88313681/2ce1e0be-2ead-46a4-a58c-c6721e99fdce)

