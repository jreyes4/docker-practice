### Overview
This is a simple project practicing setting up a docker environment. 

The project makes use of Docker-Containers to run a react project. My main purpose for creating this was project was to learn the steps to setting up a single container project before moving on to a multi-docker setup. As a result, the react project in my container is a simple out of the box setup that does not contain any special functionallity.

The project makes use of docker-compose to handle the local DEV environment. I also have a travis.yml file that is used when I push changes to the master branch of this repo. Travis CI takes care of building the production image of my docker project and rolling out that images to AWS if there are no build errors. On the AWS side, the full image is deis deployed to an Elastic Beanstalk service I setup. 

Update: I've shut down the AWS service, but the files have been kept available for viewing. 

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
