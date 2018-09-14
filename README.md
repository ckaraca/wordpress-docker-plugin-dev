This is an easy technique to develop Wordpress plugins through a Docker instance with a locally mounted plugins folder.

# Quickstart

```
git clone git@github.com:qoby/wordpress-docker-plugin-dev.git
cd wordpress-docker-plugin-dev
docker-compose up
```

Now just drop any plugins you're developing into the `plugins/` folder.

Your Wordpress instance will be available at `http://localhost:8000/wp-admin/`

