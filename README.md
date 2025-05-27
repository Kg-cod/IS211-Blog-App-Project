**Blog Application Project**

This is a Flask-based blog web application developed for the IS211 Course Project.  
It allows users to log in, create, edit, and delete blog posts.  
The project is fully built using Flask, Flask-Login, and Flask-SQLAlchemy.

**Features**
User login and logout system  
Dashboard displaying the user's posts  
Add, edit, and delete blog posts  
Posts displayed on the homepage in reverse chronological order  
SQLite database backend (`blog.db`)  
Clean and minimal HTML templates  
Organized folder structure with separation of concerns

**Project Structure**
app.py               
requirements.txt     
README.md        
templates (index.htm, login.html, dashboard.html, add.html, and edit.html)

**Database Model Details**
The application uses two main models:

1. **User**
'id' (Integer, Primary Key)  
'username' (String, unique)
'password' (String, plaintext for this assignment; note: in production, always hash passwords)

2.**Post**  
'id' (Integer, Primary Key)  
'title' (String)  
'content' (Text)  
'date_posted' (Datetime)  
'author_id' (Foreign Key to User)
