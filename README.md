Docker Slim3 PHP WebApp Template
================================

A template to build websites using PHP 7.2 with Ubuntu 18.04 containers.
This currently uses the [slim framework](http://www.slimframework.com/) version 3.


### Usage

```bash
# Create your project from this template using composer.
composer create-project programster/web-app-template my-project-name

# Use composer to pull the slim framework
cd Docker-Slim3-PHP-WebApp-Template/app
composer update

# Create the .env file from the template file
# be sure to review its settings and fill in appropriately.
cp .env.tmpl .env


# Build and deploy the docker container.
cd ../docker
bash build.sh
bash deploy.sh
```


### Dev Deployment
Whilst developing your application, you can make use of the `dev-deploy.sh` script instead
of the `deploy.sh` script. The difference is that your container will load your files through a 
volume. Thus your changes are reflected immediately and you do not have to keep rebuilding and 
re-deploying your docker container.


### Private docker registry
Click [here](http://blog.programster.org/2015/03/17/run-your-own-private-docker-registry/) to find out how to deploy your own private docker registry in under a minute.


### Cron Jobs
Easily add cron jobs to your container by adding lines to the `docker/crons.conf` file.
