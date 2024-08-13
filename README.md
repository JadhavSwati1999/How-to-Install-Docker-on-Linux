# How-to-Install-Docker-on-Linux
How to Install Docker on Linux
To install docker follow the below-mentioned steps:

- Launch an instance with basic configuration.


- Connect to the instance.


### Set up the repository

Install the `yum-utils` package (which provides the `yum-config-manager` utility) and set up the repository.

`$ sudo yum install -y yum-utils
$ sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo`



### Install Docker Engine

1. Install Docker Engine, containerd, and Docker Compose:
    
    Latest Specific version
    
    ---
    
    To install the latest version, run:
    
    `$ sudo yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin`
    
    This command installs Docker, but it doesn't start Docker. It also creates a `docker` group, however, it doesn't add any users to the group by default.
    
    - To install docker
    
    `$ sudo yum install docker -y`
    



Start Docker.

`$ sudo systemctl start docker`

You have now successfully installed and started Docker Engine.

---
