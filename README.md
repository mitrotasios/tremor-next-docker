### Description
This repository enables users to run an isolated environment within a Docker container using an
**linux alpine**  base image.

The repository is cloned from the official [next.js GitHub repository](https://github.com/vercel/next.js/tree/canary/examples/with-docker). The `@tremor/react` npm package has been added as adependency on top and an example Tremor Block has been added the the `pages/index.js` file.

### Prerequisites
1. Clone this repository
2. [Install docker](https://docs.docker.com/get-docker/) on your machine

### Running the application
1. Run `npm install`
2. Build the docker image:
```
docker build -t tremor-alpine .
```
3. Run the docker container:
```
docker run -p 3000:3000 tremor-alpine
```
4. Open your browser at `http://localhost:3000/`
