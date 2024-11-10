## Bookstore Microservices
A small e-commerce platform with core functionalities broken into individual services.

## Microservices Overview
1. **Book Service # Built with Express**

    - Stores information about books (title, author, genre, price).
    - Exposes endpoints for adding, retrieving, updating, and deleting book entries.
2. **Order Service # Built with NestJS**

    - Manages customer orders.
    - Exposes endpoints for creating orders, viewing order details, and updating order status.
    - Interacts with the Book Service to verify book availability and prices.
3. **Payment Service # Built with NestJS**

    - Simulates payment processing for orders.
    - Exposes endpoints to initiate and verify payments.
    - Interacts with the Order Service to finalize the order after successful payment.
4. **User Service (optional) # Built with NestJS**

    - Handles user registration and login.
    - Can generate JWTs for securing interactions with other services.