# Node-red + MongoDB Docker

## Basic Usage:
- Install docker & docker-compose
- set the permissions on the data & public folders (linux)
  ```
    chmod -R a+rw data && chmod -R a+rw public
  ```
- Run  `docker-compose up` in the repo root

## Default Configuration:

- The node-red admin dashboard is served from /admin by default
- Configuration files and flows are saved in the data folder
- Files added to the public folder are served from the root directory /
- Node Red Dashboard and MongoDB nodes are installed by default
- The MongoDB server is available on port 27017

## Adding NPM Modules:

- Edit Dockerfile RUN command and append npm modules required
Modify settings.js to enable global npm modules in red

- Run `docker-compose up --force-recreate --build`
