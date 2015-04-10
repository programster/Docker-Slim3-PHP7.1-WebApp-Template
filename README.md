# docker-php-website-template
A template to kick off a dockerized website built in PHP (currently using the [slim framework)(http://www.slimframework.com/) )

### Usage

```
# Clone this repo
git clone https://github.com/programster/docker-php-website-template.git

# Use composer to pull the slim framework
cd docker-php-website-template/project
composer update

# Edit the content of the docker_settings.php in the settings folder
# and point it to your own private docker registry.
# CHange the VIRTUAL_HOST and the PROJECT_NAME whilst you're at it.

# Build the container and run it.
cd docker
bash build.sh
bash run-container.sh
```
