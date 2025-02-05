# Text-Generation-App

## Project Overview:
FastAPI: A modern, fast (high-performance) web framework for building APIs with Python 3.6+ based on standard Python type hints.

Transformers: A library developed by Hugging Face that provides pre-trained models for natural language processing tasks. In this project, it’s used for text generation.

## Main Features:
### Home Endpoint (GET /):
A simple greeting endpoint that returns {"message": "Hello World"}.
### Text Generation Endpoint (GET /generate):
This endpoint accepts a text string as input (text query parameter), processes it using the pre-trained Flan-T5 model (from Hugging Face's google/flan-t5-small), and returns the generated text as a response.

## Docker Setup:
Docker: The project includes a Dockerfile that sets up the application in a containerized environment. This allows the app to be deployed anywhere with Docker support, ensuring consistency across different environments.

The base image used is python:3.9.

Required dependencies are installed from a requirements.txt file.

The application is set to run with Uvicorn (an ASGI server) on port 7860, making it accessible through the specified host and port.
