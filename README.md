# Movie Reviews Application - Backend

## Introduction

This backend for the Movie Reviews Application is built using Java, Spring Boot, and MongoDB. It provides a RESTful API to manage movies and reviews, serving as the server-side component of the full-stack application.

## Technologies Used

- **Backend**: Java, Spring Boot
- **Database**: MongoDB, MongoDB Atlas, MongoDB Compass

## Setup Instructions

### MongoDB Atlas Configuration

1. **Create an Account**: Sign up on [MongoDB Atlas](https://www.mongodb.com/cloud/atlas).
2. **Create a Project**: Set up a new project and configure a MongoDB database.
3. **Database User and Security**: Create a new database user and configure IP access lists.
4. **Import Sample Data**: Optionally, you can import sample movie data using [JSON file](https://github.com/fhsinchy/movieist/blob/master/_data/movies.json) from Farhan Hasin Chowdhury GitHub repository.

### Backend Setup

1. **Clone the Repository**: 
   ```bash
   git clone https://github.com/Lenka03/moviesAPI.git

2. **Configure Database Connection**: Modify the application.properties file in the src/main/resources directory with your MongoDB connection details.

3. **Set Environment Variables**: Define the MongoDB connection details (e.g., database, user, password, cluster) in a .env file.

4. **Run the Application**: 
   ```bash
   ./mvnw spring-boot:run
  - *Access the frontend at localhost:8080.*

## Project Structure

- **Movie and Review Entities**: The application works with two main entities, `Movie` and `Review`, represented by separate classes.
- **Controllers**: `MovieController` and `ReviewController` manage API endpoints for movies and reviews.
- **Repositories**: Interfaces extending `MongoRepository` to handle database operations for movies and reviews.
- **Services**: Business logic encapsulated in `MovieService` and `ReviewService`.

## API Endpoints

- `GET /api/movies`: Retrieves all movies.
- `GET /api/movies/{id}`: Retrieves a single movie by ID.
- `POST /api/reviews`: Submits a review for a movie.

## Conclusion

This backend service is a critical component of the Movie Reviews Application, providing API functionalities and integrating with MongoDB for data persistence.

## Link to Frontend Repository

For the frontend part of this application, please visit [MovieClient](https://github.com/Lenka03/MovieClient) to set up and run the client-side code.
