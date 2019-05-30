# GANDissect Tutorial Setup

This tutorial branch of GAN Dissect can be cloned via

```
git clone --branch tutorial https://github.com/CSAILVision/gandissect.git
```

If you do not have git installed on your local machine, you can download the branch as a ZIP file with

```
wget https://github.com/CSAILVision/gandissect/archive/tutorial.zip
```

## Setup

To install everything needed from this repo, have `conda` available (`conda` installation instructions can be found [here](http://ganocracy.csail.mit.edu/tutorial/setup.html)),
and run:

```
script/setup_env.sh      # Create a conda environment with dependencies
script/make_dirs.sh      # Create the dataset and dissect directories
conda activate netd      # Enter the conda environment
pip install -v -e .      # Link the local netdissect package into the env
```

Then within the `notebooks` directory:
```
cd notebooks
jupyter notebook &
```

Then run the notebook `dissect_progan.ipynb`