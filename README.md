# Heroku Buildpack MaxMind GeoLite2

Buildpack for the free MaxMind GeoLite2 database packages.

## Configuration

Add the buildpack:

```
heroku buildpacks:add https://github.com/physiovia/heroku-buildpack-maxmind-geolite2
```

Decide which package (City or Country) you need and set up your environment accordingly:

```
heroku config:add MAXMIND_DB_NAME=City
# or
heroku config:add MAXMIND_DB_NAME=Country
```

Then deploy and start using the database.

## Credits

(c) 2017 physiovia GmbH

Heavily inspired by https://github.com/mantisadnetwork/heroku-buildpack-maxmind. Check out this buildpack if you're using the paid versions of MaxMind.

This product includes GeoLite2 data created by MaxMind, available from http://www.maxmind.com.
