# Read: Class 29

## Django: Custom User Model

In order to create a custom user model we need to use something called `AbstractUser`.

### Using AbstractUser:

In order to do that we need to do a couple of things:

- Inform Django of the new custom user model using `AUTH_USER_MODEL` within `settings.py`: ex:

        AUTH_USER_MODEL = "app_name.CustomUser"

- Update `models.py` with the new user model:

        class CustomUser(AbstractUser):
            pass
            # add additional fields in here

            def __str__(self):
                return self.username

- Create a new file inside the **django-app** called `forms.py`, which should include the two methods, one for a **creation form**, and another for a **changing form**: ex ([source](https://learndjango.com/tutorials/django-custom-user-model))

        from django import forms
        from django.contrib.auth.forms import UserCreationForm, UserChangeForm

        from .models import CustomUser

        class CustomUserCreationForm(UserCreationForm):

            class Meta:
                model = CustomUser
                fields = ("username", "email")

        class CustomUserChangeForm(UserChangeForm):

            class Meta:
                model = CustomUser
                fields = ("username", "email")

- Update `admin.py`, with the new model and forms: ex ([source](https://learndjango.com/tutorials/django-custom-user-model))

        from django.contrib import admin
        from django.contrib.auth.admin import UserAdmin

        from .forms import CustomUserCreationForm, CustomUserChangeForm
        from .models import CustomUser

        class CustomUserAdmin(UserAdmin):
            add_form = CustomUserCreationForm
            form = CustomUserChangeForm
            model = CustomUser
            list_display = ["email", "username",]

        admin.site.register(CustomUser, CustomUserAdmin)

- Create a home template that will hold the log in stuff, and reference it in `settings.py`, ex:

    LOGIN_REDIRECT_URL = "home"
    LOGOUT_REDIRECT_URL = "home"

The rest is up to you as the developer to add view and shap the output.



## Things I want to know more about

- None.