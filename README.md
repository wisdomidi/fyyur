Fyyur - iperform
Introduction
Fyyur is a musical venue and artist booking site that facilitates the discovery and bookings of shows between local performing artists and venues. This site lets you list new artists and venues, discover them, and list shows with artists as a venue owner.

## Tech Stack - 

- SQLAlchemy ORM ORM library
- PostgreSQL database
- Python3 and Flask server language and server framework, respectively 
- Flask-Migrate for creating and running schema migrations
- HTML, CSS, and Javascript with Bootstrap 3 for the front end

### Main Files: Project Structure
```
-├── README.md
-├── app.py *** the main driver of the app. 
-├── models.py *** SQLAlchemy database models.
-├── config.py *** Database URLs, CSRF generation, etc
-├── error.log
-├── forms.py *** Your forms
-├── requirements.txt *** The dependencies we need to install with "pip3 install -r requirements.txt"
-├── static
-│   ├── css 
-│   ├── font
-│   ├── ico
-│   ├── img
-│   └── js
-└── templates
-    ├── errors
-    ├── forms
-    ├── layouts
-    └── pages
```
 ### Overall:

Models are located in the MODELS models.py.
Controllers are also located in app.py.
The web frontend is located in templates/, which builds static assets deployed to the web server at static/.
Web forms for creating data are located in form.py

#### Highlight folders:

templates/pages -- Defines the pages that are rendered to the site. These templates render views based on data passed into the template’s view, in the controllers defined in app.py. These pages successfully represent the data to the user, and are already defined for you.

templates/layouts -- Defines the layout that a page can be contained in to define footer and header code for a given page.

templates/forms -- Defines the forms used to create new artists, shows, and venues.
app.py -- Defines routes that match the user’s URL, and controllers which handle data and renders views to the user. This is to connect to and manipulate the database and render views with data to the user, based on the URL.

Models in models.py -- Defines the data models that set up the database tables.
config.py -- Stores configuration variables and instructions, separate from the main application code. This is to connect to the database.

### Development Setup

> First, install Flask if you haven't already.

```

$ cd ~
$ sudo pip3 install Flask
To start and run the local development server,

```

### Install the dependencies:
```

$ pip install -r requirements.txt

> Run the development server:

$ FLASK_APP=app.py FLASK_DEBUG=true flask run
```
Navigate to Home page http://localhost:5000


Starter code is from Udacity full stack nano degree program

iperform