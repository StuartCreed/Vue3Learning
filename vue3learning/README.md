Laravel v8 (with Sail and BrowserSync), VueJS v3 with Vue Loader boilerplate.

<u>Sail config</u><br/>
docker-composer.yml file changed to use port '8081:80' so that the app runs on localhost:8081, as I have another program that uses localhost:8080 (the default for Sail).
See https://dev.to/stuartcreed/using-laravel-sail-docker-composer-for-laravel-on-a-existing-application-24k5 for more information.
