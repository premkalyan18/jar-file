# premkalyan

Your description here

# Project information

The project starts out with a fully configured minimal JakartaEE 9 setup and HelloWorld endpoint

# Project Commands 

| Command          | Description                                                                                                                                                                                                                                                 |
|:-----------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| run              | Start docker locally and expose docker volume `/opt/payara/payara5/glassfish/domains/domain1/autodeploy` to directory `./artifact` so that every time `mvn package` is run locally it will automatically redeploy the application in the docker environment |
| build            | will build the application and the docker image                                                                                                                                                                                                             |
| build-run        | will build the application and the docker image and run locally                                                                                                                                                                                             |
| build-deploy     | will build the application and the docker image and deploy that image to the docker registry                                                                                                                                                                |
| buildx-boodstrap | will bootstrap docker buildx for multi platform builds                                                                                                                                                                                                      |
| buildx-deploy    | will build the application and the docker image for amd64 and arm64 architectures                                                                                                                                                                           |
| buildx-stop      | removes the buildx multi-platform config (cleanup)                                                                                                                                                                                                          |
| logs             | will show the logs if run with `build-run`                                                                                                                                                                                                                  |

# Docker

* The docker image is hosted as [ivonet/payara](http://ivo2u.nl/tM)
* The docker image is maintained [here](http://ivo2u.nl/oO) 

# Example endpoint

[http://localhost:8080/premkalyan/rest/example](http://localhost:8080/premkalyan/rest/example)
[health check url](http://localhost:8080/health)