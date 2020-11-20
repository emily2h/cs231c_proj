This is the README.md from the original deep-image-prior repository, with some changes to adapt to this project.

In this project, we are developing a tool to do digital + automatic restoration of paintings and evaluate different methods. You can run through the script in inpainting.ipynb and place your own images of paintings you wish to restore there. 

Links to the github repositories used and papers are included in inpainting.ipynb. 

# Install

Here is the list of libraries you need to install to execute the code:
- python = 3.6
- [pytorch](http://pytorch.org/) = 0.4
- numpy
- scipy
- matplotlib
- scikit-image
- jupyter

All of them can be installed via `conda` (`anaconda`), e.g.
```
conda install jupyter
```


or create an conda env with all dependencies via environment file

```
conda env create -f environment.yml
```

## Docker image

Alternatively, you can use a Docker image that exposes a Jupyter Notebook with all required dependencies. To build this image ensure you have both [docker](https://www.docker.com/) and  [nvidia-docker](https://github.com/NVIDIA/nvidia-docker) installed, then run

```
nvidia-docker build -t deep-image-prior .
```

After the build you can start the container as

```
nvidia-docker run --rm -it --ipc=host -p 8888:8888 deep-image-prior
```

you will be provided an URL through which you can connect to the Jupyter notebook.

## Google Colab

To run it using Google Colab, click [here](https://colab.research.google.com/github/emily2h/cs231c_proj/) and select the inpainting.ipynb notebook to run. 

