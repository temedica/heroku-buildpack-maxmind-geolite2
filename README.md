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

Add your licence key, which is now a requirement for downloading even the free databases.
```
heroku config:add MAXMIND_KEY=Your-License-key
```

Then deploy and start using the database.

## Credits

Forked from physiovia GmbH https://github.com/physiovia/heroku-buildpack-maxmind-geolite2

Heavily inspired by https://github.com/mantisadnetwork/heroku-buildpack-maxmind. Check out this buildpack if you're using the paid versions of MaxMind.

This product includes GeoLite2 data created by MaxMind, available from http://www.maxmind.com.
