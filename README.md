Introduction to PyTorch: materials for the reading group presentation

# Getting started
To follow the tutorial exercises, you are going to need a laptop with Miniconda (a minimal version of Anaconda) and several Python packages installed.

## Download and install Miniconda
Please go to the [Anaconda website](https://conda.io/miniconda.html).
Download and install *the latest* Miniconda version for *Python* 3.6 for your operating system.

```bash
wget <http:// link to miniconda>
sh <miniconda .sh>
```

After that, type:
```bash
conda --help
```
and read the manual.

## Check-out the git repository with the exercise
Once Miniconda is ready, checkout the tutorial repo and proceed with setting up the environment:
```bash
git clone https://github.com/ASvyatkovskiy/pytorch-intro
```

## Create isolated Miniconda environment
Change into the course folder, then type:

```bash
#cd pytorch-intro
conda env create -f environment.yml
source activate hello-pytorch
```

## Enable anaconda kernel in Jupyter
To make newly created miniconda environment visible in the Jupyter, you might need to install `ipykernel`:

```bash
#source activate hello-pytorch
python -m ipykernel install --user --name hello-pytorch --display-name "Hello, PyTorch"
```

## Start jupyter notebook
If working on a laptop, start from terminal as usual:

```bash
jupyter notebook
```
In the upper rigt corner, check that you are indeed using the "Hello, PyTorch" kernel. If not, change to it from the dropdown menu under "Kernels"
