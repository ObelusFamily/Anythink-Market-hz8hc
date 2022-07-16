# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

### Machine requirement

* Make sure the Docker is installed on the machine. See [link](https://docs.docker.com/get-docker/) on how to install.

### Setup

1. Open a terminal

2. Verify the docker is ready by running follow commands in terminal

    ```bash
      docker -v
      docker-compose -v
    ```

    Expect to see the docker version and docker compose version in the output.

3. In terminal, navigate to the root directory of this project

4. Execute following command to start the project in docker.

    ```bash
      docker-compose up
    ```

    Once docker finishes downloading the image and starting the containers.

5. Enter following url in the browser to verify the project is running. `http://localhost:3000/api/ping`

    You should see response with json data. A message includes "Pong".

6. Go to registration link http://localhost:3001/register to register a new user. To verify other componetns in the backend is running properly.

Now the project should be ready for development.
