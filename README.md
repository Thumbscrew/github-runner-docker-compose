# Github Runner Docker Compose
Docker Compose file for a Github Runner (Docker image created by tcardonne - see [https://hub.docker.com/r/tcardonne/github-runner](https://hub.docker.com/r/tcardonne/github-runner))

## Steps

1. Clone the repository

```bash
git clone https://github.com/Thumbscrew/github-runner-docker-compose.git
cd github-runner-docker-compose
```

2. Create a copy of [.env.example](.env.example)

```bash
cp .env.example .env
```

3. Create your runner in your repository settings (**Settings -> Actions -> Runners -> New self-hosted runner**)

4. Copy the token and set the `RUNNER_REPOSITORY` and `RUNNER_TOKEN` in the `.env` file

5. Bring up the containers!

```bash
sudo docker-compose -p github_runner up -d
```