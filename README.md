# Restaurant Menu Explorer

## Project Overview

**Restaurant Menu Explorer** is a Python-based FastAPI application that allows users to fetch and filter restaurant menus using a public API. The app provides an endpoint to retrieve restaurant data and another to search by restaurant name, returning detailed information such as items, prices, and descriptions.

## Features

- Fetch all restaurant data in JSON format.
- Search for specific restaurants by name and retrieve their menu details.
- Save restaurant data locally as JSON files using Python scripts.

## Requirements

To run this project, you'll need the following dependencies:

- Python 3.8+
- FastAPI
- Uvicorn
- Requests

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/DonGraeff/restaurant-menu-explorer
    cd restaurant-menu-explorer
    ```

2. Create a virtual environment:

    ```bash
    python -m venv venv
    ```

3. Activate the virtual environment:

    - On Windows:
      ```bash
      venv\Scripts\activate
      ```

    - On Linux/MacOS:
      ```bash
      source venv/bin/activate
      ```

4. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Running the Application

1. Start the FastAPI server with Uvicorn:

    ```bash
    uvicorn main:app --reload
    ```

2. Open your browser and navigate to:

    ```
    http://127.0.0.1:8000/api/restaurants/?restaurant=KFC
    ```

3. To fetch all available restaurant data, go to:

    ```
    http://127.0.0.1:8000/api/restaurants/
    ```

## Code Structure

- **`main.py`**: Handles the API routes and serves restaurant data dynamically through query parameters.
- **`app.py`**: Fetches restaurant data from the public API and saves it locally as JSON files for offline access.

## Example Usage

- Retrieve all restaurant data:

    ```bash
    http://127.0.0.1:8000/api/restaurants/
    ```

- Retrieve the menu for a specific restaurant (e.g., KFC):

    ```bash
    http://127.0.0.1:8000/api/restaurants/?restaurant=KFC
    ```

## Dependencies

- **FastAPI**: Web framework for building APIs
- **Uvicorn**: ASGI server to serve FastAPI
- **Requests**: To make HTTP requests for fetching restaurant data

## Contributing

Feel free to fork the project and submit pull requests. Contributions are always welcome!
