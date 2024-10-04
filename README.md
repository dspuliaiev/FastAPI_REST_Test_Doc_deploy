# REST API for storing and managing contacts. 
The API is built using the FastAPI infrastructure and utilizes the SQLAlchemy ORM to manage the PostgreSQL database using the Pydantic data validation module.

## Table of contents
* [General info](#general-info)
* [Setup](#setup)

## General info
In the application:
*  an authentication mechanism is implemented;
*  implemented an authorization mechanism using JWT tokens;
*  a mechanism for verifying the registered user's email is implemented;
*  the number of requests to the main contact routes is limited; 
*  the speed of creating contacts for the user is limited;
*  CORS is enabled;
*  the ability to update the user's avatar is implemented, the Cloudinary service is used;
*  all environment variables are stored in the .env file; 
*  Docker compose is used to run all services and databases in the application;
*  documentation was created using Sphinx;
*  module tests covered the repository modules using the Unittest framework; 
*  functional tests covered the main routes using the pytest framework.


## Setup:

1. Clone the repository:
    ```
    git clone https://github.com/dspuliaiev/REST_FastAPI_Doc_Test
    ```

2. Install dependencies:
    ```
    poetry install
    ```

3. Run the container:
    ```
    docker-compose up
    ```

4. Apply changes:
    ```
    alembic upgrade head
    ```

5. Run the server:
    ```
    python main.py
    ```


