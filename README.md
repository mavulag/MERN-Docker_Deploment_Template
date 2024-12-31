# MERN Stack Application with Docker

This repository contains a MERN (MongoDB, Express, React, Node.js) stack application with Docker deployment. The application is designed to be easily deployable using Docker Compose.

## Table of Contents
- [Prerequisites](#prerequisites) - Lists the necessary software to run the project. 
- [Project Structure](#project-structure) - Briefly describes the main parts of the project.
- [Setup Instructions](#setup-instructions) - Includes steps to clone the repository, set up environment variables, and build/run the application using Docker Compose.
  - [Clone the Repository](#clone-the-repository)
  - [Environment Variables](#environment-variables)
  - [Build and Run the Application](#build-and-run-the-application)
- [Usage](#usage) - Provides URLs to access the different parts of the application.
- [Contributing](#contributing) - Mentions that contributions are welcome and points to a contributing guide.
- [License](#license) - Specifies the project's license.

## Prerequisites

Make sure you have the following installed on your local development machine:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Project Structure

The project is divided into three main parts:

- `server`: Contains the Node.js/Express backend code.
- `client`: Contains the React frontend code.
- `docker-compose.yml`: Docker Compose file that defines and runs multi-container Docker applications.

## Setup Instructions

### Clone the Repository

First, clone the repository to your local machine:

```sh
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### Environment Variables

Create a `.env` file in the root directory of the `server` folder and add the following environment variables:

```env
MONGO_URI=mongodb://root:example@mongo:27017/yourdbname?authSource=admin
```

You can adjust the values as needed.

### Build and Run the Application

To build and run the application using Docker Compose, execute the following command from the root directory:

```sh
docker-compose up --build
```

This command will build the Docker images for the server and client and start the services defined in the `docker-compose.yml` file.

## Usage

Once the services are up and running, you can access the application in your web browser:

- React Client: `http://localhost:3000`
- Node.js/Express Server: `http://localhost:5000`
- MongoDB: `mongodb://localhost:27017`

## Contributing

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) to learn how you can contribute.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.