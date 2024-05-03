# FinalProject
# Final Project: FastAPI SQLite Integration

## Introduction

Welcome to the FastAPI SQLite Integration project! This project showcases a simple CRUD (Create, Read, Update, Delete) API built using the FastAPI framework with SQLite database integration. It provides endpoints to manage customers, items, and orders efficiently.

## Features

- **Customer Management:** Create, read, update, and delete customers.
- **Item Management:** Create, read, update, and delete items.
- **Order Management:** Create and read orders.

## Prerequisites

Before running the project, ensure you have the following:

- Python 3.7 or later installed.
- Virtual environment set up.

## Execution Steps

To run the project, follow these steps:

1. **Create a virtual environment:**
   - For Windows:
     ```
     python -m venv venv
     venv\Scripts\activate
     ```
   - For macOS/Linux:
     ```
     python -m venv venv
     source venv/bin/activate
     ```

2. **Install dependencies:**
   ```
   pip install fastapi uvicorn pydantic
   ```

3. **Initialize the SQLite database:**
   ```
   python db_init.py
   ```
   This script creates necessary tables and populates them with sample data from `example_orders.json`.

4. **Run the FastAPI server:**
   ```
   uvicorn main:app --reload
   ```
   The server will start running on `http://127.0.0.1:8000`.

5. **Access the API documentation:**
   Open your web browser and navigate to `http://127.0.0.1:8000/docs` to access the Swagger UI. Here, you can explore and interact with the API endpoints.

## API Endpoints

### Customers:
- **POST /customers/:** Create customer
- **GET /customers/{cust_id}:** Read Customer
- **PUT /customers/{cust_id}:** Update Customer 
- **DELETE /customers/{cust_id}:** Delete Customer 

### Items:
- **POST /items/:** Create item
- **GET /items/{item_id}:** Read item 
- **PUT /items/{item_id}:** Update item 
- **DELETE /items/{item_id}:** Delete item 

### Orders:
- **POST /orders/:** Create Order
- **GET /orders/{order_id}:** Read Order 
- **PUT /orders/{order_id}:** Update Order 
- **DELETE /orders/{order_id}:** Delete Order 

This project provides an easy-to-use API for managing customers, items, and orders. Feel free to explore and utilize these endpoints as per your requirements.
