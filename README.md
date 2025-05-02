# Laravel-project
Laravel Restaurant Website

Overview

This project is a Restaurant Management System built using Laravel. It provides functionality for administrators to manage restaurant operations efficiently, including categories, menus, contact information, and orders. For users, the website serves as an online platform to explore the restaurant menu and place food orders, making it easy to enjoy the restaurant's offerings from anywhere.

Features

Category Management: Admins can create, update, and delete categories for organizing the menu.
Menu Management: Add, edit, and delete menu items with details like pricing, description, and categories.
Contact Management: Manage the restaurant's contact information, including phone numbers, addresses, working hours, and social media handles.
Order Management: View and process customer orders efficiently.
Explore Menu: Customers can browse the restaurant's menu, filter by categories, and view detailed information about each item.
Online Food Ordering: Users can add menu items to their cart, place orders online, and receive confirmation for their orders.
Responsive Design: The website is fully responsive, ensuring it works seamlessly on all devices.
Dynamic Content: Admins can update information like working hours, addresses, and phone numbers dynamically.
Demo

Check out the live demo of the project: Restaurant Management System Demo

Screenshot Screenshot

Security

Best practices are being employed in this project according to the latest Laravel 11 documentation. This includes proper data encryption and two-factor authentication to ensure the security and privacy of user data.

Tools & Technologies Used

Laravel Framework: PHP framework for building robust web applications.
MySQL: Database for storing restaurant data (menus, orders, contact info, etc.).
AdminLTE 3: For the admin dashboard interface (AdminLTE 3 Dashboard).
HTML5 & CSS3: For building the front-end structure and design.
JavaScript & jQuery: For interactive elements and dynamic behavior.
Bootstrap: For responsive design and layout.
Templatemagic: Portfolio template (Portfolio by Templatemagic).

Security

Best practices are being employed in this project according to the latest Laravel 11 documentation. This includes proper data encryption and two-factor authentication to ensure the security and privacy of user data.

Tools & Technologies Used

Laravel Framework: PHP framework for building robust web applications.
MySQL: Database for storing restaurant data (menus, orders, contact info, etc.).
AdminLTE 3: For the admin dashboard interface (AdminLTE 3 Dashboard).
HTML5 & CSS3: For building the front-end structure and design.
JavaScript & jQuery: For interactive elements and dynamic behavior.
Bootstrap: For responsive design and layout.
Templatemagic: Portfolio template (Portfolio by Templatemagic).
Libraries Used

This project utilizes the following libraries for enhanced functionality:

ezyang/htmlpurifier (4.18.0): Standards-compliant HTML filter written in PHP to ensure clean and secure HTML content.
intervention/image-laravel (1.3.0): Laravel integration of Intervention Image for image manipulation.
yajra/laravel-datatables-oracle (11.1.5): jQuery DataTables API for Laravel, simplifying server-side processing.
stripe/stripe-php (16.4.0): Stripe PHP library for payment processing and integration.
getcountrycurrency/country-currency-api (1.0.0): A PHP library for fetching country currency details.
How to Deploy On Shared Host Cpanel

Deploy On Shared Host Cpanel

How to Run This Project on Your Local Machine

Follow these steps to set up and run the project locally:

Step 1: Clone the Repository

git clone https://github.com/chrysanthusobinna/laravel-restaurant.git
cd laravel-restaurant
Step 2: Set Up the Environment

Rename .env.example to .env:
mv .env.example .env
2. Configure Your .env File

Set up your .env file with the following configurations:

Database Connection

Define the database connection settings:

DB_CONNECTION=sqlite  
# DB_HOST=  
# DB_PORT=  
# DB_DATABASE=  
# DB_USERNAME=  
# DB_PASSWORD=  
Mail Configuration

Set up mail configurations:

MAIL_MAILER=log  
MAIL_HOST=1  
MAIL_PORT=  
MAIL_USERNAME=  
MAIL_PASSWORD=  
MAIL_ENCRYPTION=  
MAIL_FROM_ADDRESS=  
Stripe Configuration

Get your Stripe secret key and webhook secret from Stripe:

STRIPE_SECRET=sk_xxxxxxxxxxxxxx
STRIPE_WEBHOOK_SECRET=whsec_xxxxxxxxxxxxxxxxxxxxxxxx
Google Maps API Key

Get your Google Maps API key from the Google Cloud Console:

GOOGLE_MAPS_API_KEY=AIzaSyCDC0tAy9sV41Wwa9Ou-Kch95GJIQ51JKw  
Company Address

Set the company address here. Note that the address saved in the database will take precedence, and this will only serve as a fallback:

ADDRESS="Bradshawgate Bolton, BL1 1QD"  
--

Step 3: Set Up the Database

Create a new MySQL database (e.g., restaurant_db).
Run migrations and seeders:
php artisan migrate
Step 4: Start the Application

Run the application on port 8000 or any port of your choice:

php artisan serve --port=8000
Visit the application at http://127.0.0.1:8000.

Step 5: Create an Admin User

To create an admin user with global rights:

Edit the UserSeeder file located at database/seeders/UserSeeder.php and set the user details as desired.
Run the following command to seed the user:
php artisan db:seed --class=UserSeeder
This user account will have global rights and can be used to create other user accounts.

Credits

BootstrapDash: The admin dashboard celestialAdmin admin template design is powered by BootstrapDash, offering a modern and customizable interface.
Templatemagic Portfolio: The front-end template for the website is inspired by Templatemagic's portfolio designs.
Feel free to fork this repository or contribute to its development by submitting a pull request!

