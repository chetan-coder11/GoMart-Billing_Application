
# GoMart - E-commerce Application

GoMart is a comprehensive e-commerce application built using Spring Boot on the backend and React.js on the frontend. The application features user authentication, category management, product management, cart operations, and order processing. It also includes an POS dashboard for managing products and categories, with integrated image storage using Cloudinary.

# Key Features:

- User Authentication: Register and log in securely.
- Product Management: Add, update, delete, and view products with category associations.
- Cart Operations: Manage your shopping cart, checkout.
- Order Processing: Handle order placements with a streamlined process.
- POS Dashboard: Manage products, categories, and settings through a dedicated interface.
- Image Upload: Images are uploaded and stored using Cloudinary.

# Technologies Used:
# Backend
- Java 17
- Spring Boot 3.x
- JPA/Hibernate
- MySQL
- Cloudinary (for image uploads)
- Maven

# Frontend
- React.js
- Axios (for API calls)
- React Router
- Bootstrap (for styling)

# Database Schema
The project uses the following database schema:

- usermaster: Stores user credentials and information.
- categorymaster: Stores product categories.
- productmaster: Stores product details.
- cartmaster: Stores user cart information.
- settingmaster: Stores business settings.
- customermaster: Stores customer details.

# API Endpoints

# User API
 1) POST /GoMart/user/loggedin - Authenticate a user

# Category API
  1) GET   /GoMart/category - Get all categories
  2) Post  /GoMart/category/addCategory - Add Category
  3) PUT   /GoMart/category/updateCategory/{categoryId) - Update category
  4) DELETE  /GoMart/category/deleteProduct/{categoryId} - Delete Category
     
 # Product API
  1) GET  /GoMart/product - Get all Products
  2) GET /GoMart/product/{categoryName} - Get all Products by categoryname
  3) POST  /GoMart/product/addProduct  - Add product
  4) PUT  /GoMart/product/updateProduct/{productId}  - Update product
  5) DELETE /GoMart/product/deleteProduct/{productId}   - Delete Product

# Customer API
  1) POST  /GoMart/customer/addCustomer  - Add customer
     
# Cart API
  1) POST  /GoMart/cart/addToCart - Add product to the cart for billing process
     
# Setting API
  1) GET  /GoMart/settings  - Get all settings
  2) POST  /GoMart/settings/addSettings  - Add settings
  3) PUT  /GoMart/product/updateSettings/{settingId}   - Update the setting
 
# Raw API for addToCart 
{
    "products": [
        {
            "productid": 1
        },{
            "productid": 2
        },{
            "productid": 3
        },{
            "productid": 4
        }
    ],
    "qty": 4,
    "subTotal": 100.0,
    "discountPercentage": 10.0,
    "discountAmount": 10.0,
    "netBill": 90.0,
    "paymentType": "Cash",
    "customer": {
        "customer_id": 5
    }
}

#Output
1) Log In :-
![Screenshot (68)](https://github.com/user-attachments/assets/cf23bbaa-e61b-4b89-981b-e406066fc86e)

2)POS :-
![Screenshot (70)](https://github.com/user-attachments/assets/6cf71cbf-43e1-4452-b15a-5b31190a295d)

3)Billing :-
![Screenshot (71)](https://github.com/user-attachments/assets/31dac855-5cfe-4eb5-afab-592da6b88e77)

4)Products :-
![Screenshot (72)](https://github.com/user-attachments/assets/232dce15-7d3e-47b2-9f26-89962ce2906b)

4)Category :-
![Screenshot (73)](https://github.com/user-attachments/assets/ba9a51e2-f5ac-4a5f-ac2a-93bbd87f2b19)

5)Reports :-
![Screenshot (74)](https://github.com/user-attachments/assets/5000822c-52ee-4cb7-b159-0b92cf1e60ac)

6)Business Setting :-
![Screenshot (75)](https://github.com/user-attachments/assets/7193f764-6b67-4061-a1e2-71875223cd40)
