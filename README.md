# docker-fundamental

Commands:

1-> 	* docker build -t <image_name> .
	    * docker build -t <image_name>:<version_name> .

2-> 	* docker run --name <container_name> <image_name>
        * docker run --name <container_name> -p 8000:4000 -d <image_name>:<version_name>
        * docker run --name <container_name> -p 4000:4000 -d <image_name>
        * docker run --name <container_name> -p 4000:4000 --rm <image_name>:<version_name>
        * docker run --name <container_name> -p 7000:4000 --rm -v <path>:<container_path> -v <container_path_specific> <image_name>:<version_name>

3-> 	* docker stop <container_name>
    	* docker start <container_name>

4-> 	* docker images
        * docker ps
        * dokcer ps -a

5-> 	* dokcer image rm <image_name>
        * docker image rm <image_name>:<version_name>
        * docker image rm <image_name> -f
    	* dokcer container rm <container_name>

6->	    * dokcer system prune
	    * docker system prune -a

7-> 	* docker-compose down 
	    * docker-compose dowm --rmi all -V