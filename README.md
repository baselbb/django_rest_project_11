# django_rest_project_11
Django REST API backend for Dog selection website

## Run Project from your terminal on your local server
`python manage.py runserver`

## Coverage Report
file|statements| miss| cover|
----|----------|-----|------|
pugorugh_models.py|36|2|94%|
pugorugh_serializers.py|26|4|85%|
pugorugh_urls.py|7|0|100%|
pugorugh_views.py|97|28|71%|
backend_urls_py.html.py|9|0|100%|
pugorugh_tests_py.html|140|0|100%|

# Project Requirements
Project Instructions

## To complete this project, follow the instructions below. If you get stuck, ask a question in the community.
The application needs the following models with the associated field names included.

### Dog Model
- name
- image_filename
- breed
- age - integer for months
- gender - “m” for male, “f” for female, “u” for unknown
- size, "s" for small, "m" for medium, "l" for large, "xl" for extra large, "u" for unknown

### UserDog Model
- user
- dog
- status - “l” for liked, “d” for disliked

### UserPref Model
- user
- age - “b” for baby, “y” for young, “a” for adult, “s” for senior
- gender - “m” for male, “f” for female
- size - “s” for small, “m” for medium, “l” for large, “xl” for extra large

Serializers are needed for the Dog and UserPref Models. All fields need to be revealed except user from the UserPref Model.
The front end JavaScript application is expecting the following routes to be in place:

To get the next liked/disliked/undecided dog

`/api/dog/<pk>/liked/next/`

`/api/dog/<pk>/disliked/next/`

`/api/dog/<pk>/undecided/next/`


To change the dog's status

`/api/dog/<pk>/liked/`

`/api/dog/<pk>/disliked/`

`/api/dog/<pk>/undecided/`

To change or set user preferences

`/api/user/preferences/`

The supplied project includes Token-Based Authentication, that functionality should be maintained.
Unit test the app. Write unit tests to test that each view is displaying the correct information. Write unit tests to test that the models, classes, and other functions behave as expected.

### Extra Credit
To get an "exceeds" rating, you can expand on the project in the following ways:
1. Extend the application by allowing the addition or deletion of dogs to the site.
2. Add additional data fields to the Models which increase the application’s functionality.
3. Additional routes are added to site which increase the application’s functionality.
4. Unit tests cover more than 75% of the views, models, and other functions.
