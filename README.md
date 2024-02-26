# WordPress Compose

This repository contains the necessary files to deploy a WordPress website using Docker Compose.

## Description

WordPress Compose simplifies the process of setting up a WordPress website by using Docker Compose. It includes a pre-configured environment with WordPress, MySQL, and PHP for easy deployment.

## Prerequisites

Before getting started, ensure you have Docker and Docker Compose installed on your system.

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## Installation and Usage

To deploy the site, run the following command:

```bash
docker-compose up -d
```

This will start the necessary containers in the background.

### Removing and Redeploying

If you need to remove the data and redeploy the site, you can use the following command:

```bash
docker-compose down && rm -vfr data && docker-compose up -d
```

This will stop the containers, delete the data, and redeploy the site.

### Stopping Without Deleting Data

To simply stop the containers without deleting the data, use:

```bash
docker-compose down
```

### Restarting

To restart the site, you can use the following command, which stops and starts the containers:

```bash
docker-compose down && docker-compose up -d
```

## Customization

You can customize the WordPress setup by modifying the `docker-compose.yml` file according to your requirements. Feel free to add plugins, themes, or make configuration changes.

## Accessing the Site

Once the containers are running, you can access the WordPress site in your web browser at `http://localhost`.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Acknowledgements

- This project is inspired by the need for a simple and portable WordPress deployment solution.
- Thanks to the Docker and WordPress communities for their amazing work and contributions.

---
