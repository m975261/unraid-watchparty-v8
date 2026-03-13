# unraid-watchparty-v8

> Auto-containerized for Unraid 7.0.1 by **TITAN Dockerizer v2.8**
> Source: [https://github.com/howardchung/watchparty](https://github.com/howardchung/watchparty)

## Docker Image
```
docker pull muaeabudhabi/watchparty-v8:latest
```

## Install on Unraid
1. Download `unraid-templates/my-watchparty-v8.xml`
2. Copy to `/boot/config/plugins/dockerMan/templates-user/`
3. Docker tab → Add Container → select `watchparty-v8`

## Auto-Updates
| Workflow | Schedule | Purpose |
|---------|----------|---------|
| `docker-build.yml` | Push / Manual / Dispatch | Builds multi-arch image → DockerHub |
| `upstream-watch.yml` | Daily 02:00 UTC | Checks upstream releases → triggers rebuild |
