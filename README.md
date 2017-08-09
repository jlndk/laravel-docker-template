# Laravel Docker Template

A multi-stage, production-ready docker template for Laravel applications.
Plays well with continuous integration pipelines.

## Features
- Production-ready
- Optimised for build time &amp; size
- OPCache optimised for immutable environment
- phpredis for blazing-fast Redis (be sure to change client to `phpredis` in your `config/database.php` file)
- Frontend webpack asset compiling
- Backend composer requirements
- Ready to ship to a production cluster

## Requirements
- Docker version `>=17.05` (for multi-stage builds)

## How to use
1. Copy the `Dockerfile`, `.docker` folder and `.dockerignore` into your project
2. Edit the configuration files as necessary (php extensions, different npm build command etc.)
3. Run `docker build .` and ship the image!
