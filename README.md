# AI Blog Generator with Backend using Python Django and PostgreSQL

Initial release date: 19 July 2020

## Description
AI blog generator tool, generate YouTube link to an article blog. It's using Python Django framework for backend and admin content management, along with PostgreSQL databases and Tailwind CSS.

## Step by Step

1. Create a virtual environment in the root directory: `python -m venv $ENV_NAME`
2. Activate the virtual environment: ` source $ENV_NAME/bin/activate` (for MacOS, Unix, or Linux users) or ` .\ENV_NAME\Scripts\activate` (for Windows users)
3. Install requirements: `pip install -r requirements.txt`
4. Create Django on gen_ai_blog folder: `django-admin startproject gen_ai_blog`
5. Jump in the gen_ai_blog folder: `cd gen_ai_blog`
6. Create Django app folder: `python3 manage.py startapp blog_generator`
