# Calculator API

## Goal
Creating a basic calculator API providing RESTful endpoints for performing basic arithmetic operations.
The API is built using Python, Poetry for dependency management, and FastAPI for the web framework.

## Approach

### API Design
1. I will implement endpoints with clear names for each arithmetic operation (e.g., `/add`, `/subtract`, `/multiply`, `/divide`).
2. Each endpoint will accept two query parameters, which will be validated to ensure they are numbers.
3. The API will return the result in a JSON format, showing if the operation was successful or if there was an error, along with an appropriate HTTP status code.
4. Error handling will be implemented to manage cases such as invalid input and division by zero.

### Project Structure
- `main.py`: The startup place of the FastAPI application.
- `routes/*`:  directory to hold route definitions for each arithmetic operation.
- `services/*`: directory to hold the business logic for the calculation methods.
- `schemas/*`: directory to hold Pydantic models for request validation and response formatting.
- `tests/*`: directory for unit tests for the correctness of the API endpoints.
