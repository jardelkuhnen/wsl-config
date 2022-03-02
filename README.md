# wsl-config


### 1. WSL Instalation
On the internet has, many tutorials that, can help you on installation. 
Above some links that can help you in this journey:
- https://docs.microsoft.com/pt-br/windows/wsl/install
- https://linuxhint.com/install_ubuntu_windows_10_wsl/

> After wsl is working you can check the instalation and the distros available using the following command: 
`wsl --list`

### 2. Configure wsl Memory usage:
Go to users directory, some cases like `c:/users/user.name/` and create a file called `.wslconfig`
In this file put the follot text to set the memory: 

```
[wsl2]
memory=3GB   # Limits VM memory in WSL 2 up to 3GB
```

### 3. Docker instalation
You can install docker using the engine for your wsl distro selected. 
Above the link of docker that help you on installation: 
- https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

### 4. Running Docker
When start the wsl, you need to run the commands below, to start, and check the status of Docker engine: 
- sudo service docker start
- sudo service docker status

### 5. Start a docker container
- docker run --name mynginx1 -p 80:80 -d nginx
