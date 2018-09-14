This is an easy technique to develop Wordpress plugins through a Docker instance with a locally mounted plugins folder.

Wordpress, Apache and MySQL are all automatically created in tidy, isolated containers that can be created and destroyed as needed, but your plugin folder will remain undisturbed.

# Quickstart

1. [Install Docker](https://docs.docker.com/install/).

2. ```
    git clone git@github.com:qoby/wordpress-docker-plugin-dev.git
    cd wordpress-docker-plugin-dev
    docker-compose up
    ```

3. Now just drop any plugins you're developing into the current directory's `plugins/` folder. This is linked to the Wordpress container's `/var/www/html/wp-content/plugins/` folder.

Your Wordpress instance will be available at `http://localhost:8000/wp-admin/`

# See Also

For [Gutenberg](https://wordpress.org/gutenberg/) development, this pairs nicely with [create-guten-block](https://github.com/ahmadawais/create-guten-block):

```
cd plugins
npx create-guten-block my-block
cd my-block
npm start
```
