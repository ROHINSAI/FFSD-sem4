# FFSD - Sem 4

Chasing Horizons - A comprehensive Tourism and Hotel Booking website

## Formats and Syntax

SPACING SYSTEM (px) \
2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80 / 96 / 128

FONT SIZE SYSTEM (px) \
10 / 12 / 14 / 16 / 18 / 20 / 24 / 30 / 36 / 44 / 52 / 62 / 74 / 86 / 98

01 - Typography \
02 - Font Weights \
03 - Line Heights \
04 - Colors (Primary, Tints, Shades, Greys) \
05 - Spacing System \
06 - Shadows \
07 - border radius

## Folder Structure Explained

Controller -> Contains all the js files that handles user requests \
Model -> Contains all the js files where we define the Database Models \
Views -> Contains all the EJS templates

public -> This folder contains all the files which will be used in the client side of the application \
public/images -> Contains all the images \
public/css -> Contains all the CSS files \
public/js -> Conatins all the Client side js files

routes -> Folder for handling different routes , contains all related routes in one file \
For example all the /tours routing code in one tourRouter file

## Common Questions

1. Difference between Client Side JS and Server Side JS

- Server Side JS \
  Handles backend logic, database interactions, authentication, etc. \
  Fetching data from a database, processing requests \
  Cannot Manipulate DOM

- Client Side JS \
  Handles UI interactions, DOM manipulation, animations, etc. \
  Validating form inputs, updating page content dynamically \
  Can manipulate the DOM

1.  Database Integration with MongoDB
    Current State: The project uses SQLite (better-sqlite3) for user data storage.
    Action Items:
    Replace SQLite with MongoDB for user data storage.
    Update the usersModel.js file to use Mongoose for database operations.
    Define Mongoose schemas and models for users and other entities (e.g., hotels, trips).
    Update all database-related functions (insertUser, getAllUsers, etc.) to use Mongoose queries.
2.  Authentication and Authorization
    Current State: Basic session management is implemented using express-session.
    Action Items:
    Implement secure password hashing using libraries like bcrypt.
    Add middleware to protect routes (e.g., user dashboard, admin dashboard).
    Implement role-based access control (e.g., restrict admin routes to admin users).
    Add JWT-based authentication for APIs if needed.
3.  Frontend Integration
    Current State: The project uses EJS for server-side rendering and serves static HTML files.
    Action Items:
    Create dynamic EJS templates for all views (e.g., sign-up, sign-in, dashboards).
    Add client-side validation for forms (e.g., sign-up, sign-in).
    Optionally, integrate a frontend framework like React or Angular for a more modern UI.
4.  API Development
    Current State: Some routes are defined (e.g., /signUp, /signIn, /logout).
    Action Items:
    Create RESTful APIs for CRUD operations (e.g., managing users, hotels, trips).
    Implement proper error handling and response formatting for APIs.
    Add API documentation using tools like Swagger or Postman.
5.  Hotel and Trip Management
    Current State: Basic hotel data is hardcoded in hotelsRouter.js.
    Action Items:
    Create MongoDB collections for hotels and trips.
    Implement routes and controllers for managing hotels and trips (e.g., add, update, delete).
    Add search and filter functionality for hotels and trips.
6.  Admin Panel
    Current State: Admin dashboard routes are defined but lack functionality.
    Action Items:
    Add features for managing users, hotels, and trips in the admin panel.
    Implement analytics and reporting features (e.g., user statistics, booking trends).
