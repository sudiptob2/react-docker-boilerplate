# React Docker Boilerplate
This is a react + docker boilerplate which solves `node_modules` sync related issues while developing React application with `docker`. A detailed explanation can be found [here](https://medium.com/@sudiptob2/properly-setting-up-react-development-environment-using-docker-a2de46464d0b).

![banner](.temp/banner.png)

## Setup and Usage

Pull the source code

```bash
git clone [url]
```

If pulled for the first time or the package.json changed run

```bash 
docker compose build
```

Starting the environment in background
```bash
docker compose up -d
```

To see the logs of your app

```bash
docker compose logs -f react
```

If you need to install any npm package.

```bash
docker compose exec react npm install <pacakge-name>
```
To run any NPM command

```bash
docker-compose exec react <npm-command>
```

stop the containers

```bash
docker compose down
```

# For Any support
Please raise an issue.  Also you can contact me @ [twitter](https://twitter.com/sudiptob2) | [Linkedin](https://www.linkedin.com/in/sudiptob2/)