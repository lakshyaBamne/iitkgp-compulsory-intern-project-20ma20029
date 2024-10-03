# Grocery Store V-1.0

## Steps required to clone and run the web application

- Clone the github repository using the command

```
    git clone https://github.com/lakshyaBamne/iitkgp-compulsory-intern-project-20ma20029.git
```

- Make sure you have python installed on the machine
- Using *pip* you can downlaod the requirements for the project directly
- First create a virtual environment using *virtualenv*

```
    python -m venv venv
```

- Now activate the virtual environment (example is given using *gitbash*)

```
    source venv/Scripts/activate
```

- Now install the requirements

```
    pip install -r requirements.txt
```

- Now run the web application using either of the two commands

```
    flask run --debug
    python grocery_store.py
```

- The second command runs the web application on the current network as well to be accessed using other devices connected to the network

### How to make the admin after cloning the repository for the first time

- After cloning the repository and running the project for the first time, there are no elements in the database.
- We need to add an admin through the terminal so that that account can add products in the website for customers to see.
- the following commands are run in the python shell after activating the virtual environment

```
    from grocery_store import app
    from flaskr.extensions import db
    from flaskr.models import Admin
    app.app_context().push()
    adm = Admin(full_name="Lakshya Bamne", user_name="Admin_lakshyaBamne", email="lakshyabamne181@gmail.com", contact="7024837727",password_hash="pbkdf2:sha256:600000$fhPpUD5qCyMdNuW8$6e7016d6b4a697721287e6fc0206588d6b8349f568b847a28a736921583e0074")
    db.session.add(adm)
    db.session.commit()
```

- exit the python shell and run the application once again and then the admin can login with the details given in the query above
