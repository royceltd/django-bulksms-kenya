Django Bulk SMS Kenya is a Django app that helps you send Bulk sms to groups or contacts via an easy to use UI. 
You can also send Bulk sms from any Django view function



Quick start
-----------

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'roycebulksms',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('roycebulksms/', include('roycebulksms.urls')),

3. Run ``python manage.py migrate`` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/bulksms/ to participate in the poll.

.. image:: https://docs.typo3.org/m/typo3/docs-how-to-document/main/en-us/_images/a4.jpg
   :alt: some image
   :target: https://typo3.org
   :class: with-shadow
   :scale: 50