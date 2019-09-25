# Devbox
 
#### CONTAINS
This devbox contains: 
 - linux(ubuntu) 
 - apache2 
 - mysql
 - php7.2
#### CONTENT

* [Devbox usage](#devbox-usage)
* [Devbox db connect](#devbox-db-connect)
* [Default ports](#default-ports)

#### Devbox usage

Requirements on local machine

    - Install php7.X version
    - Install composer

Env setup (For laravel projects)
    
    - git clone <project>
    - Root folder: 'docker-compose up --build -d'
    - Run 'cd web/'
    - In web/ run: 'composer install'
    - Move .env.example to .env
    - Run: php artisan key:generate
    - Open localhost:8080 in browser

Navigate to root folder

- For first time run
	`docker-compose up --build -d`

- In opposite to start run
	`docker-compose start`

- To stop the containers 
	`docker-composer stop`
	
- To kill the containers 
	`docker-compose kill`

- To ssh container
	`docker exec -it <container_id> bash`

#### Devbox db connect 
	- user: devbox
	- pass: devbox
	- db: tubeDb
	- servername: devbox-mysql

#### Default ports
	- Webserver `localhost:8080`
	- Mysql `3306`
