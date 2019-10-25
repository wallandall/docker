1)	The file .env contains the version, domain, password and port which can be changed as needed.
2)	To build the images run: docker-compose up -d 
	-This needs to be run from the directory where the docker-yml and .env files are located
3) 	To view all containers run: docker-compose images
4)	Open your brouser and go to the domain and port you defined in you .env file eg: http://localhost:8080/login
5) 	login with the username and password you defined in the .env file, eg: admin and admin
6)	If you need to log into one of the servers and run system commands, you can type:
	-docker-compose exec container-name command
	-eg: 
         docker-compose exec owncloud /bin/bash
	 you can also run owncloud OCC commands
	 docker-compose exec owncloud occ user:list
7) 	To shut down th images, type: docker-compose down
	-To start the images again you can run the start command
	-When shutting down the containers, it will not delete the images you need to delte them
	*All files files will be stored in the images in the location defined so if you do delete the images all files, configuration etc 	will be deleted
	
