# Installing Docker for Windows

If you are a Windows Home user, you will not be able install the Docker for Windows Desktop edition, as it requires Hyper-V virtualization. This is supported only by Windows Professional and Enterprise editions.

If you want to install Docker in your windows system, I would recommend following the Docker Toolbox approach, as Hyper-V directly conflicts with VMWare Workstation and VirtualBox.

**Windows Home users will need to install Docker Toolbox** which uses VirtualBox instead.

Docs and setup info available here:
https://docs.docker.com/toolbox/toolbox_install_windows/

Release downloads available here:
https://github.com/docker/toolbox/releases

Toolbox will install everything you need including VirtualBox.

You may also need to enable virtualization in your computer's BIOS settings. This will be different for each manufacturer, please refer to their documentation on which keys to use to access these settings on reboot.

After Toolbox is finished installing, open the Docker Quickstart Terminal. This will complete the setup and provision your VirtualBox machine.

**Check your install:**

In the Docker QuickStart terminal

```
docker run hello-world
```

This should pull down the test container and print hello-world to your screen.

***Note\***

A major difference between the course lecture using Docker Desktop vs. Docker Toolbox is that you will not be able to use localhost anymore.

Instead, you will need to access your machine with the IP address **192.168.99.100**