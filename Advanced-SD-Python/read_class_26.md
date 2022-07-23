# Read: Class 26

## Definition

Django is an open-source Python-based web framework that follows a model-template–views pattern.

## Intro to Django

### Object-relational mapper:

Django allows users to define their data models entirely in Python, also it provides them with free access to a rich, dynamic database-access API, while also allowing SQL if needed.

### URLs and views:

Django allows users to create clean, elegant URL schemes, and doesn’t put any cruft in their URLs.

In order to create URLs for an application using Django, the user should create a Python module called `URLconf.` as a table of content for the application, which contains simple mapping between URL patterns and views.

### Templates:

Django's offers a template language that is comfortable and easy to learn especially to users that are used to working with HTML and front-end design.

ex: ([source](https://www.djangoproject.com/start/))

    <html>
    <head>
        <title>Band Listing</title>
    </head>
    <body>
        <h1>All Bands</h1>
        <ul>
        {% for band in bands %}
        <li>
            <h2><a href="{{ band.get_absolute_url }}">{{ band.name }}</a></h2>
            {% if band.can_rock %}<p>This band can rock!</p>{% endif %}
        </li>
        {% endfor %}
        </ul>
    </body>
    </html>

### Forms:

Django provides users with a powerful form library for rendering just like HTML, by converting user-submitted data to native Python types.

### Authentication:

Django provides users with a full-featured, secure authentication system, that handles user accounts, groups, premissons and even cookie-based user sessions.

### Admin:

Django provides users with an automatic admin interface, that reads metadata, and also provides a powerful interface to manage content on the site.

### Security:

Django provides users full sprotection against:
- **Cross site scripting** 
- **Clickjacking**
- **SQL injection**
- **Remote code execution**
- **Cross site request forgery - CSRF**

## Things I want to know more about

- None.
