# Admin

## Overview
This repository contains the source code MOSIP Admin module. For an overview refer [here](https://docs.mosip.io/1.2.0/modules/administration). The module exposes API endpoints. For a reference front-end UI implementation refer to [Admin UI github repo](https://github.com/mosip/admin-ui/)

Admin module contains following services:
1. Admin Service
2. Masterdata Service
3. Sync Data Service
4. Hotlist Service

## Databases
Refer to [SQL scripts](db_scripts).

## Build & run (for developers)
The project requires JDK 1.11. 
1. Build and install:
    ```
    $ cd kernel
    $ mvn install -DskipTests=true -Dmaven.javadoc.skip=true -Dgpg.skip=true
    ```
1. Build Docker for a service:
    ```
    $ cd <service folder>
    $ docker build -f Dockerfile
    ```

## Deploy
To deploy Admin on Kubernetes cluster using Dockers refer to [Sandbox Deployment](https://docs.mosip.io/1.2.0/deployment/sandbox-deployment).

## Test
Automated functional tests available in [Functional Tests repo](https://github.com/mosip/mosip-functional-tests).

## APIs
API documentation is available [here](https://mosip.github.io/documentation/).

## License
This project is licensed under the terms of [Mozilla Public License 2.0](LICENSE).

