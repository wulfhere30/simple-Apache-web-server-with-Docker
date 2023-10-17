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

### Docker Deployment with 

## License

This project is distributed under the MIT License. See `LICENSE` file for more details.
