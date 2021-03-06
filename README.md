# Docker_Project_on_Drupal

Under ``IIEC-RISE 1.0`` Campaign I learnt about Docker under the guidance of Vimal Daga Sir.
I made Two Tier Architecture:-

1.Web Tier:-Where front-end application code is hosted. Front-end application is openly accessible over the internet.

2.Database Tier:-Where the application Database engine and Database is hosted. The database is only accessible from Web Tier only.

<img src="https://www.codeproject.com/KB/applications/1262641/Single_Server_-_Two_Tier.png" width="800" height="500">


## I am going to explain the whole set-up process in this documentation.

## 1. Pre-configurations:-
 - I am using RedHat Enterprise Linux. Plus I have also installed Docker Software in it. You can use any OS and inside that      OS you should have docker software installed.
## 2. Setting up :-
 - Starting the docker:
 - Use ```systemctl start docker``` to start Docker Service.
## 3.Downloading images:- 

  After that I pull the two images from Docker Hub

   1.MYSQL:5.7:- 
     -Use this commmand```docker pull mysql:5.7```
     - MySQL Image go to this page:https://hub.docker.com/_/mysql
  
  
   2.Drupal:8.8.5-Apache:-
    - Use this command ```docker pull Drupal:8.8.5-Apache```
    - Drupal Image go to this page:https://hub.docker.com/_/drupal
  
  
  <img src="https://github.com/Vishal700-cmd/DOCKER-PROJECT/blob/master/vishal.png" 
  width="800" height="500" >
  
  
  # 4. Docker-Compose:-
  - Before using Docker-Compose you should install the software.Link of the Website :
    https://docs.docker.com/compose/install/
  - You can create and edit this file using vim editor. For that use ```vim docker-compose.yml```. Remember the file name          should always be docker-compose.yml.
  - In the below picture you can see the composed file
  <img src="https://github.com/Vishal700-cmd/DOCKER-PROJECT/blob/master/ymlfile.png"
  width="800" height="500">
  
  
 ### Version:-
  - In each version the style and syntax are different. I used version 3  versions.
 ### Services:-
  - In docker compose we use the term services to rectify which things will run when we start the compose file.
 ### Container name:-
 drupalos are the name of the containers which will be setup. Docker-compose automatically creates the name for the containers using our defined container name.
 ### Volumes:-
  - In docker as soon as we terminate an container our whole data inside that container destroyed. But if we want to make our     data permanent then we have to use docker volume.
 ### Environment:-
  - There are many images in Docker which needs some pre-defined environment variables to run. That's why we need to pass         these variables.
 ## 6. Docker-compose up:-
  - Use ```docker-compose up``` to complete the setup.
  
  
## 7. Drupal:-
  - Got to your browser and type ```localhost:8080``` and done you will be able to see your Drupal

<img src="https://github.com/Vishal700-cmd/DOCKER-PROJECT/blob/master/Screenshot%20from%202020-04-27%2009-43-43.png" width="800" height="500">

#### Further process on Drupal


<img src="https://github.com/Vishal700-cmd/DOCKER-PROJECT/blob/master/Screenshot%20from%202020-04-27%2009-43-59.png" width="800" height="500">



#### Next Process 



<img src="https://github.com/Vishal700-cmd/DOCKER-PROJECT/blob/master/Screenshot%20from%202020-04-27%2009-45-09.png" width="800" height="500">


## Thanku Vimal Daga Sir
