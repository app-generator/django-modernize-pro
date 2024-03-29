# [Django Modernize PRO](https://appseed.us/product/modernize-dashboard-pro/django/)

**Django Dashboard** crafted by `AppSeed` on top of a modern design. **[Modernize PRO](https://appseed.us/product/modernize-dashboard-pro/django/)** is a premium `Bootstrap 5` designed by `AdminMart` that comes with feature-rich pages and developer-centric code components. This design provides many prebuilt admin layouts which give you the best selection choice for a modern dashboard.

- 👉 [Modernize PRO Django](https://appseed.us/product/datta-able-pro/django/) - `product page`
- 👉 [Modernize PRO Django](https://django-modernize-pro.onrender.com) - `LIVE Demo`

<br />

## Features

- `Up-to-date dependencies`
- Database: `SQLite`, PgSQL, MySql
- **Authentication**
  - `Session-Based authentication`
  - `Social Login`: **Github** & **Google**
- **User Extended profile**
- **API** via DRF
- DataTables
- Charts
- Celery
- File Manager
- i18n (internationalization) 
- `Docker`

![Modernize PRO - Thumb Image](https://github.com/app-generator/dummy/assets/51070104/6b1d21c2-5e26-4708-bcc5-7958e7f49d3d)

<br />

## Start in `Docker`

> **Step 1** - Download the [code](https://appseed.us/product/modernize-dashboard-pro/django/) and unzip the sources (requires a `purchase`). 

```bash
$ unzip django-modernize-pro.zip
$ cd django-modernize-pro
```

<br />

> **Step 2** - Start the APP in `Docker`

```bash
# Optional (kill all existing containers)
$ docker container kill $(docker ps -q) ; docker container rm $(docker ps -a -q) ; docker network prune -f 
# Start the APP
$ docker-compose up --build 
```

Visit `http://localhost:5085` in your browser. The app should be up & running.

<br />

## Create new `.env` from `env.sample`

The meaning of each variable can be found below: 

- `DEBUG`: if `True` the app runs in develoment mode
  - For production value `False` should be used
- `MYSQL` credentials 
  - `DB_ENGINE`, default value = `mysql`
  - `DB_NAME`, default value = `appseed_db`
  - `DB_HOST`, default value = `localhost`
  - `DB_PORT`, default value = `3306`
  - `DB_USERNAME`, default value = `appseed_db_usr`
  - `DB_PASS`, default value = `pass`
- `OAuth` via Github
  - `GITHUB_ID`=<GITHUB_ID_HERE>
  - `GITHUB_SECRET`=<GITHUB_SECRET_HERE> 
- `OAuth` via Google
  - `GOOGLE_CLIENT_ID`=<GOOGLE_ID_HERE>
  - `GOOGLE_SECRET_KEY`=<GOOGLE_SECRET_HERE> 

<br />

## Manual Build

> **Step 1** - Download the [code](https://appseed.us/product/modernize-dashboard-pro/django/) and unzip the sources (requires a `purchase`). 

```bash
$ unzip django-modernize-pro.zip
$ cd django-modernize-pro
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Create Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:8000/register/`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:8000/login/`

<br />

## Enable Social Login 

> 👉 **Github Setup** - [Create an OAuth App](https://docs.github.com/en/developers/apps/building-oauth-apps/creating-an-oauth-app)

- SignIN to `Github`
- Access `Settings` -> `Developer Settings` -> `OAuth Apps`
- Edit your OAuth App
  - `App Name`
  - `App Description`
  - (mandatory) `HomePage`: `https://localhost:8000`
  - (mandatory) `Authorization callback URL`: `https://localhost:8000/`
  - Generate a new `secret key`

<br />

## Codebase

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/              # Implements app configuration
   |    |-- settings.py   # Defines Global Settings
   |    |-- wsgi.py       # Start the app in production
   |    |-- urls.py       # Define URLs served by all apps/nodes
   |
   |-- home/              # Serves all pages from the UI Kit  
   |
   |-- apps/
   |    |
   |    |-- common/       # Assets used by all APPS (models, helpers)
   |    |-- users/        # Handles Auth Flow
   |    |-- api/          # DRF API
   |    |-- charts/       # Charts APP
   |    |-- tables/       # DataTables APP
   |    |-- tasks/        # Celery App
   |
   |-- templates/         # Pages & Templates   
   |-- assets/            # Static Assets [ JS, CSS, images ]   
   |
   |-- requirements.txt   # Development modules - SQLite storage
   |
   |-- .env               # Environment
   |-- env.sample         # Environment Sample
   |
   |-- manage.py          # Django Manager File
   |
   |-- ************************************************************************
```

<br />

---
[Django Modernize PRO](https://appseed.us/product/modernize-dashboard-pro/django/) - Starter crafted by **[AppSeed](https://appseed.us/)**.
