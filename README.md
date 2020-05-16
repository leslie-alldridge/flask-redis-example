# flask-redis-example

Polling task queue in redis using flask

### Deploy

git push staging master (or specific branch)

git push prod master

staging URL https://flask-redis-staging.herokuapp.com/

prod URL https://flask-redis-prod.herokuapp.com/

last command I ran was \$ python manage.py db migrate

### Database

connect to db `psql -U postgres`

### Dyno config

Worker and server currently run on the same dyno (small workload). Best to create separate dyno's for heavier workloads.

### Other notes

Latest Redis introduces a breaking change (need to investigate)
