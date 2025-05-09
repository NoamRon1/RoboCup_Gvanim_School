# How to use the raspberry pi running ros2 on docker

---
## connect to the raspberry pi 
> **Note:** This guide assumes that your raspberry-pi is already connected to the network, and you know the IP address of the Raspberry Pi.

### To get into a terminal based connection via SSH
Run this command to connect. **Be sure that you are on the same network**
``` bash
ssh admin@<Raspberry-pi IP address>
```
Then enter the password of the user (admin in my case).

> **Note:** the admin in the command is a user I created with root accsses.

### To get into a code based connection via SSH and vsCode
1. Open Visual Studio Code and install the SSH extension in [this link](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh).
2. Click on Remote control logo in the down-left corner of the window.
3. Click on "Connect to Host" &rarr; "Add New SSH Host".
4. Then Enter:
    ``` bash
   ssh admin@<Raspberry-pi IP address>
    ```
5. Then enter the password of the user (admin in my case).
> **Note:** the admin in the command is a user I created with root accsses.

### To get into the raspberry-pi using raspberry connect
> **Still in progress.**

---
## The container
### Building the container
To build the container we need to move to directory of the docker-file and build it there

``` bash
cd /home/admin/ros2/ !!!!STILL IN PROGRESS!!!!
docker build .
docker compose run <press tab to fill name>
```

### Running the container
To start the container (after the first installation)
``` bash
docker start <press tab to fill name>
```
> If you have the docker extension you can run it through there.

### Entering a running container
To enter a running container (after you started it)
``` bash
docker exec -it <press tab to fill name> bash
```

---
## The file system