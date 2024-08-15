# AmneziaWG-Docker-Compose
Docker Compose to deploy AmneziaWG services


## Deploying
```bash
git clone https://github.com/metya/AmneziaWG-Docker-Compose
cd AmneziaWG-Docker-Compose
chmod -R 775 server_scripts
docker compose up -d
```
When you add your server to AmneziaWG app you need to be able to run `sudo` from your user on the server. When doing so, `sudo` must be without a password. You can do it like that:

```bash
sudo visudo
```

Add `$user ALL=(ALL) NOPASSWD:ALL` line to that file, where `$user` is the name of your user, and save.
