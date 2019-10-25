# Elasticsearch



# .env

The  **.env** file is your environment variable file and is used to define the version, domain, admin user and password and port. This file must be included in the same folder as the docker-compose.yml file. 

## Usage:

 1. Update the **.env** to reflect your requirements.
 2. Build the image by running `docker-compose up -d` it is important to run this from the same directory as the docker-compose.yml and .env files
 3. To shutdown the environment run `docker-compose down`


## Additional Commands:

 - To view all images run : `docker-compose images
 - To get shell access to a server type: `docker-compose exec container-name command`
	 - e.g:.  `docker-compose exec owncloud /bin/bash`
