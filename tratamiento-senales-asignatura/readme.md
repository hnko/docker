# TSV
This docker is created for the tratamiento de senales de video subject of the Universidad Autonoma de Madrid.

## Dockerfile
We start from jupyter/minimal-notebook image and install the packages required for the future practices. All the packages can be found in the requirement.txt

## Build an image
```docker build -t tsv-image . ```

## Create a container
```docker run --rm -it -p 8888:8888 -v $(pwd):/home/jovyan/tsv tsv-image ```

* if you want to have jupyterLab add "JUPYTER_ENABLE_LAB=yes"

    ```docker run --rm -it -p 8888:8888 -v $(pwd):/home/jovyan/tsv JUPYTER_ENABLE_LAB=yes tsv-image ```