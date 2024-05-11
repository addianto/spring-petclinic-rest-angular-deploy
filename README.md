# Spring Petclinic REST & Angular Deployment

> Explore container-based deployment strategies for Spring Petclinic REST & Angular.

## Setup

Clone the frontend repository to a folder named `frontend` in the same level as the project:

```shell
git clone -b chore/deploy-nginx-unprivileged https://github.com/addianto/spring-petclinic-angular.git frontend
```

Ensure the `frontend` is ignored by the existing [`.gitignore`](./gitignore) file to avoid adding the frontend repository as Git submodule:

```shell
cat .gitignore
```

> The output should show a line that contains `frontend/`.
> If not, please add it manually.

## Docker Compose

```shell
docker compose up --detach
```

> Explanation: `--detach` is used to run the containers in background mode.
> It means that the containers will continue running even if you terminate your shell.
