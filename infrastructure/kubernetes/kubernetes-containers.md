# Containers

## Docker

- [The Docker Handbook](https://www.freecodecamp.org/news/the-docker-handbook/)
- [Back to Basics: Top Useful Docker Commands](https://adamtheautomator.com/back-to-basics-top-useful-docker-commands/)
- [dockerd configuration file](https://docs.docker.com/engine/reference/commandline/dockerd/)
- [Install Docker compose](https://docs.docker.com/compose/install/)
- [Manage data in Docker](https://docs.docker.com/engine/admin/volumes/)
- [The base command for the Docker CLI](https://docs.docker.com/engine/reference/commandline/docker/)
- [Easily Host an Awesome Docker Registry at Home](https://medium.com/@lukebenson/easily-host-an-awesome-docker-registry-at-home-694a9c70740f)

`/mnt/registry:/var/lib/registry`

- [Deploy a registry server](https://docs.docker.com/registry/deploying/)
- [Test an insecure registry](https://docs.docker.com/registry/insecure/)
- [How to get a list of images on docker registry v2](https://stackoverflow.com/questions/31251356/how-to-get-a-list-of-images-on-docker-registry-v2)

```http
https://myregistry:5012/v2/_catalog
https://myregistry:5012/v2/ubuntu/tags/list
```

- [Using a (in)secure registry with Synology Docker](https://lenain.info/using-a-in-secure-registry-with-synology-docker/)
- [Create a service which creates an NFS volume](https://docs.docker.com/storage/volumes/#create-a-service-which-creates-an-nfs-volume)
- [Docker Swarm Persistent Storage with NFS](https://sysadmins.co.za/docker-swarm-persistent-storage-with-nfs/)
- [Netshare by ContainX](http://netshare.containx.io/docs/getting-started) and [github repository](https://github.com/ContainX/docker-volume-netshare)
- [How To Mount An NFS Share Into A Container](https://anto.online/guides/how-to-mount-an-nfs-share-into-a-container/)
- [Docker volumes: how to create and get started](https://phoenixnap.com/kb/docker-volumes)

```bash
docker volume create --name [name] --opt type=nfs --opt device=:/volume1/[name] --opt o=addr=nasserver.domain.com
docker run -it --rm --name=[containername] --mount source=[name],destination=/test ubuntu
```

- [How to Run GUI Applications in a Docker Container](https://www.cloudsavvyit.com/10520/how-to-run-gui-applications-in-a-docker-container/)
- [7 Docker Anti-Patterns You Need to Avoid](https://www.cloudsavvyit.com/14343/7-docker-anti-patterns-you-need-to-avoid/)
- [How to Assign a Static IP to a Docker Container](https://www.cloudsavvyit.com/14508/how-to-assign-a-static-ip-to-a-docker-container/)

### Build

- [Using Makefiles to build and publish (docker) containers](https://dev.to/flpslv/using-makefiles-to-build-and-publish-docker-containers-7c8)

### Compose

- [Install Compose](https://docs.docker.com/compose/install/)
- [Compose file version 3 reference](https://docs.docker.com/compose/compose-file/)

## Portainer

- [Set up a new Portainer Server installation](https://docs.portainer.io/v/be-2.7/start/install/server)

## Linux

- Install Docker on Linux:

```bash
apt-get update
wget -qO- https://get.docker.com | sh
```

- Add loggedin user to docker group:

```bash
sudo gpasswd -a $USER docker
```

  re-login with new group membership:

```bash
newgrp docker
```

### Powershell Containers

- [Using Azure PowerShell in Docker](https://docs.microsoft.com/en-us/powershell/azure/azureps-in-docker?view=azps-6.4.0)
- [PowerShell by Microsoft](https://hub.docker.com/_/microsoft-powershell)
- [Run Azure PowerShell in a Docker Container](https://www.thomasmaurer.ch/2020/03/run-azure-powershell-in-a-docker-container/)
- [Azure-PowerShell by Microsoft](https://hub.docker.com/_/microsoft-azure-powershell)

## Rancher

- [Watch How To Replace Docker With nerdctl And Rancher Desktop](https://youtu.be/evWPib0iNgY)

## Windows

- [Install Docker on Windows Server 2019](https://www.ntweekly.com/2018/11/03/install-docker-on-windows-server-2019/)
- [What's new for Docker on Windows Server 2019?](https://stefanscherer.github.io/docker-on-windows-server-2019/)
- [Pull WindowsServerCore Container Image](https://hub.docker.com/r/microsoft/windowsservercore/)
- [Linux Containers on Windows](https://docs.microsoft.com/en-us/virtualization/windowscontainers/deploy-containers/linux-containers)
- [Setup Docker on Windows Server 2016](https://blogs.technet.microsoft.com/canitpro/2016/10/26/step-by-step-setup-docker-on-your-windows-2016-server/)
- [Windows Containers Documentation](https://docs.microsoft.com/en-us/virtualization/windowscontainers/)

## Videos

- Containers? So What? Docker 101 Explained - Computer Stuff They Didn't Teach You #8

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/0oEsMwSxBsk/default.jpg)](https://www.youtube.com/watch?v=0oEsMwSxBsk)
