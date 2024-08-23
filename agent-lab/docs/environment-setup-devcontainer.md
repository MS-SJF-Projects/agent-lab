# Using VS Code Dev Containers

The repository includes a [Dev Container](https://code.visualstudio.com/docs/devcontainers/containers) to make provisioning the environment and required dependencies very easy.  
You will need:

- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Dev Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) installed.

## Configure environment variables

Create a `.env` file in the root directory of the repository with these details:

```bash
AZURE_OPENAI_ENDPOINT=https://<your-endpoint>.openai.azure.com/
AZURE_OPENAI_DEPLOYMENT=gpt-4-32k        # or whatever you named your deployment
AZURE_OPENAI_API_KEY=***********
AZURE_OPENAI_API_VERSION=2024-02-01

TIMEZONE=Europe/Berlin
```

## Open code in Dev Container  

Clone the repository & open it with VS Code.

Press `Ctrl` + `Shift` + `P` in VS code:

```text
> Dev Containers: Reopen in Container
```

![Picture of VSCode command palette with command reopen in container](./images/container_command.png 'Reopen in container command')

Wait for the Dev Container to be created.
Once the container is started, the bottom left of your VSCode window will show that the Dev Container is running:

![VSCode window shows running dev container](./images/devcontainer.png 'Dev container is running')

## Open Notebooks

You can simply open and run the [Notebooks](../notebooks/) within VS Code.
