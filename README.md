# Weather-App-Django
This repository implements a weather app that uses Open Weather API and Django as a backend framework![weather](https://user-images.githubusercontent.com/61186730/111905352-3597a400-8a71-11eb-9ca7-7511dec33ff0.JPG)
.
## Summary Workflow
The following is a basic workflow that you can use as a quick reference for developing a Django Project.

### Setup
1. Within a new directory, create and activate a virtualenv.
2. Install Django.
3. Create your project: <pre> django-admin.py startproject <name> </pre>
4. Create a new app:<pre> python manage.py startapp <appname> </pre>
5. Add your app to the INSTALLED_APPS tuple.


### Add Basic URLs and Views
1. Map your Project’s urls.py file to the new app.
2. In your App directory, create a urls.py file to define your App’s URLs.
3. Add views, associated with the URLs, in your App’s views.py; make sure they return a HttpResponse object. Depending on the situation, you may also need to query the model (database) to get the required data back requested by the end user.


### Templates and Static Files
1. Create a templates and static directory within your project root.
2. Update settings.py to include the paths to your templates.
3. Add a template (HTML file) to the templates directory. Within that file, you can include the static file with - <pre>{% load static %}</pre> and <pre> {% static "filename" %} </pre>. Also, you may need to pass in data requested by the user.
4. Update the views.py file as necessary.



