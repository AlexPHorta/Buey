---
title: "Today I learned: Django"
date: 2023-04-19T23:57:20
draft: true
slug: today-i-learned-django
---

## Create a project

```
$ django-admin startproject name_of_the_project
```
## Create an app inside the project

```
$ python manage.py startapp name_of_the_app
```

Remember that a project can have many apps inside.

## Basic workflow

### Create a view

```
# <app>/views.py

from django.http import HttpResponse

def index(request):
    return HttpResponse("The view")
```

### Create the URLs

Wire the views in <app>/urls.py by creating (for example) path() calls;

```
# <app>/urls.py

from django.urls import path

from . import views


urlpatterns = [
    path("january", views.index)
]
```

Then, create the URL path in the project, for the _challenges_ subpath;

```
# <project>/urls.py

from django.contrib import admin
from django.urls import path, include


urlpatterns = [
    path("admin/", admin.site.urls),
    path("challenges/", include("challenges.urls"))
]
```
