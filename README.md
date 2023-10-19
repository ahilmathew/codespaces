# How to use codespaces configuration in this repo

* Open this repository in VSCode.
* The [GitHub Codespaces](https://marketplace.visualstudio.com/items?itemName=GitHub.codespaces) extension installed in Visual Studio Code
* Open the command palette by pressing Ctrl+Shift+P (Windows/Linux) or Cmd+Shift+P (Mac).
* In the command palette, start typing "Codespaces" and select `Codespaces: Create New Codespace`.
* Select this repository from the list and select the main branch.
* The devcontainer configurations in this repo should now show up. Select the required configuration (`devcontainer.json`).
* Select the instance capacity size.
* Visual Studio Code will now open a new window connecting to the Codespace. This may take a few moments as it creates and configures the environment based on the devcontainer.json file.

# Forwarding a process running in codespaces to your local machine.

If you have an application (example - nodejs express server) running inside codespaces and you want to access the application from your local machine then follow the below steps - 
* Open up the VSCode panel inside codespaces - Press Ctrl+J (Windows/Linux) or Cmd+J (Mac). This keyboard shortcut toggles the visibility of the panel.
* You should be able to see the `Ports` tab.
* You add the port your application is running on to the list. For example 3000
* Now you should be able to access the application on `localhost:3000` from your machine.

You can also add a list of forwarded ports inside the `forwardPorts` array in `devcontainer.json` file. This will ensure that the ports are forwarded when codespaces starts up.

# How do I add VSCode extensions

* Check the `extensions` inside `devcontainer.json`.
* Add the extension id of any vscode extensions you want. Codespaces will have that when you spin it up.

# Limitation

* Cannot run docker containers inside the codespaces created here.