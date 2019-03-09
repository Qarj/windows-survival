# Django

## After changing database model

```
python manage.py makemigrations 
python manage.py migrate
```

## Run one test
```
manage.py test summary.tests.KPISummaryTests.test_adobe_fake_api_returns_report_not_ready_on_first_attempt
```

## Disable HTML escaping
```
    <p>Artefact url: {{ url|safe }}</p>
```

## Disable CSRF token
```
from django.views.decorators.csrf import csrf_exempt

@csrf_exempt
def feature(request):
```

## Format a date

```
firstTestLogDate = runLab[0].date_created.strftime("%a %d/%m/%Y %H:%M:%S") # Wed 18 Mar, 2018 15:11:05
```
