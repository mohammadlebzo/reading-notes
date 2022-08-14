# Read: Class 33

## JSON Web Tokens

### Definition:

JSON Web Token is compact, self-contained way for securely transmitting information between parties as a JSON object.
And because it is digitally signed, it can be verified and trusted.
JWTs can be signed using either a secret key, which uses *HMAC* algorithm, or a public/private key by using *RSA* or *ECDSA*.

The reason behind using signed tokens is to verify the integrity of it's content and hide it from other parties, but that raises a question, which is when should these signed tokens be used ? 

### When should you use Tokens?

Tokens are used mainly for:

- **Authorization**: using these tokens allow you to confirm the permissionlevel of the users when using any service or when performing any kind of activity in your application.

- **Information Exchange**: using tokens also allows you to send needed data, while also checking it to make sure that the content hasn't been tempered with.

### JSON Web Token structure:

JSON Web Tokens consist of three parts separated by dots (.), and these parts are:

- Header
- Payload
- Signature

And a JWT usually looks like this:

`xxxxx.yyyyy.zzzzz` -- Header.Payload.Signature

### Installation & Setup:

In order to use tokens in your Django REST api, do the following:

1. install `djangorestframework_simplejwt`:

        pip install djangorestframework_simplejwt

2. Add the following code to `sittings.py` within your Django project:

        REST_FRAMEWORK = {
            'DEFAULT_AUTHENTICATION_CLASSES': [
                'rest_framework_simplejwt.authentication.JWTAuthentication',
            ],
        }

3. Add the following code to `urls.py` within your Django project:

        from django.urls import path
        from rest_framework_simplejwt import views as jwt_views

        urlpatterns = [
            # Your URLs...
            path('api/token/', jwt_views.TokenObtainPairView.as_view(), name='token_obtain_pair'),
            path('api/token/refresh/', jwt_views.TokenRefreshView.as_view(), name='token_refresh'),
        ]

### Why use refresh tokens?

Refresh tokens are used to make sure that users permissions are updated as soon as possible, as they might change with time.

## Things I want to know more about

- None.