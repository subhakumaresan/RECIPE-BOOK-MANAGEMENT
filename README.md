# 🍲 Recipe Book Management System

A Python-based web application for storing, organizing, and managing personal recipes, built with *Streamlit* and *SQLite*.

## 📌 Overview

Managing recipes manually using notebooks or paper is time-consuming and prone to loss. This project solves that problem by providing a simple, digital recipe management system where users can securely log in, browse recipes by category, and (as an admin) add, update, or delete recipes — all backed by a persistent SQLite database.

## ✨ Features

- 🔐 *User Authentication* – secure login and registration with password hashing (SHA-256)
- 👤 *Role-Based Access* – separate views for *Admin* and *User*
- ➕ *Add Recipe* (Admin) – add new recipes with name, category, ingredients, instructions, cooking time, and servings
- 📖 *View Recipes* – browse all recipes or view full details of a selected recipe
- 🔍 *Browse by Category* – filter recipes by Breakfast, Lunch, Dinner, or Snacks
- ✏️ *Update Recipe* (Admin) – edit existing recipe details
- 🗑️ *Delete Recipe* (Admin) – remove unwanted recipes with confirmation
- 💾 *Persistent Storage* – all data is stored in a local SQLite database

## 🧠 Core Concepts Used

- Functions and modular programming
- Lists and dictionaries
- Conditional statements and loops
- File/database handling with sqlite3
- CRUD operations (Create, Read, Update, Delete)
- Exception handling
- Session state management in Streamlit

## 🗂️ Module Overview

| Module | Description |
|---|---|
| User Authentication | Handles login, registration, and password security |
| Add Recipe | Lets admins add new recipes with validation |
| View Recipe | Displays all stored recipes with full details |
| Search / Browse Recipe | Lets users browse recipes by category |
| Update Recipe | Allows admins to edit existing recipe data |
| Delete Recipe | Allows admins to remove recipes safely |
| Exit System | Safely closes database connections on exit |

## 🏗️ Architecture


Login / Register
      │
 ┌────┴────┐
 Admin      User
 │           │
 Add        Choose Recipes
 Manage     by Category
 View
 │           │
 └────┬─────┘
     Exit


## 🛠️ Tech Stack

- *Language:* Python 3.8+
- *Frontend:* Streamlit
- *Database:* SQLite (sqlite3)
- *Security:* hashlib for password hashing

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip

### Installation

bash
git clone <repository-url>
cd recipe-book-management
pip install streamlit


### Run the Application

bash
streamlit run recipe_book.py


The app will open automatically in your browser at http://localhost:8501.

### Default Admin Credentials

| Username | Password |
|---|---|
| admin | admin123 |

## 📸 Screenshots

The application includes:
- Login & Registration page
- Admin Panel (Add / Manage / View recipes)
- Category-wise recipe browsing for users
- Detailed recipe view with ingredients and instructions

## 📈 Future Enhancements

- Recipe images and video tutorials
- Nutritional information and calorie tracking
- Favorite recipes and recipe ratings
- Advanced search filters (cooking time, difficulty, diet type)
- Cloud deployment and mobile app version

## 📚 References

1. [Python Documentation](https://docs.python.org/)
2. [Streamlit Documentation](https://docs.streamlit.io/)
3. [SQLite Documentation](https://www.sqlite.org/docs.html)
4. [W3Schools Python Tutorial](https://www.w3schools.com/python/)
5. [GeeksforGeeks](https://www.geeksforgeeks.org/)
6. [TutorialsPoint](https://www.tutorialspoint.com/)

## 👥 Authors

- Subha Kumaresan
- Supriya S

*Guided by:* Mrs. P. Vanathi, M.E., (PhD), Assistant Professor/CSE
*Department:* Freshmen Engineering, M. Kumarasamy College of Engineering (Autonomous), Karur

## 📄 License

This project was developed for academic purposes as part of the *CGB1121 – Python Programming* course.
