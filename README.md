# Bank security console
This is internal repository for employees of bank "Shining". If you came here accidently then you can't run it, because of not having database access info. But you can use layout code or check database queries.

Security console is a site, which can be connected to remote database with visits and passcards of our bank employees.

### How to install
Python3 should be already installed. Then use pip (or pip3, if there is a conflict with Python2) to install dependencies:
```
pip install -r requirements.txt
```
Some settings need to be set in `.env` file of the root of this project
```
DATABASE_URL=ENGINE://USER:PASSWORD@HOST:PORT/BASENAME

# The key to securing signed data
SECRET_KEY="REPLACE_ME"

# Show or not debug information, default False, not to show
DEBUG=False

# If you run server in different time zone, default Europe/Moscow
TIME_ZONE="Europe/Moscow"
```
### Usage
Run server at localhost by following command:
```
$ python manage.py runserver 0.0.0.0:8000
```
### Project Goals
The code is written for educational purposes on online-course for web-developers dvmn.org.