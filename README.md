## Running this app

This app ẃas created following this tutorial:

https://docs.docker.com/compose/rails/

Start the app
`sudo docker-compose up -d`

Create a db
`sudo docker-compose run web rake db:create`

(This is also in Dockerfile but not working)
`RUN web rake db:create`

DB migration:
```
>docker exec -it dockertwo_web_1 rake db:migrate
== 20170217120000 CreateBreweries: migrating ==================================
-- create_table(:breweries)
   -> 0.0171s
== 20170217120000 CreateBreweries: migrated (0.0173s) =========================

juhapekm@dhcp-asv-114:~/Git_projects/OhtuProjekti/Docker-two$ 
>docker exec -it dockertwo_web_1 rake db:seed
juhapekm@dhcp-asv-114:~/Git_projects/OhtuProjekti/Docker-two$ 
>

```

### TEST EDIT
