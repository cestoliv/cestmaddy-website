# Installation
## Installation Guide for cestmaddy under Debian

First of all, make sure you have an up to date system ;)

### Dependencies
The **cestmaddy** dependencies are as follows:
- git
- nodejs
- npm
- imagemagick

### Downloading
You will then need to download the latest version of **cestmaddy** from our repository.
To do so, use the following command:
```bash
git clone https://git.cestoliv.com/cestoliv/cestmaddy.git
```

### First start
Then go to the **cestmaddy** directory created by `git` :
```bash
cd cestmaddy
```
Then install the dependencies via the `npm` dependency manager:
```bash
npm install
```
   
Then move the default files (or create your own directly if you are an expert) :
```bash
cp res/deployment/default/config.yml config.yml
cp -r res/deployment/default/source source/
cp -r res/deployment/default/custom custom/
```

And finally start **cestmaddy** with the following command :
```bash
npm start
```

If everything went well, **cestmaddy** will compile the sources and then launch the web server, go to `http://localhost:8625`, you should see this :

![cestmaddy post-installation page](/documentation/installation/imgs/post-installation-page.png)

### What's next?
What's next? We'll have to configure all this! See you on the [configuration](/documentation/configuration)!