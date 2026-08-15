# 🎬 Cinema Movie Ticket Booking System

## 📌 About the Project

The **Cinema Movie Ticket Booking System** is a backend REST API application developed using **Java and Spring Boot**. The project is designed to manage movies and movie ticket bookings through RESTful APIs.

The application uses **PostgreSQL** as the database and **Spring Data JPA/Hibernate** for database operations.

Users can view available movies, search movies based on different criteria, add new movies, update or delete movie details, book tickets, and view booking history.

## ✨ Features

* View all available movies
* Search movies by:

  * Title
  * Date
  * Location
  * Genre
* View movie details by ID
* Add new movies
* Update movie information
* Delete movies
* Book movie tickets
* Automatically manage available seats
* View booking history
* PostgreSQL database integration

## 🛠️ Technologies Used

* **Java**
* **Spring Boot**
* **Spring Data JPA**
* **Hibernate**
* **PostgreSQL**
* **Maven**
* **REST API**
* **Postman**
* **Eclipse IDE**
* **Git & GitHub**

## 🔗 REST API Endpoints

| Method   | Endpoint                                           | Description          |
| -------- | -------------------------------------------------- | -------------------- |
| `GET`    | `/movie`                                           | Get all movies       |
| `GET`    | `/movie/{id}`                                      | Get a movie by ID    |
| `POST`   | `/movie`                                           | Add a new movie      |
| `PUT`    | `/movie/{movieId}`                                 | Update movie details |
| `DELETE` | `/movie/{movieId}`                                 | Delete a movie       |
| `POST`   | `/movie/booking/{movieId}/{quantity}/{totalPrice}` | Book movie tickets   |
| `GET`    | `/movie/booking/history`                           | View booking history |

## 🗄️ Database

The project uses **PostgreSQL** to store movie and booking information.

The application connects to a PostgreSQL database using **Spring Data JPA and Hibernate**.

For security reasons, the `application.properties` file containing database credentials is **not included in this public repository**.

To run the project locally, create your own `application.properties` file inside:

```text
src/main/resources/application.properties
```

Example configuration:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5555/cinema_database
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/adii790/cinema-project.git
```

### 2. Open the project

Open the project in **Eclipse IDE** as an existing Maven project.

### 3. Configure PostgreSQL

Create the required PostgreSQL database and create your own:

```text
application.properties
```

file with your local database credentials.

### 4. Run the application

Run:

```text
CinemaProjectApplication.java
```

as a **Spring Boot Application**.

The application runs on:

```text
http://localhost:8081
```

## 🧪 API Testing

The REST APIs can be tested using **Postman**.

Example:

```text
GET http://localhost:8081/movie
```

To add a movie:

```text
POST http://localhost:8081/movie
```

Example request body:

```json
{
  "description": "An exciting action movie",
  "director": "Raj Kumar",
  "genre": "Action",
  "title": "The Last Mission",
  "date": "2026-08-20",
  "location": "Delhi",
  "totalSeats": 100,
  "availableSeats": 100,
  "price": 250
}
```

## 🎯 Learning Objectives

This project demonstrates practical implementation of:

* Spring Boot application development
* REST API creation
* CRUD operations
* Database connectivity
* JPA/Hibernate
* PostgreSQL integration
* API testing with Postman
* Git and GitHub version control



---

⭐ **This project was created as a practical backend development project using Java, Spring Boot, PostgreSQL, and REST APIs.**
