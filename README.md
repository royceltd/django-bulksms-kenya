#### Integrate Bulk SMS into your Django project in 2 minutes

[Open a free account](https://bulksms.roycetechnologies.co.ke/) and obtain your apikey

Example sender ID `RoyceLtd`

## Quick start

##### 1. Install this package

```
pip install django-bulksms-kenya
```

##### 2. Install requests

```
pip install requests
```

##### 3. Add roycebulksms into installed apps

```
INSTALLED_APPS = [
   ...
   'roycebulksms',
   ]
```

##### 4. Include the roycebulksms URLconf in your project urls.py like this

```
path('roycebulksms/', include('roycebulksms.urls')),
```

Run `python manage.py migrate` to create the Bulk SMS models.

5.Start the development server and visit http://127.0.0.1:8000/admin/
to login, for security anly loggin users can access the bulksms UI (you'll need the Admin app enabled).

6.Visit http://127.0.0.1:8000/bulksms/ to access to Bulk SMS UI. (Add Sender and API key Obtained from Bulk SMS portal).

###### Open a free account](https://bulksms.roycetechnologies.co.ke/) and obtain your apikey

#### Sending from a view

- import sendTextMessage

```
from roycebulksms.views import sendTextMessage
```

- send Text message

```
sendTextMessage('0713727937', 'text', 'RoyceLtd')
```

- access status of sent text in the outbox
