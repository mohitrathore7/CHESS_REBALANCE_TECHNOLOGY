Django Chess
Django Chess is a web-based chess game built using the Django framework. This project allows players to compete against each other in a classic game of chess directly in their browser.

Table of Contents
Features
Installation
Usage
Screenshots
Technologies Used
Contributing
License


Features
Player vs Player chess gameplay.
User authentication and profiles.
Real-time game updates using WebSockets.
Move validation and check/checkmate detection.
Persistent game state storage.
Responsive design for mobile and desktop use.
Installation
To get a local copy up and running, follow these simple steps:

Prerequisites
Python 3.x
Django 3.x
Docker (optional, for containerized setup)
Node.js (for front-end assets)
Clone the Repository
bash
Copy code
git clone https://github.com/rlichiere/django-chess.git
cd django-chess
Create a Virtual Environment
bash
Copy code
python3 -m venv venv
source venv/bin/activate
Install Dependencies
bash
Copy code
pip install -r requirements.txt
Set Up the Database
Apply the migrations to set up the database:

bash
Copy code
python manage.py migrate
Create a Superuser
Create an admin user to access the Django admin panel:

bash
Copy code
python manage.py createsuperuser
Collect Static Files
Collect all static files into a single directory:

bash
Copy code
python manage.py collectstatic
Run the Development Server
Start the Django development server:

bash
Copy code
python manage.py runserver
Open your browser and go to http://127.0.0.1:8000 to see the application running.

Usage
Playing a Game
Register or log in to your account.
Create a new game or join an existing one.
Start playing chess with another player in real-time.
Moves are validated and updates are reflected in real-time.
Admin Panel
Access the admin panel at http://127.0.0.1:8000/admin to manage users, games, and other administrative tasks.


Technologies Used

Backend: Django, Django Channels
Frontend: HTML, CSS, JavaScript
Database: SQLite (default, can be configured to use other databases)
WebSockets: Django Channels
Contributing
Contributions are welcome! Follow these steps to contribute:

Fork the repository.
Create your feature branch: git checkout -b feature/YourFeature
Commit your changes: git commit -m 'Add some feature'
Push to the branch: git push origin feature/YourFeature
Open a pull request.
