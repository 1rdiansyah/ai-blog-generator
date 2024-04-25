# AI Blog Generator with Backend using Python Django and PostgreSQL

Initial release date: 24 April 2024

## Description
AI blog generator tool, generate YouTube link to an article blog. It's using Python Django framework for backend and admin content management, along with PostgreSQL databases and Tailwind CSS.

## Step by Step

1. Create a virtual environment in the root directory: `python -m venv $ENV_NAME`
2. Activate the virtual environment: ` source $ENV_NAME/bin/activate` (for MacOS, Unix, or Linux users) or ` .\ENV_NAME\Scripts\activate` (for Windows users)
3. Install requirements: `pip install -r requirements.txt`
4. Create Django on gen_ai_blog folder: `django-admin startproject gen_ai_blog`
5. Jump in the gen_ai_blog folder: `cd gen_ai_blog`
6. Create Django app folder: `python3 manage.py startapp blog_generator`
7. Open your gen_ai_blog/setting.py, make sure you adding the 'blog_generator' on INSTALLED_APPS lists
8. Create urls.py on 'blog_generator' folders or you can just copy it from [blog_generator/urls.py](https://github.com/1rdiansyah/ai-blog-generator-from-youtube-link/blob/main/blog_generator/urls.py)
9. Open your gen_ai_blog/setting.py, make sure you adding the 'DIRS': [BASE_DIR, 'templates'] on TEMPLATES lists
10. Copy all of html templates on [templates](https://github.com/1rdiansyah/ai-blog-generator-from-youtube-link/tree/237e62c5ab0ae187d9722588509257cb0cc841f0/templates) to your templates folder
11. Setup your PostgreSQL databases, add the credential to the gen_ai_blog/setting.py, specifically on the DATABASES line
12. After you add the credential, you need to run `python3 manage.py makemigrations` and then run `python3 manage.py migrate` on the terminal
13. To accessing the Django admin you need to create superuser with `python3 manage.py createsuperuser`, then add your username, email, and password
14. Setup your views.py or you can just copy it from [blog_generator/views.py](https://github.com/1rdiansyah/ai-blog-generator-from-youtube-link/blob/main/blog_generator/views.py)
15. To get/download the Youtube Audio (only) and Title you need to install and import pytube : `pip3 install pytube`
16. Transcribe the audio to text with [AssemblyAI](https://www.assemblyai.com/), signup and create and copy API Token to [blog_generator/views.py](https://github.com/1rdiansyah/ai-blog-generator-from-youtube-link/blob/main/blog_generator/views.py)
