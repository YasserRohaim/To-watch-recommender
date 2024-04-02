# To-Watch Recommender

This project is a web application that recommends movies and series to users based on their input using a content-based recommendation system. The system calculates cosine similarity to find similar shows from a database filled by web scraping IMDb with bueatifulsoup. This content based recommendation is built using sikitlearn. The backend is built with FastAPI and MongoDB, while the frontend utilizes HTML, CSS, and JavaScript.

## Setup

### Prerequisites

You will need Python3 running on your machine

### Installation

1. Clone this repository:

    ```
    git clone https://github.com/YasserRohaim/To-watch-recommender
    ```

2. Install dependencies:

    ```
    pip install -r requirements.txt
    ```

### Running the Application

1. Start MongoDB server:

    ```
    mongod
    ```

2. Run the FastAPI application:

    ```
    python main.py
    ```

3. Access the application in your web browser at `http://localhost:80`

## Project Structure

- `main.py`: Main FastAPI application entry point.
- `app/routers`: Contains router definitions for handling different endpoints.
- `app/logic`: Contains the logic for recommendation system and scraping.
- `app/schemas`: Contains data schemas.
- `templates`: Contains HTML templates for frontend.
- `static`: Contains static files (CSS, JavaScript).

## Endpoints

- `/`: Home page.
- `/moviesearch`: Page for searching movies.
- `/recommend`: Endpoint for receiving recommendations based on user input.
- `/recommends`: Endpoint for receiving recommendations based on multiple movies.
- `/scrape`: Endpoint for initiating web scraping of IMDb.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License - see the license file for details.

