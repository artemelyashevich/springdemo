## Project Overview

This project provides a secure user authentication system with the following features:
- User registration
- User login
- Password encryption

## Technologies Used

- Java 21
- Spring Boot 3.4.4
- Spring Security
- Spring DataJpa
- Thymeleaf 
- Bootstrap 5 
- Mysql

## Setup Instructions

### Prerequisites

- JDK 21 or higher
- Maven 3.8+
- Your preferred IDE (IntelliJ IDEA, Eclipse, etc.)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/artemelyashevich/springdemo.git
   cd demo
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

## API Endpoints

### Authentication

| Endpoint  | Method | Description                  |
|-----------|--------|------------------------------|
| `/signIn` | GET    | Display login form           |
| `/signIn` | POST   | Process login request        |
| `/signUp` | GET    | Display registration form    |
| `/signUp` | POST   | Process registration request |
| `/logout` | POST   | Logout current user          |
| `/users`  | Get    | Display all users            |

## Security Configuration

The application uses Spring Security with the following configuration:
- BCrypt password encoding
- Form-based authentication

## Usage

### Registration

1. Go to `/signUp`
2. Fill in the registration form
3. Submit the form

### Login

1. Go to `/signIn`
2. Enter your credentials
3. Submit the form
4. On successful authentication, you'll be redirected to the home page

### Logout

1. Make a POST request to `/logout`
2. You'll be redirected to the login page with a logout message
