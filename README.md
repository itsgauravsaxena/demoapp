# Demoapp


#### Run basic application

The app work using springboot based microservice which hosts backed service with an in-memory database. And in addition, user interface is built using angular 7 using typescript.

1. Run the backend component and that should launch microservice at port 8888
2. Test using http://localhost:8888/users
3. h2 database can be accessed using http://localhost:8888/h2-console
4. in order to start fonttend app, make sure npm is installed, start node server using command
`ng serve --open`
5. App should be available on http://localhost:4200/users


#### Running in containers
###### Spring boot part
1. Easiest way is to make Docker file and run few commands locally
2. To test if images can be built - type 
` docker build -t demoapp .`
3. To create an image with tag, use command
`docker image build -t gauravimages/demoapp .`
4. To run image as a container, use this command
`docker container run --name demoapp -p 8888:8888 -d gauravimages/demoapp`
5. Use command `docker ps` you should be able to list containers
6. You can can access this using running app
`curl http://0.0.0.0:8888/users`

###### node part


