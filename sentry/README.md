First run docker-compose to get everything up:

Sentry: https://github.com/Turistforeningen/sentry

```
docker-compose up -d
```

Once things are up, run this to init the sentry db:
```
docker-compose exec sentry sentry upgrade
```
Make sure to answer the question about creating a user to access the site.
Login to the site via the exposed web ui on port 9000.
