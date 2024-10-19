# Ecommerce Restful Application

## Overview
This project is an **Ecommerce Restful Application** built using **Spring Boot**, with a focus on providing a secure and scalable backend solution for an e-commerce platform. The application supports **role-based authentication** with **Spring Security** and **JWT tokens** to ensure secure access control for different types of users, such as **Admin** and **Customer**.

## Features
- **Restful API**: Fully functional APIs for managing products, users, orders, and carts.
- **Role-Based Authentication**: Implemented **JWT token-based** authentication for securing endpoints based on user roles (Admin/Customer).
- **User Roles**:
  - **Admin**: Manage products, view all orders, manage users.
  - **Customer**: Browse products, place orders, manage their cart.
- **JWT Token**: Users receive a JWT upon login to securely access protected routes.
- **Spring Security**: Used to implement role-based access control and JWT token validation.

## Technologies Used
- **Backend**: Java, Spring Boot
- **Security**: Spring Security, JWT (JSON Web Tokens)
- **Database**: MySQL (or any other preferred RDBMS)
- **ORM**: Hibernate
- **Tools**: Gradle, IntelliJ IDEA
- **Version Control**: Git, GitHub

### Role-Based Access
- **Admin**: Full access to manage products, users, and orders.
- **Customer**: Access to view products, manage their cart, and place orders.

## How JWT Authentication Works
1. **Register/Login**: Users (Admin/Customer) can register or login via `/api/auth/register` or `/api/auth/login`.
2. **Token Issuance**: After successful login, a JWT token is generated and returned to the user.
3. **Accessing Protected Endpoints**: The user must include the JWT token in the `Authorization` header when making requests to protected endpoints.
4. **Role Validation**: Spring Security validates the token and grants access based on the user's role.

