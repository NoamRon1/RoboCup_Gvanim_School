# Connecting to the Raspberry Pi

> **Note:** This guide assumes that your Raspberry Pi is already connected to the network and that you know its IP address.

---

## Terminal-Based Connection via SSH

To establish a terminal-based connection to your Raspberry Pi using SSH, follow these steps:

1. Open a terminal on your computer.
2. Run the following command, ensuring that your computer is on the same network as the Raspberry Pi:
   ```bash
   ssh admin@<Raspberry-Pi-IP-Address>
   ```
3. Enter the password for the user (`admin` in this example).

> **Note:** The `admin` user in this example is a custom user with root access.

---

## Code-Based Connection via SSH in Visual Studio Code

To connect to your Raspberry Pi using Visual Studio Code and SSH:

1. Open Visual Studio Code.
2. Install the [Remote - SSH extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh).
3. Click on the **Remote Explorer** icon in the bottom-left corner of the VS Code window.
4. Select **Connect to Host** → **Add New SSH Host**.
5. Enter the following command:
   ```bash
   ssh admin@<Raspberry-Pi-IP-Address>
   ```
6. Enter the password for the user (`admin` in this example).

> **Note:** The `admin` user in this example is a custom user with root access.

---

## Connecting via Raspberry Connect

> **Note:** This section is still under development.

---

# Working with Docker Containers

## Building the Container

To build the Docker container:

1. Navigate to the directory containing the Dockerfile: <still don't work do not run this>
   ```bash
   cd /home/admin/ros2/
   ```
2. Build the container:
   ```bash
   docker build .
   ```
3. Run the container using Docker Compose:
   ```bash
   docker compose run <press Tab to autocomplete the container name>
   ```

> **Note:** This section is still a work in progress.

---

## Running the Container

To start the container after the initial setup:

```bash
docker start <press Tab to autocomplete the container name>
```

> **Tip:** If you have the Docker extension installed in Visual Studio Code, you can start the container directly from the extension.

---

## Accessing a Running Container

To access a running container:

```bash
docker exec -it <press Tab to autocomplete the container name> bash
```

---

# File System

> **Note:** This section is currently under development.