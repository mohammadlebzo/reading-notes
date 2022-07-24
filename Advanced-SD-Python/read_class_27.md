# Read: Class 27

## Django: Using models

### Definition:

**Models** in Django define the structure of stored data, meaning that its used to create tables, fields, and apply various constraints on them.

**Note**: models in Django are somewhat like SQL, meaning that structural database that uses relationships to connect data tables.

### Brief overview of how a model is defined:

Models are usually defined in an application's `models.py` file, as a subclass for `django.db.models.Model`.

An example on craeting a **field** that can be used for queries:

    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')

In the previous example the data type was a string od characters (`models.CharField`), followed by a couple of arguments.

#### Some common field arguments:

| Argument | Use |
|----------|-----|
| help_text | Text label for the HTML form |
| verbose_name | Human-readable name for the field used in field labels |
| default | Specifies the default value for the field |
| null | Stores `NULL` for the blank values if its `True` |
| blank | Allows for blank fields in the form if `True` |
| choices | Allows to specify a group od choices for the field |
| primary_key | Makes the current field as primary key if `True` |

#### Some common field types:

| Type | Meaning |
|------|---------|
| CharField | Storing short to mid size strings |
| TextField | Storing Large size strings |
| InteferField | Storing integers, and also validating input as integers |
| DateField / DateTimeField| Storing date/time information |
| EmailField | Storing and validating email addresses |
| FileField / ImageField | Storing uploaded files |
| AutoField | Storing an integer that auto increment primary key numbers |
| ForeignKey | Used to specify a foreign key for a one-to-many relationship |
| ManyToManyField | Used to specify a many-to-many relationship |

## Django: Django admin site

### Main Use:

Admin application uses the models to automatically build a site area that can be used to create, view, update, and delete records.

**Note**: In order to access the admin application to manage your models, all you have to do is register the models, then create a superuser to log in to it.

### Creating a super user:

In order to create a superuser all you have to do is run the command below, and then add a username, email address and a strong password when prompted.

    python manage.py createsuperuser

## Things I want to know more about

- None.