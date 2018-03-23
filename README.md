# Machine Learning

Support materials for Jupiter notebooks and Machine Learning

# Docker

We will be using the Jupyter Notebook from https://github.com/jupyter/docker-stacks using this image from Docker Hub:

> https://hub.docker.com/r/jupyter/datascience-notebook/

In order to run it, open your command line and run the container:

```
docker run -it --rm -v /<local_path_to_be_mapped>/<ipython-project>/:/home/jovyan/work -p 8888:8888 jupyter/datascience-notebook
```

The container will start and the command line will prompt something similar to:

```
Container must be run with group root to update passwd file
Executing the command: jupyter notebook
[I 10:51:22.607 NotebookApp] Writing notebook server cookie secret to /home/jovyan/.local/share/jupyter/runtime/notebook_cookie_secret
[W 10:51:23.164 NotebookApp] WARNING: The notebook server is listening on all IP addresses and not using encryption. This is not recommended.
[I 10:51:23.213 NotebookApp] JupyterLab beta preview extension loaded from /opt/conda/lib/python3.6/site-packages/jupyterlab
[I 10:51:23.214 NotebookApp] JupyterLab application directory is /opt/conda/share/jupyter/lab
[I 10:51:23.229 NotebookApp] Serving notebooks from local directory: /home/jovyan
[I 10:51:23.229 NotebookApp] 0 active kernels
[I 10:51:23.229 NotebookApp] The Jupyter Notebook is running at:
[I 10:51:23.230 NotebookApp] http://[all ip addresses on your system]:8888/?token=a80467a5585008cf82d894e1e2519a244eef4948c2651d66
[I 10:51:23.230 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 10:51:23.231 NotebookApp]

    Copy/paste this URL into your browser when you connect for the first time,
    to login with a token:
        http://localhost:8888/?token=a80467a5585008cf82d894e1e2519a244eef4948c2651d66
```

As the message says, Copy the URL displayed at the end, and paste it in your browser:


> http://localhost:8888/?token=a80467a5585008cf82d894e1e2519a244eef4948c2651d66
