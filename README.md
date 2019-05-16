# Dockerized Rails 5 App
 
Example of how to dockerize a rails app 

## Getting Started




### How to Run

1. Install Docker for mac osx. [Docker](https://store.docker.com/editions/community/docker-ce-desktop-mac)

2. Clone the repo:

       $  git clone git@github.com:mehedikhan/dockerized-rails5-app.git

3. Build container image.

       $ docker-compose build
           
4. Run application and docker containers

       $ docker-compose up
        
5. Prepare application database and users

       $ docker-compose exec app rake db:create
       $ docker-compose exec app rake db:migrate
       $ docker-compose exec app rake db:seed        

6. Access the app at [http://localhost:3000/](http://localhost:3000/)        
        
