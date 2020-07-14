# Django Haystack Example App
Repository contain sample app to test out a basic feature of django haystack

Additional info can be found at [Haystack](https://django-haystack.readthedocs.io/en/master/index.html) and [drf_haystack](https://drf-haystack.readthedocs.io/en/latest/01_intro.html) 

## Application Setup

### Run Migrations
- `python manage.py migrate`
- `python manage.py runserver`

## SQL query to generate test record in sqlite
`insert into example_location(latitude, longitude, address, city, zip_code, created, updated) values (1000,-1000,'Test town test area test town','Test City','10000',' 2017-03-17 18:37:29.229991',' 2017-03-17 18:37:29.229991')`


## Run Query

You can also use field lookups in your field queries. See the Haystack [field lookups](https://django-haystack.readthedocs.io/en/latest/searchqueryset_api.html?highlight=lookups#id1) documentation for info on what lookups are available. A query using a lookup might look like the following:

http://example.com/api/v1/location/search/?city__startswith=Test
