# django-simple-coupons
##  A Django app that makes the use of coupons a simple task!

![PyPI v0.2](https://img.shields.io/badge/PyPI-v0.2-blue.svg)
![MIT License](https://img.shields.io/badge/License-MIT-lightgray.svg)
![Docs](https://img.shields.io/badge/docs-meh-orange.svg)

django-simple-coupons is a simple Django app to create and use promotional coupons in your website.

### Downloading

django-simple-coupons is available on The Python Package Index (PyPI). You can simply use ***pip*** to install it:

```bash
$ pip install django-simple-coupons
```

### Installing

1 - Add ```django_simple_coupons``` inside INSTALLED_APPS in settings.py:

```python
INSTALLED_APPS = [
        ...
        'django_simple_coupons',
]
```

2 - (Optional) If you want to use more than 12 chars (default) for your coupon code, add ```DSC_COUPON_CODE_LENGTH``` variable in settings.py:

```python
DSC_COUPON_CODE_LENGTH = 16
```

3 - (Optional) If you make use of another User model in your project, add ```DSC_USER_MODEL``` variable in settings.py:

```python
DSC_USER_MODEL = 'custom_auth.models.User'  # app.module.class format (example)
```

4 - Run the migrations:

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

And that's it! django-simple-coupons should appear in your admin as ```Simple Coupons```.

### Documentation

##### [https://github.com/Wolfterro/django-simple-coupons/blob/develop/docs/README.md](https://github.com/Wolfterro/django-simple-coupons/blob/develop/docs/README.md)
