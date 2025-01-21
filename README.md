# alx-project-0x14

## API Overview

The **MoviesDatabase API** provides access to a wide range of movie-related data, including movie details, cast information, reviews, and more. It allows developers to integrate movie data into their applications, search for movies, and filter results based on various criteria such as genres, release dates, and ratings.

## Version

The current version of the MoviesDatabase API is **v1.0**.

## Available Endpoints

### 1. **GET /movies**
   - **Description**: Retrieve a list of movies from the database. You can filter movies based on various parameters such as genre, release date, and popularity.
   - **Example Request**: `GET https://api.moviesdatabase.com/v1/movies`

### 2. **GET /movies/{id}**
   - **Description**: Get detailed information about a specific movie by its unique ID.
   - **Example Request**: `GET https://api.moviesdatabase.com/v1/movies/12345`

### 3. **GET /genres**
   - **Description**: Fetch a list of available movie genres.
   - **Example Request**: `GET https://api.moviesdatabase.com/v1/genres`

### 4. **GET /movies/{id}/cast**
   - **Description**: Get a list of cast members for a particular movie.
   - **Example Request**: `GET https://api.moviesdatabase.com/v1/movies/12345/cast`

### 5. **GET /search**
   - **Description**: Search for movies based on keywords or filter criteria such as genre, release year, or rating.
   - **Example Request**: `GET https://api.moviesdatabase.com/v1/search?query=action`

## Request and Response Format

### Request Example (GET /movies)
```http
GET https://api.moviesdatabase.com/v1/movies?genre=action&release_year=2020