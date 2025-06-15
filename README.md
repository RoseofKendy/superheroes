# superheroesSuperheroes API

🔥 Description

This Flask API allows users to manage a list of superheroes, their superpowers, and the strength with which those powers are wielded. The app uses SQLAlchemy for database management and includes full CRUD routes, model validations, and nested JSON serialization.

🛠️ Technologies Used

Python 3.10+

Flask

Flask SQLAlchemy

Flask Migrate

SQLite

📦 Setup Instructions

Clone the Repository:

git clone <your_repo_url>
cd superheroes-api

Create Virtual Environment & Install Dependencies:

pipenv install
pipenv shell

Run Migrations:

flask db init
flask db migrate -m "Initial"
flask db upgrade

Seed the Database:

python seed.py

Start the Server:

flask run

🚀 API Endpoints

GET /heroes

Returns a list of all heroes.

GET /heroes/<id>

Returns details for a specific hero including their powers.

GET /powers

Returns a list of all powers.

GET /powers/<id>

Returns details for a specific power.

PATCH /powers/<id>

Updates the description of a power. Must be at least 20 characters.

POST /hero_powers

Creates a new HeroPower entry. Requires strength, hero_id, and power_id.

🧪 Sample JSON

POST /hero_powers

{
  "strength": "Average",
  "power_id": 1,
  "hero_id": 3
}

🧑 Author

Sharon Njue Kendi
sharon.njue@student.moringaschool.com