# Store Rating Web Application

This web application allows users to rate stores registered on the platform. It features a role-based access control system, offering different functionalities to System Administrators, Normal Users, and Store Owners.

## Tech Stack

-   **Backend:** Express.js (Node.js framework) with MVC architecture
-   **Database:** SQL (e.g., PostgreSQL or MySQL)
-   **Frontend:** React.js (using JSX), Axios for API calls, Context API for state management, Vite as the build tool, and Tailwind CSS v4 for styling.

## Features

-   **User Management:**
    -   System Administrators can add, view, and filter users (Normal Users and Admin Users).
    -   Normal Users can sign up, log in, and update their passwords.
-   **Store Management:**
    -   System Administrators can add and view stores.
    -   Normal Users can view and search for stores.
-   **Rating System:**
    -   Normal Users can submit and modify ratings for stores (1 to 5 stars).
    -   Store Owners can view ratings submitted for their stores and see the average rating.
-   **Role-Based Access Control:**
    -   Different user roles (System Administrator, Normal User, Store Owner) have access to different functionalities.
-   **Dashboard:**
    -   System Administrators have access to a dashboard displaying total users, stores, and submitted ratings.
    -   Store Owners have a dashboard to view user ratings and the average store rating.
-   **Form Validations:** Input fields are validated according to the specified rules.
-   **Sorting:** Listings support ascending/descending sorting for key fields.

## User Roles

1.  **System Administrator:**

    -   Manages users and stores.
    -   Has access to a comprehensive dashboard.
    -   Can add new users with Name, Email, Password, and Address.
    -   Can view a list of stores with Name, Email, Address, and Rating.
    -   Can view a list of normal and admin users with Name, Email, Address, and Role.
    -   Can apply filters on all listings based on Name, Email, Address, and Role.
    -   Can view details of all users (including Rating if the user is a Store Owner).
    -   Can log out.

  
2.  **Normal User:**

    -   Can sign up with Name, Email, Address, and Password.
    -   Can log in.
    -   Can update their password.
    -   Can view a list of all registered stores (displaying Store Name, Address, Overall Rating, User's Submitted Rating, and options to submit/modify ratings).
    -   Can search for stores by Name and Address.
    -   Can submit ratings (1-5) for individual stores.
    -   Can modify their submitted rating.
    -   Can log out.

   
4.  **Store Owner:**

    -   Can log in.
    -   Can update their password.
    -   Has a dashboard to view a list of users who have submitted ratings for their store.
    -   Can see the average rating of their store.
    -   Can log out.

   

## Functionalities

### System Administrator

-   **Add New Store:** Functionality to register a new store on the platform.
-   **Add New User:** Functionality to create new Normal User and Admin User accounts.
-   **Dashboard:** Displays key metrics: total users, total stores, and total submitted ratings.
-   **View Stores:** Lists all registered stores with details and overall rating.
-   **View Users:** Lists all normal and admin users with their details and roles.
-   **Apply Filters:** Allows filtering of store and user listings based on various criteria.
-   **View User Details:** Shows complete information for individual users.

![WhatsApp Image 2025-06-13 at 15 56 36_58782617](https://github.com/user-attachments/assets/5ddf8aa0-43fd-42ff-ba21-c54b405d09cc)


### Normal User

-   **Signup:** Registration form for new users.
-   **Login:** Authentication for existing users.
-   **Update Password:** Option to change their password after logging in.
-   **View Stores:** Displays a list of all registered stores with relevant information.
-   **Search Stores:** Allows searching for stores by name and address.
-   **Submit Rating:** Enables users to rate a store.
-   **Modify Rating:** Allows users to change their previously submitted rating for a store.

### Store Owner

-   **Login:** Authentication for store owner accounts.
-   **Update Password:** Option to change their password after logging in.
-   **Dashboard:** Displays users who rated their store and the average rating.

## Form Validations

-   **Name:** Minimum 20 characters, maximum 60 characters.
-   **Address:** Maximum 400 characters.
-   **Password:** 8-16 characters, must include at least one uppercase letter and one special character.
-   **Email:** Must follow standard email validation rules.

## Additional Notes

-   All relevant tables in the SQL database should support sorting (ascending/descending) for key fields like Name and Email.
-   The project should adhere to best practices for both frontend (React, Context API, Tailwind) and backend (Express.js MVC, SQL) development.
-   The database schema should be well-designed and follow best practices for relational databases.
![admin-profile(2)](https://github.com/user-attachments/assets![admin-dashboard(1)](https://github.com/user-attachments/assets/69fa1741-a60b-4ed4-a90e-f13931d59eee)
/d90ce47a-1ef5-4a90-87df-3c738f6d0709)![Login](https://github.com/user-attachments/assets/9b57833d-61d7-4dd6-9a18-7d8a887fb827)![Register](https://github.com/user-attachments/assets/98bba977-cb55-444f-9bbc-55aa8ace1293)
![StoreDash](https://github.com/user-attachments/assets/48c1e195-c533-4623-9223-cfda0a7a7f04)
![StoreRatings](https://github.com/user-attachments/assets/43f468ce-bd69-47ed-88d9-e9c7e3a573c5)
![Users](https://github.com/user-attachments/assets/83ad29e3-a4cf-4fed-a27f-c824d8f91533)



**Important:** Please replace the placeholder image URLs (`[Insert Image URL Here]`) with the actual URLs of your images to visualize the application's features. You can use services like Imgur, Cloudinary, or any other image hosting platform to obtain these URLs.
