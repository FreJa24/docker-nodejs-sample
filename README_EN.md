# ToDo Application

A simple ToDo application built with Node.js.

DE [Deutsche Version](README_DE.md)

## Requirements

To run this project locally, you need:

- [Node.js](https://nodejs.org) (including npm)
- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/)

## Clone the repository

Clone the repository using the following command:

```bash
git clone https://github.com/FreJa24/docker-nodejs-sample
cd docker-nodejs-sample
```

## Install packages

Install the required Node.js dependencies:

```bash
npm install
```

## Start the application locally

Start the application in development mode with:

```bash
npm run dev
```

The application will then be available at:

**[http://localhost:3000](http://localhost:3000)**

## Build the Docker image

Build the Docker image with the following command:

```bash
docker build -t todo-app .
```

## Run the application with Docker

Start a container from the image:

```bash
docker run --name todo-container -p 3000:3000 todo-app
```

The application will then be available at [http://localhost:3000](http://localhost:3000).

## Run the application with Docker Compose

Start the application with Docker Compose:

```bash
docker compose up --build
```

Or in the background (detached):

```bash
docker compose up -d --build
```

## Stop the application

Stop and remove the container:

```bash
docker stop todo-container
docker rm todo-container
```

Or if started with Docker Compose:

```bash
docker compose down
```
