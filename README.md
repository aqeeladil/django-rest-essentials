# Django-Rest-Framework


```bash
python -m venv myenv
source myenv/Scripts/activate
pip install -r requirements.txt # OR (pip install django djangorestframework django-extensions pillow django-silk djangorestframework-simplejwt)
pip freeze > requirements.txt 
django-admin startproject core .
python manage.py startapp api

python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

# management/commands/populate_db.py
# Apply the below command after creating the models in api/models.py to populate the database with default values
python manage.py populate_db
```

```bash
# Optional

# Django Graph Models command - Generate ER Diagrams for your Database
# pip install django-extensions
python manage.py graph_models api > models.dot      
# will generate the ER code for the api app
# now copy the code from models.dot and generate ER diagram by visiting the GraphvizOnline website.   
```

```bash
python manage.py runserver

# Django Silk is a powerful profiling and debugging tool for Django applications. It helps analyze database queries, response times, and code execution performance.
# Django Silk is not recommended in production due to performance overhead.
# pip install django-silk

python manage.py test

# REST Client (vs-code extension for sending http requests
# REST Client allows you to send HTTP request and view the response in Visual Studio Code directly.
```



