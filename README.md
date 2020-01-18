# vscode-remote-docker-host-react
Sample starter project for developing a react app in a container on a remote docker host using VSCode and its Remote Extensions.

# Try Out Development Containers on Remote Docker Hosts: React

This is a sample project that lets you try out the **[VS Code Remote - Containers](https://aka.ms/vscode-remote/containers)** extension in a few easy steps.

> **Note:** If you're following the quick start, you can jump to the [Things to try](#things-to-try) section.

## Setting up the development container

Follow these steps to open this sample in a container on a remote docker host:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started).

2. To use this repository, you can:
   Open the repository in an isolated Docker volume:
    - TBD: Try the Remote-Containers: Open Repository in Container" command

   Or connect to the empty container and clone the repo manually:
    - Clone this repo to your local machine.
    - Edit .devcontainer/devcontainer.json to include your remote docker host's IP and port you'd like to access remotely.
    - Edit .vscode/settings.json to your username and hostname/IP of the remote docker host.
    - Press <kbd>F1</kbd> and select Remote-Containers: Reopen in remote container...
    - In the newly opened terminal of the remote container, clone this repo. You should see the files appear in the project explorer of VSCode. You can now edit and run these files just as you would if they were local.
   

## Things to try

Once you have this sample opened in a container, you'll be able to work with it like you would locally.

> **Note:** This container runs as a non-root user with sudo access by default. Comment out `"remoteUser": "node"` in `.devcontainer/devcontainer.json` if you'd prefer to run as root.

Some things to try:

1. **Edit:**
   - Open `server.js`
   - Try adding some code and check out the language features. Notice that `eslint` and the `vscode-eslint` extension are already installed in the container.
2. **Terminal:** Press <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>\`</kbd> and type `uname` and other Linux commands from the terminal window.
3. **Build, Run, and Debug:**
   - Open `App.js`
   - Add a breakpoint or edit the JSX in render().
   - Run `npm start` in a terminal.
   - Once the breakpoint is hit, try hovering over variables, examining locals, and more.
   - Continue, then open a local browser and go to `http://{ipOfYourRemoteDockerHost}:3000` and note you can connect to the server in the container on the remote host.
4. **Forward another port:**
   - This needs further direction describing the devcontainer.js "runArgs" changes, etc.

## Contributing
TBD

## License
TBD

