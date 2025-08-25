# Created-a-Docker-image-using-Javascript-
Developing a Simple Java Script Application and Creating a Docker Image of the Application
Read on [Medium Link](https://medium.com/@ejadaji7/developing-a-simple-java-script-application-and-creating-a-docker-image-of-the-application-f7bed9f4447e?source=user_profile_page---------0-------------a93f2578e95f----------------------)

I built a simple application using Java script which outputs “My first application deployed successfully “.

Prerequisites

Install the following

1. Docker

2. Docker desktop

3. Git Bash

4. VS Code

Introduction

Docker is a virtualization software which makes development and development of applications easy by packaging an application into a container that has dependencies, it's libraries, configuration, running environment and system tools. That is application and its running environment are packaged into a docker package that can easily be shared. Once you have Docker runtime installed on the server you can simply run Docker command . Docker Desktop an application was created to allow me build, share and run containerized applications and managements. It includes Docker Engine, Docker Client, GUI Client etc. Docker images which are read-only templates containing instructions needed in creating Docker containers were created to let me run the application. I created Docker container, a running instance of an image, an isolated process that packages all the files an application needs, letting my application run consistently on one or more environments .

Building my image, I created an image from a definition written in Dockerfile.

Below is my server.js file

<img width="1100" height="404" alt="image" src="https://github.com/user-attachments/assets/a02d2736-d963-481a-8714-74e77e6b4b69" />


My package.json file

<img width="1100" height="390" alt="image" src="https://github.com/user-attachments/assets/2885c23a-86f2-4132-bc15-e585afdd9be2" />


The root of my application

<img width="377" height="272" alt="image" src="https://github.com/user-attachments/assets/c8cf8f43-7faf-4407-a632-709ab6398808" />


I created a Dockerfile

<img width="1100" height="424" alt="image" src="https://github.com/user-attachments/assets/52d14d3c-38ee-475e-89b0-e596f48bf52c" />


Built the image by running the command below

docker build -t node-app:1.0.
<img width="1100" height="273" alt="image" src="https://github.com/user-attachments/assets/5e009307-c0c9-4838-a754-cfafddba1c1a" />


I ran the application executing the command below

docker run -d -p 3000:3000 node-app:1.0
<img width="1100" height="209" alt="image" src="https://github.com/user-attachments/assets/7fc08464-b918-48ae-b6ca-d49246dbf746" />


Back on the browser is the message from my application .

I opened the browser and typed in localhost:3000 to check if my node-application was successful.

<img width="858" height="511" alt="image" src="https://github.com/user-attachments/assets/0b13a0d0-405f-4dd8-93b8-752a92a140e6" />






