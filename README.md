# python-getting-started

A barebones Scipy+Python app, which can easily be deployed to Heroku.

## Running Locally

Make sure you have Python [installed properly](http://install.python-guide.org).  Also, install the [Heroku Toolbelt](https://toolbelt.heroku.com/).

```sh
$ git clone git@github.com:brook-seaton/scipy-getting-started.git
$ cd scipy-getting-started
$ pip install -r requirements.txt
$ python manage.py syncdb
$ foreman start web
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```sh
$ heroku create
$ git push heroku master
$ heroku run python manage.py syncdb
$ heroku open
```

## Documentation

For more information about using Python on Heroku, see these Dev Center articles:

- [Python on Heroku](https://devcenter.heroku.com/categories/python)

