# Example Library Specification
This repository defines a simple API using [OpenAPI v3.0.1](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.1.md).

[![Build Status](https://travis-ci.org/devjack/example-library-specification.svg?branch=master)](https://travis-ci.org/devjack/example-library-specification)

# Setup and installation

The API spec is defined in `openapi.yml`. Each URL has its own endpoint in `endpoints/` and JSON request/response schemas are defined in `schemas/`. JSON Schema is used to define responses and can be used for validation.

## Setup and run the documentation
Run these commands to install npm dependencies and serve the API documentation locally.

```sh
npm install
npm run test
npm run serve
```

The API documentation will be available at [https://localhost:5000](http://localhost:5000).

To resolve and publish the API spec, run:

```sh
npm run resolve
```

A simple HTML document including [ReDoc](https://github.com/Rebilly/ReDoc) is available in the `public/` directory. To copy across the published spec and schemas, run:

```sh
npm run publish
```

You can then serve `/public` from any static content hosting service. The current documentation is hosted on Netlify at [example-library-specification.netlify.com](https://example-library-specification.netlify.com)
