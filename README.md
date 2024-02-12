<h1 align="center">CKAN-OGC harvester Cron: A Docker Compose solution for dataset management.</h1>
<p align="center">
<a href="https://github.dev/mjanez/ckan-ogc_worker"><img src="https://img.shields.io/badge/%20ogc_worker-0.0.1-brightgreen" alt="ogc_worker version"></a><a href="https://opensource.org/licenses/MIT"> <img src="https://img.shields.io/badge/license-MIT-brightgreen" alt="License: MIT"></a> <a href="https://github.com/mjanez/ckan-ogc_worker/actions/workflows/docker/badge.svg" alt="License: MIT"></a>


<p align="center">
    <a href="#overview">Overview</a> •
    <a href="#quick-start">Quick start</a> •
    <a href="#test">Test</a> •
    <a href="#debug">Debug</a> •
    <a href="#containers">Containers</a>
</p>

**Requirements**:
* [Docker](https://docs.docker.com/get-docker/)

## Overview
Docker compose environment to manage scalable background harvesting of datasets for development and testing with CKAN Open Data portals.

>**Note**<br>
> It can be easily tested with a CKAN-type Open Data portal deployment: [mjanez/ckan-docker](https://github.com/mjanez/ckan-docker)[^1].

Available components:
* **ogcworker**: Software to 

## Quick start
### With docker compose
Copy the `.env.example` template and configure by changing the `.env` file. Change `PYCSW_URL` and `CKAN_URL`,  as well as the published port `PYCSW_PORT`, if needed.

    ```shell
    cp .env.example .env
    ```


[^1]: A custom installation of Docker Compose with specific extensions for spatial data and [GeoDCAT-AP](https://github.com/SEMICeu/GeoDCAT-AP)/[INSPIRE](https://github.com/INSPIRE-MIF/technical-guidelines) metadata [profiles](https://en.wikipedia.org/wiki/Geospatial_metadata).