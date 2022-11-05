# ALTSCHOOL-BACKEND-Python-SECOND-SEMESTER-EXAMINATION-PROJECT.
## CONTENT
### Title
### Introduction 
### Project Environment
### Installation
### Folder Creation
### File Creation
### Templates Folder
### Static Folder
### Project Webpages
### Authentication
### Authorization
### Profile
### Database
### What i learned
### Challenges
### Conclusion

# TITLE:
## ALTSCHOOL AFRICA SCHOOL OF ENGINEERING BACKEND (Python) SECOND SEMESTER EXAMINATION PROJECT.

# INTRODUCTION :
This project is for AltSchool Africa school of engineering backend (Python) track students for our second Semester Examination. This project is a "Blogging App" website with many functions.
This project " SIRMUSO BLOG WEBSITE" allows anyone visiting the site to be able to view all blog posts but only restricted to some web pages when not signed in and will be able to view all web pages when signed in except the admin page.
The homepage which is the landing page of the website contains all the lists of articles written by different authors. The website contains many web pages, user authentication, and authorization with a well-structured database that is used in storing all users' information and posts.

# BUILT WITH:
<p align="left"> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a>
<a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/></a>
<a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> 
<a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>
<a href="https://flask.palletsprojects.com/" target="_blank" rel="noreferrer"> <br> <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-icon.svg"  alt="flask" width="40" height="40"/></a> </p>

# PROJECT ENVIRONMENT: 
This project requires a virtual environment for the proper functioning of the project. This section gives a short demonstration of how to create a virtual environment(windows users) which is as follows:
## Step 1:
Open your system command prompt from your window search bar "search command prompt".

## Step 2 :
Make a directory to your desktop or any preferable location.
### Command: cd Desktop
## Step 3:
Install virtual environment if not installed before.
### Command: pip install virtual environment
## Step 4:
Create your flask environment with any name you want. (i will be using flaskenv for demonstration)
### Command: virtualenv flaskenv
## Step 5:
Make a directory to your environment
### Command: cd flaskenv
## Step 6:
Make a directory to scripts
### Command: cd scripts
## Step 7:
Activate your environment
### Command: activate
Yes, your environment is ready for use.
### Note: The above illustrations are for windows users only.

# INSTALLATION:
This section contains all the packages to be installed for this project.
Before installation make sure your environment is activated and packages are installed in the terminal( e.g command prompt, PowerShell, Git Bash, etc) using  "pip install package".
## Packages to be installed:
### flask
### flask-login
### flask-sqlalchemy
### flask-mail

### The command for installation:
pip install " package name"

# FOLDER CREATION:
This section contains all the folders required for the creation of this project.
## BlogPost Folder:
This folder contains all the files and folders in this project except the app.py file and the requirements.txt file.
## Templates Folder:
This contains all the HTML files needed for this project.
## Static Folder:
This contains the uploads folder and CSS file need to for this project. 

# FILE CREATION
This section contains all the files needed for the creation of this project which is:

## app.py
This file is the engine of the project which is used for running the project. It is created outside the BlogPost folder.

## __init__.py
This file contains all the registration required for this project. It's used to return app, register auth, and main file.
## main.py
This file contains all the BlogPost routes needed for this project posts such as creating a post, updating the post, deleting the post, and getting the post by (id, title, author).
## auth.py
This file contains all the user authentication routes required for this project such as user registration, user login, user logout, contact page, etc.
## models.py
This file contains the User table,Image table and the BlogPost table which is used in the creation of the project database.
## The User table contains:
### Id
### Email
### Username
### Password
### Last name
### First name
### Created date

## The BlogPost table contains:
### Id
### Title
### Content
### Author
### poster_id
### Posted date
## Image table
### Id
### Name
### Mimetype

# TEMPLATE FOLDER

The templates folder contains all the HTML files needed for this project which include:
### base.html
### home.html
### contact.html
### login.html
### register.html
### edit.html
### new_post.html
### content.html
### dashboard.html
### search.html
### admin.html
### profile_update.html

# STATIC FOLDER

The static folder contains the uploads folder and the CSS file needed for this project which includes:
### Upload folder
### main.css


# PROJECT WEB PAGES:
This section contains all the pages present on the website which is as follows:

## Home Page
The homepage is also the landing page which contains all the blog articles written by different authors and also contains the new post button, edit button, and delete button which are only visible to the logged-in users.

## About Page
This page contains all the information about the website project and also some information about the website creator.

## Contact Page 
This page contains a form that will be used to contact the website Creator for any information.
## The form inputs contain:
### Username
### Email
### Phone number
### Message

## Register page 
This page contains all the information needed for a user to get registered.
## The form inputs include:
### Email
### Username
### Password
### Confirm password
### Last name
### First name
### Phone no

## Login page
The page contains all the information needed for a user to get logged in to the website.
## The form inputs include:
### Email
### Password
### With a remember me function.

## New post page
This is the website posts creation page which contains all the information needed to create and publish an article to the home page.
## The form inputs include:
### Title
### Content
### Author

## Edit page
This page is used for updating articles by clicking the edit button from the homepage but only the logged-in users can see and use the button and it is only the user author that can edit or delete his/her posts.

## Admin Page
This page is only for the admin of the website he/she is the only one authorized to view this page and it contains all user's information.
## Dashboard page 
This page contains the user's personal information that can only be accessed by the user. Individual user are only accessed to view only their dashboard.
 
# AUTHENTICATION
These are the rules which all users must abide by in the course of creating their accounts.
## These rules are as follows:
The username must not be less than 7 characters.
Password must not be less than 8 characters.
Password must equal to confirm password 
Email must be unique
The username must be unique
Only registered users are allowed to log in.
The users must log in with their correct email and password etc.
Only user of a post can edit and delete their post

Only user with id 1 which is regarded as the admin is authorized to view the admin page.


# AUTHORIZATION
The Flask_login package is used for the authorization process for this project and the authorization rules are as follows:
## Non-signed-in users can only view:  
### Homepage (but cannot view the new post, edit and delete button)
### Contact Page
### Abort page
### Register page 
### Login page

## While logged in users can view all the web pages except the admin page if not the admin.

# PROFILE

User profile contains individual personal information with an upload input where users are allowed to upload their profile picture but user are only allowed to upload their picture once in other to avoid a mix up.
The users images are stored in the database and are been called using the user id and this image are also used for the user post picture.
 
# DATABASE
This is a well-structured database that is used for storing all the user's information and all information can be accessed and retrieved by the admin.
## The database contain three tables which are:
### Users table
### Blogposts table and
### Images table

# What I learned 
### Uploading an image to the database
### Displaying an image from the database
### Sending mail through flask-mail


# THE Challenges’
Getting  posts by its title irrespective of how the title is written
Getting post by author name
Getting a specific post by its title and author name
Getting forgot password token
Resetting lost password
Using uuid for my database
Screen responsiveness (not mobile friendly)


# CONCLUSION
This blog application project " SIRMUSO BLOG WEBSITE" is an AltSchool python backend second-semester examination project which was built to suit the exam instructions.
This project is fully created both frontend and backend by ADEYEMO MUSODIQ OLALEKAN an AltSchool Africa School of Engineering student.
This project is open for contribution.

<h1 align="left" font-weight="bold">Connect with me:</h1>
<p align="left">
<a href="https://twitter.com/sirmuso" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="sirmuso" height="30" width="40" /></a>
<a href="https://linkedin.com/in/musodiq-adeyemo" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="musodiq-adeyemo" height="30" width="40" /></a>
<a href="https://fb.com/https://www.facebook.com/adeyemo.musodiq" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="https://www.facebook.com/adeyemo.musodiq" height="30" width="40" /></a>
</p>

- 📫 How to reach me **adeyemomusodiq@gmail.com**

- ⚡ Fun fact **I'm currently studying at AltSchool Africa School of Software Engineering Class of 2022.**


You can contact me on WhatsApp at 08141171294

## GOD BLESS ALT SCHOOL  AFRICA






