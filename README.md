# LAB - Class 27

## Project: Django Models

### Author: Christopher Yamas

### Setup

With this repo on your and Python3 on your local machine, while in root directory run terminal command `pip3 install -r requirements.txt`.

To view the Home page, simply run `python manage.py runserver` and go to the path specified in terminal following the words `Starting development server at`

To view each snack's details page, click on the hyperlinked name of the snack on the Snack List page.

To create a "superuser" account that can access the admin features of the Django project and app, run `python3 manage.py createsuperuser` in the terminal and follow the prompts of for username, email address, and a *strong* password.

### Tests

Tests are contained in the `snacks/tests.py` file.

They can be run in the terminal with command `python manage.py test`.

1. The first test checks that a Snack object can be created by a test user.
2. The second test checks the status code for the `snack_list` url page get request is responding (i.e. the page is working).
3. The third test checks that the `snack_list` url page is using the `snack_list.html` template, as well as extending the `base.html` template.
4. The fourth test checks that the snack object that was created in the initial test is being accessed from the `object_list` being displayed `snack_list` page, and that it possesses all the attribute values specified for its `name`, `purchaser`, and `description`.
5. The fifth test checks the status code for the `snack_detail` url page get request is responding (i.e. the page is working).
6. The sixth test checks that the `snack_detail` url page is using the `snack_detail.html` template, as well as extending the `base.html` template.
7. The seventh test checks that the snack object that was created in the initial test is being accessed as the object on the first `snack_detail` page, and that it possesses all the attribute values specified for its `name`, `purchaser`, and `description`.
