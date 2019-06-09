# Demoapp

The app work using springboot based microservice which hosts backed service with an in-memory database. And in addition, user interface is built using angular 7 using typescript.

1. Run the backend component and that should launch microservice at port 8888
2. Test using http://localhost:8888/users
3. h2 database can be accessed using http://localhost:8888/h2-console
4. in order to start fonttend app, make sure npm is installed, start node server using command
`ng serve --open`
5. App should be available on http://localhost:4200/users