# Installation
## Installation Guide for cestmaddy with Docker

Download [the default configuration](https://git.cestoliv.com/attachments/9b2db2dd-e722-4333-9557-003c46ec0ed5) and unzip it :

Here are the commands to do it from the shell:
```bash
# Download the zip
wget "https://git.cestoliv.com/attachments/9b2db2dd-e722-4333-9557-003c46ec0ed5" -O docker_default_config.zip
# Extract the zip
unzip docker_default_config.zip && mv docker_default_config cestmaddy && rm docker_default_config.zip
# Go to the new directory
cd cestmaddy
```

Modify the .zip file to match your expectations
## .env
    PORT=8629
    TZ=Europe/Paris

- **PORT**: The listening port of the cestmaddy server
- **TZ**: The timezone of your server

And finally start **cestmaddy** with the following command :

```bash
docker-compose up -d
```

If everything went well, **cestmaddy** will compile the sources and then launch the web server, go to `http://localhost:PORT`, you should see this :

![cestmaddy post-installation page](/documentation/installation/imgs/post-installation-page.png)

### What's next?
What's next? We'll have to configure all this! See you on the [configuration](/documentation/configuration)!