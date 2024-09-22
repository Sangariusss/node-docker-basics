# Node Docker Basics

## Table of Contents

- [Overview](#overview)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Contributions](#contributions)
- [License](#license)

## Overview

This project demonstrates how to set up a simple Node.js server in a Docker container, using Docker Compose for orchestration, and Nginx for proxying and serving static files. The Node.js server returns "Hello World!" on the `/hello` endpoint, and Nginx handles traffic proxying and serves static assets.

### Features

- **Node.js Server**: A simple server that responds to GET requests at the `/hello` endpoint with "Hello World!".
- **Nginx**: Serves static files and proxies requests to the Node.js backend.
- **Docker**: The project is fully containerized with Docker and uses Docker Compose to orchestrate the services.

## Usage

### Setup and Deployment

1. **Install Docker and Docker Compose**: Ensure Docker and Docker Compose are installed on your system.

2. **Clone the Repository**:
    ```bash
    git clone <repository-url>
    cd node-docker-basics
    ```

3. **Run the Application**:
    - Start the services using Docker Compose:
      ```bash
      docker-compose up
      ```

4. **Access the Application**:
    - Visit `http://localhost` in your browser to access the static files served by Nginx.
    - Visit `http://localhost/hello` to get the "Hello World!" response from the Node.js server.

## File Structure

- **html/**: Contains the static HTML files served by Nginx.
    - `404.html`: Custom 404 error page.

- **nginx/**: Nginx configuration folder.
    - `nginx.conf`: Configuration file for setting up Nginx proxying and static file serving.

- **static/**: Static assets like images or icons.
    - `favicon.svg`: Favicon for the application.

- **.dockerignore**: Specifies files and directories to ignore in Docker builds.

- **.gitignore**: Specifies files and directories to ignore in Git.

- **app.js**: The main Node.js application file.

- **docker-compose.yml**: Docker Compose file defining services for Node.js and Nginx.

- **Dockerfile**: Instructions for building the Docker image for the Node.js application.

- **LICENSE**: The project license (if applicable).

- **package.json**: Node.js dependencies and project metadata.

- **README.md**: Project documentation.

## Contributions

Contributions, feedback, and suggestions are welcome. Feel free to submit a pull request or open an issue if you have any improvements or find issues.

## License

This project is licensed under the ISC License. See the [LICENSE](LICENSE) file for details.
