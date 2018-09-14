Develop Wordpress plugins easily through a Docker instance with a locally mounted plugins folder.

Wordpress, Apache and MySQL are automatically created in tidy, isolated containers that can be created and destroyed as needed while your plugin folder remains undisturbed.

# Quickstart

1. [Install Docker](https://docs.docker.com/install/).

2. ```
    git clone git@github.com:qoby/wordpress-docker-plugin-dev.git
    cd wordpress-docker-plugin-dev
    docker-compose up
    ```

3. Put your plugins in the `plugins/` folder. This is linked to the Wordpress container's `/var/www/html/wp-content/plugins/` folder.

Your Wordpress instance will be available at `http://localhost:8000/wp-admin/`

# See Also

For [Gutenberg](https://wordpress.org/gutenberg/) development, this pairs nicely with [create-guten-block](https://github.com/ahmadawais/create-guten-block#getting-started):

```
cd plugins
npx create-guten-block my-block
cd my-block
npm start
```
