# Wish Tree

[![Build Status](https://travis-ci.com/lucky-singh/wishtree.svg?branch=master)](https://travis-ci.org/lucky-singh/wishtree)

Wish Tree is a feature request app where a company can manage software feature requests for their clients and developers can make dreams come true.

### Installation

Clone and cd to the repository and run bash install.sh if you are on Ubuntu and navigate to http://0.0.0.0:5000/

Otherwise please follow step by step instruction.
1. Make sure you have python, pip, virtualenv and git installed
2. clone repository
3. cd to repository
4. Activate virtual environment
    ```sh
    virtualenv venv
    source venv/bin/activate
    ```
5. install requirements
    ```sh
    pip install -r requirements.txt
    ```
6. export environment variables
    ```sh
    export FLASK_APP=app.py
    export DATABASE_URL='sqlite:///wishtree.db'
    ```
7. initilize database
    ```sh
    python app.py
    ```
8. Start Flask application
    ```sh
    gunicorn -b 0.0.0.0:5000 app:app
    ```
9. navigate to http://0.0.0.0:5000/

Now Wish Tree should be appeared in the browser.