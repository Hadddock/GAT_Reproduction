# GAT Reproduction
A repository containing files for reproducing the results of the ICLR 2018 confrence paper Graph Attention Networks, as well as pre-trained modesl for each dataset. This repository only contains files to reproduce the Transductive classification benchmarks of the paper.

# Dependencies

The script has been tested on Windows using a Conda environment under Python 3.5.2, with the following packages installed (along with their dependencies):

    numpy==1.14.1
    scipy==1.0.0
    networkx==2.1
    tensorflow-gpu==1.6.0

In addition, CUDA 9.0 and cuDNN 7 have been used.

# How to Run
1. Install the aforementioned dependencies in a virtual environment
2. Download and extract the repository
3. Run each of the dataset's respective scripts in the root of the repository in your virtual environment.

# Workarounds
Running execute_pubmed_sparse.py produced issues with my GPU not being compatible with CUDA 9.0, so I have opted to disable usage of the GPU in the script. To attempt to run the script with the GPU, simply comment out line 12 of execute_pubmed_sparse.py

# Acknowledgements
* GAT main repository can be found here: https://github.com/PetarV-/GAT. Most all of the code here is taken from the main GAT repository, with the only edits included to ease reproducing the results of the paper.
* See https://github.com/gordicaleksa/pytorch-GAT for reproducing the inductive benchmarks using pytorch and Tensorflow 2.0 (as well as the inductive benchmarks in pytorch)

