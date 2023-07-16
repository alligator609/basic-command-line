# list of docker images
```docker images```
# run specific container
```docker run hello-world```
# only shows running containers
```docker ps```
# Show all the running containers
```docker ps -a```
# Remove container
```docker rm docker-tutorial```
# run docker at local-> 8080 into container -> port 80 
```docker run -p 8080:80 --name docker-tutorial -d docker101tutorial  ```
(docker-tutorial= given name docker101tutoral= image name)

# Stop specific container
```docker stop docker-tutorial```
# for shutting down wsl virtual mactine
```wsl --shutdown ```
