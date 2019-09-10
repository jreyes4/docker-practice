### Overview
This is a simple project practicing setting up a docker environment. 

The project makes use of docker and docker-compose to run a react project. The react project is a simple out of the box setup that does not contain any special functionallity. My main purpose for creating this project was to learn the steps to setting up a single container project before moving on to a multi-docker setup. 

The project makes use of docker-compose to build locally in a DEV environment. There is a travis.yml file that is used when pushed to the master branch on my repo that takes care of creating and rolling out to the production environment. The travis.yml file sets up the images and pushes them to AWS for to be hosted by Elastic Beanstalk. The AWS service is not currently running, but the files have been kept available for viewing. 

### Running Locally

The project can be run locally by pulling the repo and ensuring you have docker installed on your local machine. To run the project, run ;;'docker-compose up' in your terminal window from the project directory. You should see that the client test suite and web client run succesfully.

To see the project navigate to one of the following:

Docker Desktop 
[http://localhost:3000/]

Docker Toolbox
[http://192.168.99.100:3000]

There is currently not much to see, but future goals are to add more tests and customize the page.

### Source

Material and guidance for this project is provided through Stephen Grider's exceptional Docker and Kubernetes introductory course.

https://www.udemy.com/docker-and-kubernetes-the-complete-guide/
