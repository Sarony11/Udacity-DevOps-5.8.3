# Exercise: Containerize an App #

Containers are a powerful mechanism to reuse code from experts. Test your knowledge of the power of containers in the following exercise by building a container and containerizing an app from scratch!
Instructions

    Create an empty Dockerfile using the touch command
    Use the FROM command and reference the latest version of Python here.
    Include the "Hello World" Flask example as an app within your container
        Copy any relevant directories and libraries in the Dockerfile
        Make sure any relevant requirements are installed in the Dockerfile
        Expose the port from the Flask example oin the Dockerfile - make sure you check which one is used by the example!
        Have your Dockerfile run the relevant commands for your app
    Build your container
    Run the container, opening up a bash shell
    Verify the correct version of Python is installed: python --version

## Tips ##

Below are potential options for building and running your container.

- To build your container, if tagging your container as my-python-app:
> $ docker build -t my-python-app .

- To run the container, given my-python-app as the image tag and my-running-app as the container name:
> $ docker run -it --rm --name my-running-app my-python-app

