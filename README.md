# BookBee project

BookBee is an app that connects you with a network of book lovers who are willing to lend or sell their books to you. You can browse through the catalog of available books, filter by genre, rating, price, or location, and request to borrow or buy the ones you like. You can also lend or sell your own books to other users and earn some extra cash or credit.

BookBee is more than just a book exchange app. It's also a community of readers who share their opinions, reviews, and recommendations. You can join book clubs, chat with other users, and discover new books to read. You can also earn rewards and badges for being an active member of the BookBee community.

BookBee is the ultimate app for book lovers who want to enjoy reading without spending a fortune. Download it today and start your book adventure! 🐝📚

## Requirements

Here is a possible list of functional and non-functional requirements for this project:

Functional requirements:

- The app should allow users to create an account and log in with their email and password.
- The app should allow users to browse through the catalog of available books, filter by genre, rating, price, or location, and request to borrow or buy the ones they like.
- The app should allow users to lend or sell their own books to other users by uploading the book details, setting the price or lending period, and accepting or rejecting requests.
- The app should allow users to chat with other users who have requested or offered their books, and arrange the delivery or pickup of the books.
- The app should allow users to join book clubs, chat with other members, and participate in book discussions and activities.
- The app should allow users to rate and review the books they have read or borrowed, and see the ratings and reviews of other users.
- The app should allow users to earn rewards and badges for being active members of the BookBee community, such as reading a certain number of books, lending or selling a certain number of books, joining a certain number of book clubs, etc.

Non-functional requirements:

- The app should have a user-friendly and attractive interface that follows the BookBee branding and design guidelines.
- The app should be secure and protect the privacy and data of the users. It should use encryption, authentication, and authorization mechanisms to prevent unauthorized access or misuse of the app.
- The app should be reliable and perform well under different network conditions and user loads. It should handle errors and exceptions gracefully and provide feedback to the users.
- The app should be compatible with different devices and platforms, such as Android, iOS, web browsers, etc. It should adapt to different screen sizes and orientations.
- The app should be scalable and maintainable. It should use modular and reusable code that follows the best practices and standards of software development. It should also use appropriate testing tools and methods to ensure the quality and functionality of the app.

## User stories

- As a user, I want to create an account and log in with my email and password, so that I can access the app and its features.
- As a user, I want to browse through the catalog of available books, filter by genre, rating, price, or location, and request to borrow or buy the ones I like, so that I can find and enjoy the books I want to read.
- As a user, I want to lend or sell my own books to other users by uploading the book details, setting the price or lending period, and accepting or rejecting requests, so that I can share my books with others and earn some extra cash or credit.
- As a user, I want to chat with other users who have requested or offered their books, and arrange the delivery or pickup of the books, so that I can communicate and coordinate with them easily and conveniently.
- As a user, I want to join book clubs, chat with other members, and participate in book discussions and activities, so that I can meet and interact with other book lovers and have fun.
- As a user, I want to rate and review the books I have read or borrowed, and see the ratings and reviews of other users, so that I can express my opinions and feedback and learn from others.
- As a user, I want to earn rewards and badges for being active members of the BookBee community, such as reading a certain number of books, lending or selling a certain number of books, joining a certain number of book clubs, etc., so that I can feel motivated and recognized for my achievements.

## Architecture

The micro service architecture consists of the following services and their responsibilities:

- **User Service**: This service handles the user management and authentication features, such as creating and logging in users, validating and refreshing tokens, updating user profiles, etc. It communicates with the User Database to store and retrieve user data.
- **Book Service**: This service handles the book management and exchange features, such as uploading and updating book details, requesting and offering books, rating and reviewing books, etc. It communicates with the Book Database to store and retrieve book data, and with the User Service to verify user identity and permissions.
- **Chat Service**: This service handles the chat and messaging features, such as sending and receiving messages, creating and joining chat rooms, etc. It communicates with the Chat Database to store and retrieve chat data, and with the User Service to verify user identity and permissions.
- **Book Club Service**: This service handles the book club and community features, such as creating and joining book clubs, participating in book discussions and activities, earning rewards and badges, etc. It communicates with the Book Club Database to store and retrieve book club data, and with the User Service to verify user identity and permissions.
- **API Gateway**: This service acts as a single entry point for all the requests from the clients. It routes the requests to the appropriate micro services based on the URL path, method, and parameters. It also performs load balancing, caching, logging, monitoring, security, etc. for the micro services.
- **Client**: This is the front-end application that interacts with the users. It can be a web browser, a mobile app, or any other device that can send HTTP requests to the API Gateway. It provides a user-friendly and attractive interface that follows the BookBee branding and design guidelines.
