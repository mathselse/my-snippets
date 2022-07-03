# Instalation for Development
## Get lavavel
1. Clone from Repo

        git clone https://github.com/laravel/laravel.git laravel-web
2. Better to change permission to non-root user

        sudo chown -R $USER:$USER ~/laravel-web
    
## Running on Container
### Quick manual run using sail image

        docker run -d -p 8000:80 --name=my-php-project -v $(pwd):/var/www/html sail-8.1/app
