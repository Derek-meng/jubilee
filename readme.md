

## Installation for development

1. Clone jubilee Project
    
        git clone https://github.com/Derek-meng/jubilee.git
        
2. Install `/vendor` dependency from  `composer.json`

        composer install
        
3. copy
   
        cp .env.example .env                

4. Set the application key

        php artisan key:generate
        
5.  Set database connection on `.env`

        DB_CONNECTION=mysql
        DB_HOST=127.0.0.1
        DB_PORT=3306
        DB_DATABASE=laravel
        DB_USERNAME=root
        DB_PASSWORD=

6. Migrate database with simple data
        
        php artisan migrate
7. Run Seed 
        
        php artisan db:seed
        
8. Set Env File Key
```
JUBILEE_AUTHED_HOME_URL=Host Url
JUBILEE_FACEBOOK_CLIENT_ID= your facebook client id
JUBILEE_FACEBOOK_CLIENT_SECRET= your facebook client key
JUBILEE_FACEBOOK_CLIENT_REDIRECT_URL= {host_url}/auth/facebook/feedback


```
            

## Package List

1. Reference

    - [十二星座爬蟲 ComposerPackage](https://github.com/Derek-meng/click108.git) 
    - [十二星座爬蟲 with Laravel](https://github.com/Derek-meng/laravel-click108.git)
    - [Auth with Facebook Laravel Package](https://github.com/Derek-meng/jubilee-laravel-auth)
    - [independent.kit](https://github.com/Derek-meng/php-independent.kit.git)
    


## Example
#每日抓取Command:
```
php artisan detector:constellations
           or
php artisan schedule:run  
```


