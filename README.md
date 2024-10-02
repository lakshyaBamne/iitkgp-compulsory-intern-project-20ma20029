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
