# Installation of Docker in Ubuntu :-
    sudo apt-get update 
    sudo apt-get install docker.io 
    
`Here we are installing Docker at Linux(ubuntu),then we will check for docker-compose is installed inside the docker`

# Check if Docker Compose is installed 
      sudo apt-get docker-compose 
`if the command docker-compose dosen't exits then install docker compose`

 # Install Docker Compose
       sudo apt-get install docker-compose
       
# Create docker-compose.yml file

`For installation of latest verion of wordpress we will create "docker-compose.yaml" file`
 `docker-compose.yaml file consist of three differnet services like (Php,Ngnix and Mariadb ),where yaml file will contain the data for App / Config / Docker and .Env file`
 `Where .Env file will provide the enviroment for the App Name`

# Start the containers
     docker-compose up -d 

`Here docker-compose.yaml file will install the containers and it will directly integrate wih each other`

# Check whether the Ngnix,  docker-compose-lemp-stack_php and  mariadb exits on your docker 
      docker ps 
      
 # For Creating LEMP ( Linux, Ngnix , Mysql and PHP ) 
 `Here we are creating a LEMP stack, which will be running inside the containers with a docker-compose file`

 # Working of LEMP -Stack 
`we are using Nginx as the web server, which listens for HTTP requests and forwards them to the appropriate PHP script`
`Where PHP script generates a response, which is then sent back to the user via Nginx`
`We are using MySQL is used to store and manage the website's data`

# Here we are going to watchout the App , Config and Docker 
`They Provide the diffent files for the execution of the project`

# App
`The name used when creating a container.`
`An app provides the Index.php file, which is bascially based on the Php code and HTML Languages which are going to be used as a website showcase`

# config 
`Here we are creating the Ngnix file for configuration of project as ngnix.conf,it will provide the path to the php and html to localhost by root /var/www/html` 
 `It will provide the web server as localhost to deploy the website`

# Docker 
`Inside Docker we will provide php.dockerfile  with some basic commands for updates and install`

 # Add entry to /etc/hosts 
 `Which the help of /ect/host file you can resolve your Domain name to your IP `

       127.0.0.1     $site_name

 # Enable/disable the site (stop/start containers) 
 
 `For Disable the Container in docker-compose)`
 
     docker-compose stop
     
  'For Enable the Container'

       docker-compose up -d
       
# Delete the site (delete containers and local files) 

        docker-compose down -v 

 # Remove entry from /etc/hosts 

       sudo sed -i "s/$exmaple.com/d" /etc/hosts

     

 
