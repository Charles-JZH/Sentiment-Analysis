# Sentiment-Analysis

## Three Dockerhub images:  
https://hub.docker.com/repository/docker/charlesjiang1997/sentiment-analysis-frontend  
https://hub.docker.com/repository/docker/charlesjiang1997/sentiment-analysis-logic  
https://hub.docker.com/repository/docker/charlesjiang1997/sentiment-analysis-web-app  

## Steps to get the application to work on GKE  
1. Get the source code from the Github repository given in the handout.  
2. Go into the sa-frontend folder and run "yarn build" to build the project.  
3. Go into the sa-webapp folder and run "mvn install" to get the target jar file.  
4. Docker run all Dockerfiles in these three folder to get three corresponding docker images.  
5. Rename these three docker images via "docker tag" to add my own dockerhub username as the prefix.  
6. Push these images to my own dockerhub. The url of these three images are above.  
7. Log in the GCP. Pull these images from my dockerhub to the GCP.  
8. Rename these images again and push them to Container Registry.  
9. Initialize a new GKE cluster and deploy these images to it.  
