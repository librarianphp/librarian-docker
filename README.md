# Librarian
Librarian is a stateless CMS based on static files. It uses the same format as DEV.to for markdown files with a front matter and liquid tags for custom functionality.

# Docker Setup

The setup included in this repository can be used with Docker + Docker Compose to create a local development environment powered by containers.

## How to Use It
You can download the files in this repository and save them in the root folder of your Librarian application. You may or may not want to include the files in version control - it can be helpful if other people will be working on your project.

Once the files are in place, you can get the environment up and running with:

```shell
docker-compose up -d
```

This will run the containers in background.

To execute commands such as `composer install`, run:

```shell
docker-compose exec app composer install
```

Running NPM:

```shell
docker-compose exec app npm install
```

Compiling css assets:

```shell
docker-compose exec app npm run dev
```

Stopping the environment:

```shell
docker-compose stop
```

Re-starting the environment:

```shell
docker-compose start
```

Destroying the environment:

```shell
docker-compose down
```