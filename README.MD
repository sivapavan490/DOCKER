 # Docker installation steps
 # 1st take the root user access. TO take root user acess run below cmd

    sudo su 
 
 # now run the below cmds to install docker
 
    yum install -y yum-utils
 
 # now ou can add the repos of docker

    yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

# now install docker engine

    yum install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# to start docker

    systemctl start docker

# enabling docker

    systemctl enable docker

# status docker

    systemctl status docker

# docker users can only use docker, when you install docker  a group called "docker" is automatically created

    usermod -aG docker centos


# docker compose installation

    sudo curl -L https://github.com/docker/compose/releases/download/2.29.1/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose

# execution acess
    sudo chmod +x /usr/local/bin/docker-compose

