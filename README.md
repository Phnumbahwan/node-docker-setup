![image](https://github.com/Phnumbahwan/node-docker-setup/assets/52746589/ee961c18-7612-4ace-9fdd-f4b849d2b2d0)

# Docker Setup

This document outlines the steps to set up a docker in nodejs.

1. Copy and paste the docker files to your node application with app.js

2. Run this command to build your docker image
    ```bash
    docker build -t my-node-app .
    ```

3. Run this command to run your container. Change the port or container name if needed
   ```bash
   docker run --name my-new-container -p 8080:3000 -d my-node-app
   ```

4. Access your application and visit this url
   ```bash
   http://localhost:3000
   ```

5. To stop just run this command
   ```bash
   docker stop <container_id_or_name>
   ```
   
8. To start again
    ```bash
    docker start <container_id_or_name>
    ```

9. To remove container run this command
    ```bash
    docker rm <container_id_or_name>
    ```

    ```bash
    docker rm -f <container_id_or_name>
    ```

10. If you want to access bash shell just run this command
    ```bash
    docker exec -it <container_id_or_name> /bin/bash
    ```
