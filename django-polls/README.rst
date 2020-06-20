
====
Polls
====

Polls is a Django app to conduct web-based polls. For each question,
visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. App "polls" to your INSTALLED_APP setting like this::

    INSTALLED_APP = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('polls/', Include('polls.urls')),

3. Run ``python manage.py migrate`` to create the polls models.

4. Start the development sever and visit http://127.0.0:8000/admin/
    to create a poll(you'll need the Admin app enabled).

5. Visit http://127.0.0:8000/polls/ to participate in the poll.