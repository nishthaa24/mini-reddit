# Mini Reddit
This web application can be accessed at [Mini Reddit](https://miniredditapp.pythonanywhere.com/)


Mini Reddit is a web application developed using the Django Python framework that utilizes SQLite3 for database management. The project aims to create a simplified version of the popular Reddit app, where users can share and engage with content through voting and commenting. The application was hosted on PythonAnywhere, providing users with easy access to its features.

## Features
* **Subreddit :** Create, update, and delete subreddits.

  
* **Posts :** Submit posts with titles, links, and text descriptions. Upvote or downvote posts. View the number of comments on each post.
* **Comments :** Users can comment on posts, and comments can be replies to other comments. Upvote or downvote comments.
* **Votes :** Two types of votes: upvotes and downvotes for both posts and comments.
* **Search :** Utilize the search bar to filter posts.
* **Signup/Login/Logout :** Users can create accounts, log in, and log out.
* **CSRF Protection :** The application is equipped with Cross-Site Request Forgery (CSRF) protection which is implemented using Django's built-in CSRF middleware. This protects the application from potential malicious attacks by verifying the validity of CSRF tokens in requests.
## Backend Techstack
* **Django :** A robust and feature-rich framework for backend development.


* **SQLite3 :** Lightweight and serverless database for initial development.
* **PythonAnywhere :** Platform-as-a-Service (PaaS) used for hosting and deployment.

## Frontend Techstack
* **CSS & Bootstrap :** A frontend framework for a visually appealing and responsive design.


* **Crispy Forms :** A Django package to style login and signup forms using Bootstrap classes.
* **Django Template Language :**  Crispy Forms and CSS Bootstrap were seamlessly integrated within the Django templating language, resulting in a polished and user-friendly interface for user entry points.

## Integrating Crispy Forms
Integrating Crispy Forms into the project is straightforward :-

* Install the Crispy Forms package using pip and add it to the INSTALLED_APPS in the Django settings.

  
* Use {% load crispy_forms_tags %} template tag to load Crispy Forms tags in form templates.
* Apply the |crispy filter on form instances in templates to render forms with the specified layout.

## Deployment on PythonAnywhere
Deploying the application on PythonAnywhere involves the following steps :-

* Clone the repository.

<div >

```python
git clone https://github.com/yourusername/mini-reddit.git
```
</div>

* Set up a virtual environment and install Django and other requirements.

<div >
  
```python
mkvirtualenv --python=/usr/bin/python3.7 mysite-virtualenv
pip install -r requirements.txt
```
</div>

* Make manage.py executable.
<div >
  
```python
chmod +x manage.py
```
</div>

* Create a web app using manual configuration and specify the project folder, virtual environment, and WSGI file.

* Configure static files to serve CSS, JavaScript, and images.
<div >
  
```python
./manage.py migrate
```
</div>

* Create an admin profile using python manage.py createsuperuser.
<div >
  
```python
python manage.py createsuperuser
```
</div>
