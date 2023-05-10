# [Django Modernize PRO](https://github.com/app-generator/django-modernize-pro)

**Django Dashboard** crafted by `AppSeed` on top of a modern design. **Modernize PRO** is a premium `Bootstrap 5` designed by [AdminMart](https://adminmart.com/?ref=1) that comes with feature-rich pages and developer-centric code components. This design provides many prebuilt admin layouts which give you the best selection choice for a modern dashboard.

> **NOTE**: This product `requires a License` in order to access the theme. During the purchase, a `GitHub Access TOKEN` is provided. 

- 👉 [Django Modernize PRO](#) - `Product page` (soon)
- 👉 [Django Modernize PRO](https://django-modernize-pro.onrender.com/) - `LIVE Demo`

<br />

> Features: 

- ✅ `Up-to-date Dependencies`
- ✅ Theme: [Django Admin Modernize](https://github.com/app-generator/django-admin-modernize-pro), **designed by [AdminMart](https://adminmart.com/?ref=1)**
  - `can be used in any Django project` (new or legacy)
- ✅ **Authentication**: `Django.contrib.AUTH`, Registration
- 🚀 `Deployment` 
  - `CI/CD` flow via `Render`

<br />

![Modernize PRO - Thumb Image](https://github.com/app-generator/dummy/assets/51070104/6b1d21c2-5e26-4708-bcc5-7958e7f49d3d)

<br />

## Manual Build 

> 👉 Download the code  

```bash
$ git clone https://github.com/app-generator/django-modernize-pro.git
$ cd django-modernize-pro
```

<br />

> 👉 Export `GITHUB_TOKEN` in the environment. The value is `provided during purchase`. 

This is required because the project has a private REPO dependency: `github.com/app-generator/priv-django-admin-modernize-pro`

```bash
$ export GITHUB_TOKEN='TOKEN_HERE'  # for Linux, Mac
$ set GITHUB_TOKEN='TOKEN_HERE'     # Windows CMD
$ $env:GITHUB_TOKEN = 'TOKEN_HERE'  # Windows powerShell 
```

<br />

> 👉 Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

<br />

> 👉 Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> 👉 Create the Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> 👉 Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## Codebase structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                            
   |    |-- settings.py                  # Project Configuration  
   |    |-- urls.py                      # Project Routing
   |
   |-- home/
   |    |-- views.py                     # APP Views 
   |    |-- urls.py                      # APP Routing
   |    |-- models.py                    # APP Models 
   |    |-- tests.py                     # Tests  
   |    |-- templates/                   # Theme Customisation 
   |         |-- includes                # 
   |              |-- custom-footer.py   # Custom Footer      
   |     
   |-- requirements.txt                  # Project Dependencies
   |
   |-- env.sample                        # ENV Configuration (default values)
   |-- manage.py                         # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

## Deploy on [Render](https://render.com/)

- Create a Blueprint instance
  - Go to https://dashboard.render.com/blueprints this link.
- Click `New Blueprint Instance` button.
- Connect your `repo` which you want to deploy.
- Fill the `Service Group Name` and click on `Update Existing Resources` button.
- After that your deployment will start automatically.

At this point, the product should be LIVE.

<br />

---
[Django Modernize PRO](https://github.com/app-generator/django-modernize-pro) - Minimal **Django** core provided by **[AppSeed](https://appseed.us/)**
