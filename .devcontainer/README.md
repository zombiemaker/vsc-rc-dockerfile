# Configuring Visual Studio Code Development Container

See https://aka.ms/vscode-remote/devcontainer.json for reference on syntax and capabilities.

This .devcontainer.json configuration:
* creates a containerfs directory in the project directory if none exists
* copies the .bashrc file is copied into the containerfs directory
* maps the Linux container user home directory (/home/me) to this project's folder containerfs directory.  
* executes the scripts located in the scripts sub-directory
* exposes container port 8080 to a random container host port (view the boot up log to see which host port is used)

Configuration options:
* Modify the scripts in the script directory if you want to change what occurs during the startup process
* Modify the .bashrc file if you want the bash shell to be configured differently

## Information Resources

* [Visual Studio Code Remote Development](https://code.visualstudio.com/docs/remote/remote-overview)
* [Visual Studio Code devcontainer.json Syntax Reference](https://code.visualstudio.com/docs/remote/devcontainerjson-reference)
* [Dockerfile Syntax Reference](https://docs.docker.com/engine/reference/)