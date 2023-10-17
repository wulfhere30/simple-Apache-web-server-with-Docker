# Ukrainian Poem with Apache on Docker

## Introduction

This project is a simple Apache web server deployed with Docker that displays a Ukrainian poem on a web page. The app can be run locally or on a remote host.

## Requirements

- Docker

## Installation and Running

### Local Deployment

#### Using Docker and Apache

1. **Clone the Repository:**

    ```bash
    git clone [Your GitHub Repository URL]
    ```

2. **Navigate to your project directory where the Dockerfile is located.**

    ```bash
    cd [Your Project Directory]
    ```

3. **Build the Docker Image:**

    ```bash
    docker build -t ukrainian-poem-apache .
    ```

4. **Run the Docker Container:**

    ```bash
    docker run -p 8080:80 ukrainian-poem-apache
    ```

After completing these steps, open your web browser and navigate to `http://localhost:8080/your_html_file.html` to verify the deployment.

### Remote Deployment

If you want to run this app on a remote host, you can push your Docker image to a registry like Docker Hub and then pull it on the remote machine, or you can build it directly on the remote machine by following the same steps as above.

To make the application accessible from the Internet, you may need to configure your firewall and port forwarding settings to expose port 8080. 

## Additional Commands for Apache

- To check Apache server status:

    ```bash
    docker exec -it [CONTAINER_ID] /bin/bash
    apachectl status
    ```

- To reload Apache configuration:

    ```bash
    docker exec -it [CONTAINER_ID] /bin/bash
    apachectl graceful
    ```

## License

This project is distributed under the MIT License. See `LICENSE` file for more details.

