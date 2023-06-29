# Geoserver for climATe Maps

## Installation

Follow the instructions in the [Geoserver Docker repository](https://github.com/geoserver/docker) to install the Geoserver.
The following files and directories needed to be added to the root directory of the Geoserver installation:

- `geoserver_data/`: Contains the data for the Geoserver.
- `additional_libs/`: Contains additional libraries needed for the Geoserver.
- `additional_fonts/`: Contains additional fonts needed for the Geoserver.
- `docker-compose.yml`
- `Dockerfile`
- `install-extensions.sh`
- `startup.sh`

It's also possible to simply clone the following repository into the root directory of the Geoserver installation:
`git@github.com:geoserver/docker.git`, which is the official Geoserver Docker repository.

Afterwards, the Geoserver container can be started with the following command:
`docker-compose build --no-cache && docker-compose up -d`

## Usage

The Apache Tomcat server is running on port 80. The Geoserver can be accessed via `http://localhost:8080/geoserver/web`.

## Documentation

[Documentation](https://docs.geoserver.org/)
[Getting started](https://docs.geoserver.org/latest/en/user/gettingstarted/index.html#getting-started)
[Uploading shapefiles](https://docs.geoserver.org/latest/en/user/gettingstarted/shapefile-quickstart/index.html)
[Uploading GeoTIFFs](https://docs.geoserver.org/latest/en/user/gettingstarted/image-quickstart/index.html)
