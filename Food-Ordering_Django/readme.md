
Project Setup Guide

# Step 1: Create a Virtual Environment
-------------------------------------

Navigate to your project directory (or create one if you haven't already):

CMD--->`cd  food)ordering_django`


To create a virtual environment, run the following command:

For Windows:

CMD--->`python -m venv venv`

For macOS/Linux:

CMD--->`python3 -m venv venv`

# Step 2: Activate the Virtual Environment
---------------------------------------

After creating the virtual environment, activate it by running the appropriate command:

For Windows:

CMD--->`.\venv\Scripts\activate`

For macOS/Linux:

CMD--->`source venv/bin/activate`

# Step 3: Install Project Requirements
------------------------------------

Once the virtual environment is activated, you need to install the required dependencies.

> 3.1 Create a requirements.txt File (If Not Already Created)

If a requirements.txt file does not already exist in your project, you can create it manually or generate it by adding the necessary libraries.

Example of a basic requirement. txt file:

```python required libraries like
Django==2.2.7
django-tinymce4-lite==1.7.5
jsmin==3.0.0
pytz==2019.3
sqlparse==0.3.0

```

3.2 Install Dependencies

Once the requirements.txt file is ready, run the following command to install the dependencies:

CMD--->`pip install -r requirements.txt`

# Step 4: Run Django Project
----------------------------

4.1 Apply Migrations

Before running the server, apply any database migrations:

CMD--->`python manage.py migrate`

4.2 Create a Superuser (Optional)

To access the Django admin interface, create a superuser account:

CMD--->`python manage.py createsuperuser`

Enter the required details when prompted.

4.3 Run the Development Server

Start the Django development server:

RUN--->`python manage.py runserver`

Access the application at:

http://127.0.0.1:8000

# Step 5: (Optional)  without venv referring Use Docker for Project Setup
-----------------------------------------------------------------------
To using Docker without an .env file. You can achieve this by directly passing environment variables through the Docker CLI or defining them in your Dockerfile

Docker for Windows: https://www.docker.com/products/docker-desktop

Docker for macOS: https://www.docker.com/products/docker-desktop

Docker for Linux: https://docs.docker.com/get-docker
docker --version

