# EmployeeApp-Config-Server
Spring Config server Demo

* Provides server-side and client-side support for externalized configuration in a distributed system.
* With Config Server we have a centralized place to manage external properties for applications accross all environments
* This configuration store is versioned under GIT and can be modified at application runtime

#How it works?
There are 2 applications(microservices) one has all the logic (server) and the other (client) is just making a call to this first application. We have to create a config server due to which the client will interact with the config server - this config server will have a url to the git repository this git repo will have a file applications.properties which will have the url to connect with the server insted of interacting with the server directly.
