# Installing Tools and Dependencies for PHP
## Composer
### Install Composer using Docker
1. cd to your project
2. Execute docker run

        docker run --rm -v $(pwd):/app composer install

# Running PHP on docker
## For development
1. Ready for the source code
2. Create docker file
3. Build docker image
4. Run docker container from built image

        docker run -d -p 80:9000 --name my-php-project -v ./:/var/www/html/ my-php-image
