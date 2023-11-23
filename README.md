Weather Data Centralization API
This document provides a simplified explanation of a project that involves building an API for centralizing weather data from various sources. The API is designed to consume different weather data sources and centralize them into a single response per location. It also maintains information about the API consumers for billing purposes.

Application Overview
The application is designed to consume weather data from various sources, including data about locations, wind, temperature, air quality, and cloudiness. It also maintains a record of API consumption by clients, who are identified using a unique email address and are charged for integration services at the end of each month.

How to Test the Application
The application provides several endpoints that you can use to test its functionality:

Register a new consumer API: This endpoint allows you to register a new consumer for the API. You will need to provide an email address and a preferred temperature unit.

Get locations: This endpoint returns information about all available locations.

Weather request by location with datetime filter: This endpoint returns weather information for a specific location. You can also provide a datetime parameter to get weather information for a specific time.

You can use tools like Postman or curl to send HTTP requests to these endpoints and check the responses.

How to Run the Application in Docker
To run the application in Docker, you will need to build a Docker image of the application and then run a container using that image. Here are the steps:

Build the Docker image: Run the command docker build -t weather-api . in the root directory of the project. This will create a Docker image named weather-api.

Run the Docker container: Run the command docker run -p 8080:8080 weather-api. This will start a Docker container and map port 8080 of the container to port 8080 of your host machine.

Access the application: You can now access the application at http://localhost:8080.

Please note that you need to have Docker installed on your machine to run the application in Docker.
