# Ruby 2.6.8 container that includes the functionality to run the Cloudfoundry documentation webserver

## Set up the Container and inject the corresponding documentation structure

You can specify the injected documentation repository as mounted volume under the `/tmp` directory. The following example gives you an overview how you can specify it.
```yaml
    volumes:
      - /<directory>/cf/docs-dev-guide:/tmp/docs-dev-guide
```

## Start the container via the compose file

You can start the container manual oder use can also use the `docker-compose up -d` command to run it inside the daemon mode and open the documentation inside your browser under `localhost:4567`. 