# Readme

Owncloud  is a **file sharing** that makes it easy to share and sync content. The docker-compose.yml file contins images for the Owncloud Server, Maria DB and Redis.


# .env

The  **.env** file is your environment variable file and is used to define the version, domain, admin user and password and port. This file must be included in the same folder as the docker-compose.yml file. 

## Usage:

 1. Update the **.env** to reflect your requirements.
 2. Build the image by running `docker-compose up -d` it is important to run this from the same directory as the docker-compose.yml and .env files
 3. Open your brouser and go to the domain and port you defined in you .env file eg: http://localhost:8080/login
 4. login with the username and password you defined in the .env file, eg: admin and admin
 5. To shutdown the environment run `docker-compose down`


## Additional Commands:

 - To view all images run : `docker-compose images
 - To get shell access to a server type: `docker-compose exec container-name command`
	 - e.g:.  `docker-compose exec owncloud /bin/bash`
 - ownCloud provides a list of commands that can be run to perform general administration tasks. A list of ownCloud commands can be found on their website
	 - e.g:.`docker-compose exec owncloud occ user:list` 
	
