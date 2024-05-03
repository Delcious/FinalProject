# FinalProject
# Final Project

## Features

- **Customer Management:** Create, read, update, and delete customers.
- **Item Management:** Create, read, update, and delete items.
- **Order Management:** Create and read orders.

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
   pip install fastapi uvicorn
   ```

3. **Initialize the SQLite database:**
   ```
   python db_init.py
   ```

4. **Run the FastAPI server:**
   ```
   uvicorn main:app --reload
   ```
   The server will start running on `http://127.0.0.1:8000`.

5. **Access the API documentation:**
   Open your web browser and navigate to `http://127.0.0.1:8000/docs`. 

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

 
