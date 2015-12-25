# Web Engineering 2015-2016 / Microservices


##The two microservices are running and registered.
####Accounts Server
![Account Microservice](https://github.com/diegozgz92/Laboratory-6-microservices/blob/master/AccountsServer.png)
####Web Server
![Web Microservice](https://github.com/diegozgz92/Laboratory-6-microservices/blob/master/WebServer.png)

##The service registration service has the two microservices registered.
![Microservices registred](https://github.com/diegozgz92/Laboratory-6-microservices/blob/master/RegistrationService.png)

##A second account microservice is running in the port 4444 and it is registered.
![Second Account Microservice](https://github.com/diegozgz92/Laboratory-6-microservices/blob/master/AccountsService2.png)

##A brief report describing what happens when you kill the microservice with port 2222. Can the web service provide information about the accounts? Why?
When you kill the microservice with port 2222, the Web service Microservice, when you try to do an operation, shows the error "Refused connection" because it dont know that dont work. After 20-30 sec its work again.
Its because the microservice don't working, and after a few second asks registration service for other ACCOUNTS-SERVICE, it respond with the microservice with port 4444, and start working again.
