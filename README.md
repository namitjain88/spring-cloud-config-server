# spring-boot-config-server
A sample project to understand a dedicated configuration spring-boot service to provide configuration to all services and it's copies in a spring-bot env.

# Spring Cloud Config Server
* It can connect to Git Repo and listens to changes committed.
* Connecting to Git also helps maintain version history
* Create spring-boot app with Config Server as dependency
* Add @EnableConfigServer to Main class
* Add spring.cloud.config.server.git.uri: ${HOME}/relative-path-of-gitrepo-folder OR GitHub URI
* Change port to 8888 per spring cloud config server convention
* Access gitrepo config file using http://localhost:8888/<file-name>/<profile-name> e.g. http://localhost:8888/application/default
