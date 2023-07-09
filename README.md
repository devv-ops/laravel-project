# laravel-project

#### 1. Download project  

#### 2. Navigate in project directory  
`cd laravel-project`
 
#### 3. Create .env file
`cp .env.example .env`  

#### 4. edit database connection
nano .env

#### 5. Start everything
`docker-compose up -d --build`  

#### 6. Composer install
`docker exec -it project_app bash`
`composer install`

#### 7. Check&migrate db
`php artisan migrate`

#### 8. Generate key for Laravel application
`docker-compose exec app php artisan key:generate`  
`exit`

#### 9. Profit
Enter on http://localhost  

#### P.S You maybe need the following commands
`sudo chmod 777 -R storage`
`sudo chown -R $USER:$USER ~/laravel-project`
