# Ecommerce_Follow_Along
"Ecommerce-Follow-Along"

## Milestone 1: Project Overview

In today's live session, our mentor introduced us to the overall structure of the MERN Stack. He taught us the foundational steps to set up the environment for future milestones, and we created a new repository for our follow-along project.

## Milestone 2: Front-end Setup and Login Page

In today's live session, we learned to organize the files into separate frontend and backend directories.

- Set up React for the frontend
- Node.js setup for the backend
- Tailwind CSS configurations


## Milestone 3: File Organizing and MongoDB

Set up dedicated folders for organizing backend code effectively. Initialize and configure a Node.js server to handle API requests. Connect your application to MongoDB to store and manage data. Implement basic error handling to ensure your server runs smoothly.

## Milestone 4: Created and Configured Files

Created a User Model: Our mentor explained how a MODEL in MVC architecture works and how it interacts with the database. Created a User Controller: We got to know the purpose of a controller in MVC. Enable and Configure Multer: In the live session, our mentor told us what Multer is, what it is used for, and how it can be configured to handle file uploads.

## Milestone 5: Created Frontend UI for Signup Page and Added the Code for Authentication of the Inputs

In this part of the Follow Along project, we made the UI (Frontend) for the signup page of our website. This page allows users to add their details.

After the user is done with entering, the backend comes into play. The backend does the form validation part, verifying whether the user has entered the details in the right format (e.g., email, minimum length).

## Milestone 6: Encrypt the Password Using bcrypt

- During the user signup process, encrypt the user's password using the bcrypt hashing algorithm. This ensures that the password is stored in a secure, non-reversible format. The bcrypt algorithm adds a "salt" to the password before hashing, making it resistant to common password-cracking techniques. The hashed password should never be stored in plain text.
- Save the Hashed Password in the Database: Only store the hashed version of the password in the database. Do not store plain text passwords for security reasons. Ensure the hashed password is securely saved in the database along with other user information.
- Store Complete User Data: In addition to the hashed password, save the user's other information, such as their name, email, and any other relevant data. The complete user data should be stored securely, ensuring that sensitive information like the password remains encrypted.
- Handle Login with Hashed Passwords: During the login process, compare the entered password with the hashed version stored in the database. Use bcrypt to safely verify if the entered password matches the stored hash.

## Milestone 7: Create Login Endpoint

- Accept user credentials (email/username and password). Retrieve the corresponding user from the database.
- Validate Password: Use bcrypt to hash the entered password. Compare it with the stored hashed password for authentication.

## Milestone 8: Create the Card Component

- Design a reusable card component with props for product details (e.g., name, image, price).
- Design the Homepage Layout: Set up a grid layout or flexbox for displaying multiple cards neatly.

## Milestone 9: Create the Form for Products

This form will take multiple product images as input.

## Milestone 10: Define the Structure of Product Data

- Define the structure of product data (e.g., name, description, price, image URL) using Mongoose. Ensure each field has proper validation (e.g., required fields, correct data types).
- Build a POST endpoint to receive product data.
- Validate and save the product details to MongoDB.

## Milestone 11: Write an Endpoint to Send All Products Data to Frontend

- In the frontend, write a function to get all the data.
- Display these data dynamically by passing them to the product card component.

## Milestone 12: Write an Endpoint to Send All Products with User Mail to Frontend

- In the frontend, write a function to get all the data.
- Display these data dynamically by passing them to the product card component.

## Milestone 13: Write an Endpoint to Receive New Data and Update Existing Data in MongoDB

- In the frontend, add an edit button to the product card. When clicked, send the data to the form and make it auto-fill with the option to edit those data and save.

## Milestone 14: Write an Endpoint to Delete Data from MongoDB Using ID

- In the frontend, add a delete button to the product card. When clicked, send the product ID to the server endpoint.

## Milestone 15: Create and Reuse Nav Component

- Learn how to create a nav component.
- Learn how to reuse the same component on multiple pages.

## Milestone 16: Create a New Page to Display Each Product

- Learn how to create a new page to display each product.
- Add quantity and add-to-cart buttons.


## Milestone 17: Edit the User Schema to Store Cart Products

- In this milestonw we will be Editing the user schema to store cart products.
- **Write an Endpoint to Receive Product Details**: Learn how to create a new endpoint that accepts
product details (e.g., product ID, quantity) from the frontend.
-**Store Product Details in Database**: Learn how to implement the logic to add the received product details to the user's cart in the database. Ensure that the cart is updated correctly and that the product details are stored securely.


## Milestone 18: Create Backend Endpoints for Cart Page

- Create an endpoint to receive requests from the cart page.
- Create a backend endpoint to fetch all the products inside the cart using the user's email.


## Milestone 19: Create Cart Page and Manage Product Quantity

- Create cart frontend page and display the products
- For each product add an option to increase and decrease quantity using + and - buttons.
- Create an Backend endpoint for increase and decrease quantity


## Milestone 20: Create User Profile Page


- Create an Backend endpoint that will sent user data
- Create frontend profile page
- Display profile photo, name and email in one section
- In another section display address and add an button called "Add address"
- If there are no address display "No address found"

## Milestone 21: Create Address Form

- Create address form frontend page
- Create an state that will store input address
- When we click on add address in profile it should navigate to this form page.

## Milestone 22: Save Address Inside User Profile

- You need to create an endpoint that will receive the address from address form in frontend
- Add the address to the address array inside user collection.


## Milestone 23: Place Order Flow

- Create an placeorder button inside cart page and navigate to select address page when clicked.
- Create and select address page that will display all the available address and have an option to select one address.
- Write an backend endpoint that will send all the addresses of the user.


## Milestone 24: Place Order & Select Address Flow

- Add a Place Order button inside the cart.
- Create a Select Address page to display all saved addresses.
- Allow users to select one delivery address.
- Write a Mongoose schema for storing order details.
- Build a backend API endpoint to fetch user addresses.


## Milestone 25 – Backend Endpoint for Placing Orders

- You need to create an endpoint that will receive the products, user, address details
- You will get the mail of the user using that you need to retrive the _id of the user
- For each product the order will be different with same address
- Using order schema you created earlier you will store order details in mongodb order collection


## Milestone 26 – Get All Orders of a User

- You need to create an endpoint that will receive the user mail
- You will get the mail of the user using that you need to retrive the _id of the user
- Using that _id you need to get all the orders of that user
- Send all the users orders in the response.

## Milestone 27 – Build & Display User Orders on the Frontend

- You need to create an my-orders page
- You will send an get request to my-orders endpoint that we created in previous milestone.
- We will send user mail in to endpoint to get all the user orders
- Display all the user orders
- We will add my-orders page in navbar for better navigation.