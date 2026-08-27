# Pincode Lookup API

A FastAPI-based REST API for looking up Indian pincode location information with input validation, structured responses, and custom error handling.


## Problem

Applications such as checkout systems, delivery platforms, and address forms often need to validate a user's pincode and retrieve location information such as city, state, and district.

This API provides a simple interface for performing pincode lookups while handling invalid input and missing pincodes with structured error responses.

## Problem

Applications such as checkout systems, delivery platforms, and address forms often need to validate a user's pincode and retrieve location information such as city, state, and district.

This API provides a simple interface for performing pincode lookups while handling invalid input and missing pincodes with structured error responses.

## Request Flow

The API processes requests through the following stages:

1. Client sends a pincode request.
2. FastAPI receives the request.
3. Pydantic validates the pincode format.
4. The application searches the pincode dataset.
5. A matching location is returned if found.
6. Custom exceptions generate structured error responses for invalid or missing pincodes.

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/pincode/{pincode}` | Lookup a single pincode |
| POST | `/pincode/bulk` | Lookup multiple pincodes |


## Tech Stack

- Python
- FastAPI
- Pydantic
- Uvicorn

Pincode-Lookup/
│
├── main.py
├── models.py
├── data.py
├── exceptions.py
├── requirements.txt
├── README.md
└── .gitignore