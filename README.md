## Running this app

This app ẃas created following this tutorial:

https://docs.docker.com/compose/rails/

Start the app
`sudo docker-compose up -d`

Create a db
`sudo docker-compose run web rake db:create`

(This is also in Dockerfile but not working)
`RUN web rake db:create`
