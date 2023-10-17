# Ukrainian Poem with Apache

## Introduction

This project displays a Ukrainian poem via an Apache web server. You can run this application locally or deploy it using Docker.

## Requirements

- Apache HTTP Server
- Docker

## Installation and Configuration

### Local Deployment with Apache

1. **Install Apache on Ubuntu:**
    ```bash
    sudo apt-get update
    sudo apt-get install apache2
    ```
   
2. **Check Apache Status:**
    ```bash
    sudo systemctl status apache2
    ```

3. **Place your HTML file in Apache's directory:**
    ```bash
    sudo cp poem.html /var/www/html/
    ```

Open your web browser and navigate to `http://localhost/poem.html` to see the poem.

### Docker Deployment with Apache

#### Create Dockerfile

Create a Dockerfile in your project directory and add the following content:

```Dockerfile
FROM httpd:2.4
COPY ./poem.html /usr/local/apache2/htdocs/poem.html

This tells Docker to use the official Apache 2.4 image and copies the poem.html file into Apache's HTML directory inside the container.

#### Create HTML file
