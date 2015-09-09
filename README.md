starter-python-django
=====================

This repo contains a [cookiecutter](https://github.com/audreyr/cookiecutter)
template for a Twilio [Django](https://www.djangoproject.com/) tutorial.

## Quickstart

1. Install cookiecutter on your laptop - most people install it directly to
their OS's Python, not using a virtualenv:

    ```
    pip install cookiecutter
    ```

1. Create an empty git repository and clone it (but don't `cd` into it)

1. Create a Django project using the template with this command:

    ```
    cookiecutter gh:TwilioDevEd/starter-python-django
    ```

After answering a few questions, you'll have a brand-new Django project
that's ready to grow into an informative tutorial!

## Things you'll need to check

This project template makes a few assumptions that you'll need to check
before you publish your tutorial:

### Twilio credentials

Not all our apps need to make Twilio REST API calls. If that's yours, be sure
to remove the API credentials from `.env_example`.

### Bootstrap

If your app doesn't need Bootstrap for some reason, you'll need to remove those
dependencies from `requirements.txt`, the `settings/common.py` module and the
`base.html` template.
