# Labspace - Container Getting Started

Learn Docker fundamentals by running containers, exploring the container lifecycle, and packaging a real Node.js app into your own custom image.

## What You'll Do

- Run your first container
- Build your first container image
- Run that newly created container image
- Push the new image to Docker Hub to share with others

## Launch the Labspace

To launch the Labspace, run the following command:

```bash
docker compose -f oci://dockersamples/labspace-container-getting-started up -d
```

And then open your browser to http://localhost:3030.

### Using the Docker Desktop extension

If you have the Labspace extension installed (`docker extension install dockersamples/labspace-extension` if not), you can also [click this link](https://open.docker.com/dashboard/extension-tab?extensionId=dockersamples/labspace-extension&location=dockersamples/labspace-container-getting-started&title=Container%20getting%20started) to launch the Labspace.

## Contributing

If you find something wrong or something that needs to be updated, feel free to submit a PR. If you want to make a larger change, feel free to fork the repo into your own repository.

**Important note:** If you fork it, you will need to update the GHA workflow to point to your own Hub repo.

1. Clone this repo

2. Start the Labspace in content development mode:

    ```bash
    # On Mac/Linux
    CONTENT_PATH=$PWD docker compose up --watch

    # On Windows with PowerShell
    $Env:CONTENT_PATH = (Get-Location).Path; docker compose up --watch
    ```

3. Open the Labspace at http://dockerlabs.xyz.

4. Make the necessary changes and validate they appear as you expect in the Labspace

    Be sure to check out the [docs](https://github.com/dockersamples/labspace-infra/tree/main/docs) for additional information and guidelines.
